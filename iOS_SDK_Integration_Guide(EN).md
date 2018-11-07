# Getting Started with the Cloudmobi iOS SDK

- [Before You Start](#start)
- [SDK Set Up Use CocoaPods](#step1)
- [SDK Set Up Manually](#step2)
  - [Rewarded Video](#rewardedvideo)
  - [Native](#native)
  - [Banner](#banner)
  - [Native Video](#nativevideo)
  - [New Dynamic Interstitial（need create new dynamic interstitial slot）](#interstitial)
  - [AppWall](#Appwall)



## <a name="start">Before You Start</a>

- Cloudmobi iOS SDK supports banner, interstitial, native, and rewarded video 
- Cloudmobi iOS SDK will not support iOS 7, if your APP needs to supprot iOS 7,please download [SDK supports iOS 7](https://github.com/cloudmobi/iOS-SDK/blob/a1420dfcc148c196725723956b255114bf473a94/(CT)iOS-SDK.zip)
- Please make sure you have signed up on the Cloudmobi Platform. If you haven't signed up, please contact us via email: sdk_support@yeahmobi.com
- Please make sure you have added an app and at least one ad slot in Cloudmobi Platform
- Please download [our latest SDK](https://github.com/cloudmobi/iOS-SDK/raw/master/(CT)iOS-SDK.zip)

## <a name="step1">SDK Set Up Use CocoaPods </a>
* 1. Add the following line of code to the project of Podfile file : pod 'CTSDK' 
* 2. Running a 'pod install' command

## <a name="step2">SDK Set Up Manually</a>

* 1. Unzip the SDK package and drop CTSDK.framework k into your Xcode project.

PRO TIP: Checkmark the Copy items if needed option. This creates a local copy of the framework for your project, which keeps your project organized.

* 2. Link the StoreKit.framework, AVFoundation.framework, SystemConfiguration.framework, AdSupport.framework,JavaScriptCore.framework,ImageIO.framework, UIKit frameworks and libz.tbd .

**In Info.plist added the NSAppTransportSecurity**

```
<key>NSAppTransportSecurity</key>
<dict>
	<key>NSAllowsArbitraryLoads</key>
	<true/>
</dict>
```

* 3. You should add a static link to Xcode project: Build Settings -> Other Linker Flags -> -ObjC

* 4. Add the import header #import <CTSDK/CTSDK.h> to your 
     AppDelegate.m file.
     4.Initialize CTSDK in your didFinishLaunchingWithOptions method.

```
 - (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions {
        [[CTService shareManager] loadRequestGetCTSDKConfigBySlot_id:Your_Cloudmobi_slotID];
        return YES;
}
```
**Please make sure to initialize Cloudmobi SDK before doing anything.**

* 5. Add your Slot ID .

Replace Your_Cloudmobi_slotID with your Slot ID -- Where can I find my Slot ID? Please refer to the picture below

![image](https://user-images.githubusercontent.com/20314643/35969194-03005aa0-0d01-11e8-8d24-92a6b9882a77.png)


Use this interface to upload consent from affected users.

```
/**
 For GDPR

 @param consentValue  yes/no/other
 @param consentType   content type is the agreement name you signed with users
 @param complete      state
 */
- (void)uploadConsentValue:(NSString *)consentValue
	       consentType:(NSString *)consentType
		  complete:(void(^)(BOOL state))complete;
```


###  <a name="rewardedvideo">Adding the RewardVideo Ad API in iOS</a>
For the first time you request rewarded video ads, you may need to try serveral times.Because it takes a while to load the video files.Once a video file loads completely, it will response immediately.

```     
    /**
     * to get your rewarded video
     * 1. call loadRewardVideoWithSlotId:delegate:to get RewardVideo，if success, you can use the rewarded video to show
     * @param slot_Id       RewardVideo SlotID
     * @param delegate      declare that ViewController implements the CTRewardVideoDelegate protocol, and add a function that loads the Rewarded video.
     */
    - (void)loadRewardVideoWithSlotId:(NSString *)slot_id delegate:(id)delegate;
    /**
     show 
     @param viewController set present RewardVideo Viewcontroller
     */
    - (void)showRewardVideoWithPresentingViewController:(UIViewController *)viewController;
    /**
     Please check if the reward video works well before show it
     */
    - (BOOL)checkRewardVideoIsReady;
    /**
    set custom prameters for reward video
    @param customParams         
    */
    - (void)setCustomParameters:(NSString *)customParams;
    
    CTRewardVideoDelegate delegate callback interface
    - (void)CTRewardVideoLoadSuccess {
        NSLog(@"reward video is loaded and ready to be displayed");
    }                       
    - (void)CTRewardVideoDidStartPlaying {
        NSLog(@"reward video starts to play");
    }
    - (void)CTRewardVideoDidFinishPlaying {
        NSLog(@"reward video complete-this is called after a full video view,before end card is shown");
    } 
    - (void)CTRewardVideoDidClickRewardAd {
        NSLog(@"reward video clicked");
    }
    - (void)CTRewardVideoWillLeaveApplication {
        NSLog(@"users click reward video and leave application");
    } 
    - (void)CTRewardVideoJumpfailed {
        NSLog(@"reward video click and failed jumping to App Store");
    }
    - (void)CTRewardVideoLoadingFailed:(NSError *)error {
        NSLog(@"reward video request failed ");
    }
    - (void)CTRewardVideoClosed {
        NSLog(@"reward video ad closed-this can be triggered by closing the end card");
    }
    - (void)CTRewardVideoAdRewardedName:(NSString *)rewardName rewardAmount:(NSString *)rewardAmount customParams:(NSString*) customParams {
        NSLog(@"give reward to the users interface");
    }
```



### <a name="native">Adding the Native Ad API in iOS</a>

```
    /**
     * To get the Native ads , Your custom AD View should inherit CTNativeAd 
     * Because GDPR, you need to add touch events to the ad choices in the corner. user click the ad choices in the corner and it can be opened by safai choices_link_url.Ad choices uses ADsignImage object
     * @param slot_Id       Native Ad SlotID
     * @param delegate      declare that ViewController implements the CTNativeAdDelegate protocol
     * @param WHRate        Request image rate
     * @param isTest        Debug Mode , Retention parameters
     * @param success       Load Ad success callback
     * @param failure       Load Ad Failed callback
     */
    -(void)getNativeADswithSlotId:(NSString *)slot_id
                     delegate:(id)delegate
          imageWidthHightRate:(CTImageWidthHightRate)WHRate
                       isTest:(BOOL)isTest
                      success:(void (^)(CTNativeAdModel *nativeModel))success
                      failure:(void (^)(NSError *error))failure;
    /**
     * To get the multiple Native ads , Your custom AD View should inherit CTNativeAd 
     * Because GDPR, you need to add touch events to the ad choices in the corner. user click the ad choices in the corner and it can be opened by safai choices_link_url.Ad choices uses ADsignImage object
     * @param slot_Id       Native Ad SlotID
     * @param num           Ad numbers
     * @param delegate      declare that ViewController implements the CTNativeAdDelegate protocol
     * @param WHRate        Request image rate
     * @param isTest        Debug Mode , Retention parameters
     * @param success       Load Ad success callback
     * @param failure       Load Ad Failed callback
     */
    -(void)getMultitermNativeADswithSlotId:(NSString *)slot_id
                             adNumbers:(NSInteger)num
                              delegate:(id)delegate
                   imageWidthHightRate:(CTImageWidthHightRate)WHRate
                                isTest:(BOOL)isTest
                               success:(void (^)(NSArray *nativeArr))success
                               failure:(void (^)(NSError *error))failure;
                               
    CTNativeAdDelegate delegate callback interface
    - (void)CTNativeAdDidClick:(UIView *)nativeAd {
        NSLog(@"click Ad");
    }
    - (void)CTNativeAdDidIntoLandingPage:(UIView *)nativeAd {
        NSLog(@"did Into LandingPage");
    }
    - (void)CTNativeAdDidLeaveLandingPage:(UIView *)nativeAd {
        NSLog(@"did Leave LandingPage");
    }
    - (void)CTNativeAdWillLeaveApplication:(UIView *)nativeAd {
        NSLog(@"will Leave Application");
    }
    - (void)CTNativeAdJumpfail:(UIView *)nativeAd {
        NSLog(@"click ad Jump App store failed");
    }

```


### <a name="banner">Adding the Banner Ad API in iOS</a>

Cloudmobi SDK supports three ad sizes banner to be used in your APP.

|Ad format| Size | Reconmmandation |
|--|--|--|
|CTADBannerSizeW320H50|320x50| highly reconmmanded for mobile phone APP |
|CTADBannerSizeW320H100|320x100|recommanded for tablets or larger devices| 
|CTADBannerSizeW300H250|300x250|recommanded for tablets or moblie phone |

```
    /**
    *Get Banner Ad View
    *@param slot_id         Cloud Tech Banner AD ID
    *@param delegate        Set Delegate of Ad event(<CTAdViewDelegate>)
    *@param adSize          Ad size. enum CTADBannerSize:CTADBannerSizeW320H50, CTADBannerSizeW320H100, CTADBannerSizeW300H250
    *@param isTest          Use test advertisement or not
    */
    
    - (void)getMRAIDBannerAdWithSlot:(NSString*)slotid delegate:(id)delegate adSize:(CTADBannerSize)size isTest:(BOOL)isTest;

    CTAdViewDelegate interfaces related to banner, for more detail please check CTAdviewDelegate in CTADMRAIDView.h
    //banner ad
    - (void)CTAdViewDidRecieveBannerAd:(CTADMRAIDView*)adView{
        NSLog(@"receive CT banner");
    }
    //error while request ads.
    - (void)CTAdView:(CTADMRAIDView*)adView didFailToReceiveAdWithError:(NSError*)error{
        NSLog(@"request CT ads with error");
    }
    //click ad
    - (void)CTAdViewClicked:(CTADMRAIDView*)adView{
        NSLog(@"user click ad");
    }
    //mraid ad show
    - (void)CTAdMaridAdShow:(CTADMRAIDView*)adView{
    	NSLog(@"ad is show");
    }
    
```
when you successfully integrated the Banner Ad, you will see the ads are like this


![-1](https://user-images.githubusercontent.com/20314643/42366029-b6289f2a-8132-11e8-9c3e-86557d164d85.png)
![320x100](https://user-images.githubusercontent.com/20314643/42370991-c4188812-8140-11e8-80e9-ab6947c12e92.png)
![300x250](https://user-images.githubusercontent.com/20314643/42370999-c74139f8-8140-11e8-91ff-ba0cdb0ae08a.png)

### <a name="nativevideo">Adding the Native Video Ad API in iOS</a>
iOS SDK supports two ways to use native video. One is like Elements Ad which SDK supports videoview, background image and interface to controll video play or stop. Developers should notice that video won't play in 3g/4g, we should add a background image and play button image(we both offer in delegate function) instead. User click the images to present a custom video controller, with user's permission to play video. The other is like mediaview. We recommend to use mediaview, beacuse developers don't need to worry about the issue, mediaview will do this for you. For more detail you should check our demo.https://github.com/cloudmobi/iOS-SDK/blob/master/CT_iOS_Demo.zip
```
/**
 Get Native video Ad
 Call this interface to get Native Video AD.
 Because GDPR, you need to add touch events to the ad choices in the corner. user click the ad choices in the corner and it can be opened by safai choices_link_url.Ad choices uses ADsignImage object
 @param slot_id         You should use Native Video AD ID or you wouldn't get ads.
 @param delegate        Set Delegate of Ads event (<CTNativeVideoDelegate>)
 @param WHRate          Set Image Rate
 @param isTest          Use test advertisement or not
 */
- (void)getNativeVideoADswithSlotId:(NSString*)slot_id
                           delegate:(id)delegate
                imageWidthHightRate:(CTImageWidthHightRate)WHRate
                             isTest:(BOOL)isTest;
			  
CTNativeVideoDelegate Callback Delegate
-(void)CTNativeVideoLoadSuccess:(CTNativeVideoModel *)nativeVideoModel;  //Advertisement load success.
-(void)CTNativeVideoLoadFailed:(NSError *)error;                         //Advertisement load failed
```

![image](https://user-images.githubusercontent.com/20314643/42367439-d567e9be-8136-11e8-85df-c9eeacf270d9.png)

### <a name="interstitial">Adding the New Dynamic Interstitial Ad API in iOS</a>

Interstitial ads are full-screen ads that cover the interface of the host app.

```
    /**
     Preload Interstitial Ad
     Call this interface preload Interstitial AD.
 
     @param slot_id         Cloud Tech AD ID
     @param delegate        Set Delegate of Ads event (<CTAdViewDelegate>)
     @param isTest          Use test advertisement or not
     */
    - (void)preloadMRAIDInterstitialAdWithSlotId:(NSString *)slotid delegate:(id)delegate isTest:(BOOL)isTest;

    /**
     Show interstitial ad
     Call this method after preload Interstitial ad success
     */
    - (void)mraidInterstitialShow;

    /**
     Check interstitial ad to be Ready
     Call this method before show ad
     */
    - (BOOL)mraidInterstitialIsReady;
    
    
    CTAdViewDelegate interfaces related to interstitial, for more detail please check CTAdviewDelegate in CTADMRAIDView.h
    //interstitial is ready, call mraidInterstitialShow to show it.
    - (void)CTAdViewDidRecieveInterstitialAd{
    	NSLog(@"receive CT Interstitial");
    }
    
    //error while request ads. (share the same error delegate interface with banner)
    - (void)CTAdView:(CTADMRAIDView*)adView didFailToReceiveAdWithError:(NSError*)error{
    	NSLog(@"request CT ads with error");
    }
    
    //click ad
    - (void)CTAdViewClicked:(CTADMRAIDView*)adView{
        NSLog(@"user click ad");
    }
    
    //mraid ad show
    - (void)CTAdMaridAdShow:(CTADMRAIDView*)adView{
    	NSLog(@"ad is show");
    }
    
```


**IMPORTANT: If you got the error message:"not interstitial slot",please check if the ad format in SSP is the same with the API in SDK.

when you successfully integrated the New Dynamic Interstitial Ad, you will see the ads are like this

![image](https://user-images.githubusercontent.com/20314643/41895879-b4536200-7955-11e8-9847-587f175c4a54.png)
![image](https://user-images.githubusercontent.com/20314643/41895941-e0c6ad1a-7955-11e8-9393-ed91e4a4906f.png)


### <a name="Appwall">Adding the Appwall Ad API in iOS</a>

Appwall ads are full-screen ads that cover the interface of the host app.

```
    /**
     Get AppWall ViewController
     First,you must should Call preloadAppWallWithSlotID method,Then get successs,call showAppWallViewController method show Appwall！
 
     @param slot_id         Cloud Tech Native AD ID
     @param customColor     If you want set custom UI,you should create CTCustomColor object
     param delegate        Set Delegate of Ads event (<CTAppWallDelegate>)
     @param isTest          Use test advertisement or not
     @param success         The request is successful Block
     @param failure         The request failed Block, retuen error
     */
    - (void)preloadAppWallWithSlotID:(NSString *)slot_id
                     customColor:(CTCustomColor *)customColor
                        delegate:(id)delegate
                          isTest:(BOOL)isTest
                         success:(void(^)())success
                         failure:(void(^)(NSError *error))failure;
			 
     /**
     Get App Wall ViewController

     @return AppWallViewController
     */
     - (UIViewController *)showAppWallViewController;

     CTAppWallDelegate interfaces related to Appwall, for more detail please check CTAppWallDelegate in CTADExternalDelegate.h
     
     /**
     * User click the advertisement.
     */
    -(void)CTAppWallDidClick:(CTNativeAd *)nativeAd;
    /**
     * Advertisement landing page will show.
     */
     -(void)CTAppWallDidIntoLandingPage:(CTNativeAd *)nativeAd;
    /**
     * User left the advertisement landing page.
     */
    -(void)CTAppWallDidLeaveLandingPage:(CTNativeAd *)nativeAd;
    /**
     * Leave App
     */
    -(void)CTAppWallWillLeaveApplication:(CTNativeAd *)nativeAd;
    /**
     * User close the advertisement.
     */
    -(void)CTAppWallClosed;
    /**
     * Jump failure
     */
    -(void)CTAppWallJumpfail:(CTNativeAd*)nativeAd;

```
![image](https://user-images.githubusercontent.com/20314643/42366246-47526c9c-8133-11e8-963c-bd0eb7a3e1a6.png)


Done!

You are now all set to deliver Cloudmobi Ads within your application!


