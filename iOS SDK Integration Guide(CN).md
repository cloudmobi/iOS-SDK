





<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
  <link rel="dns-prefetch" href="https://assets-cdn.github.com">
  <link rel="dns-prefetch" href="https://avatars0.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars1.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars2.githubusercontent.com">
  <link rel="dns-prefetch" href="https://avatars3.githubusercontent.com">
  <link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
  <link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">



  <link crossorigin="anonymous" media="all" integrity="sha512-hqbuBb0QOOmiWgl8a1V1N5q6TI/G0A2hVt/lCFYafR+fYsuXeRUcsdcb/yUyVEHYXktmUXl0Mx9s/BOUNZVq4w==" rel="stylesheet" href="https://assets-cdn.github.com/assets/frameworks-23c9e7262eee71bc6f67f6950190a162.css" />
  <link crossorigin="anonymous" media="all" integrity="sha512-eIYYJSKqUtZ1wca1cjvRpEFVDVFlRed6ZF1jtZ0E+plPCBYpZd78jUtSlGbFFouH9uhlhGRztTLDLwmNU6rL8w==" rel="stylesheet" href="https://assets-cdn.github.com/assets/github-50c729cf7e55c7554c6d0ceae2a0e938.css" />
  
  
  
  

  <meta name="viewport" content="width=device-width">
  
  <title>CloudmobiSSP/CloudMobi-iOS_CTSDK_入门指南.md at master · cloudmobi/CloudmobiSSP</title>
    <meta name="description" content="GitHub is where people build software. More than 27 million people use GitHub to discover, fork, and contribute to over 80 million projects.">
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
  <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
  <meta property="fb:app_id" content="1401488693436528">

    
    <meta property="og:image" content="https://avatars0.githubusercontent.com/u/20926510?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="cloudmobi/CloudmobiSSP" /><meta property="og:url" content="https://github.com/cloudmobi/CloudmobiSSP" /><meta property="og:description" content="Contribute to CloudmobiSSP development by creating an account on GitHub." />

  <link rel="assets" href="https://assets-cdn.github.com/">
  <link rel="web-socket" href="wss://live.github.com/_sockets/VjI6MjcxOTI5NzgyOjQ3YWFhM2ZlZjZhYTJlODgyZjU2M2IzMzZkMzhlZWQ1ZjRjMTFhMDEyN2RjYWNmZTY4MjE2OGVjMmJmZjkxOWI=--c4327d15c7652c6582a296024f25113a7c0d1a72">
  <meta name="pjax-timeout" content="1000">
  <link rel="sudo-modal" href="/sessions/sudo_modal">
  <meta name="request-id" content="C988:0A51:F0C54A:162EE35:5B0CE35A" data-pjax-transient>


  

  <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
  <meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
  <meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">
    <meta name="google-analytics" content="UA-3769691-2">

<meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-request_id" content="C988:0A51:F0C54A:162EE35:5B0CE35A" /><meta name="octolytics-dimension-region_edge" content="ap-southeast-1" /><meta name="octolytics-dimension-region_render" content="iad" /><meta name="octolytics-actor-id" content="15391506" /><meta name="octolytics-actor-login" content="lanxuping" /><meta name="octolytics-actor-hash" content="1eac08f646faf4c6362d9def6d0df2ea417c57b1680054235d08f386800e8d2c" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />




  <meta class="js-ga-set" name="dimension1" content="Logged In">


  

      <meta name="hostname" content="github.com">
    <meta name="user-login" content="lanxuping">

      <meta name="expected-hostname" content="github.com">
    <meta name="js-proxy-site-detection-payload" content="ZWNlZWY1Y2MzMjRhZjIwMjJjZTgxODVhNTRiYWYzNDJiZDQwMGVhNDlkMmZhOTJjMGNjM2I2OTVmZjExZTAyNnx7InJlbW90ZV9hZGRyZXNzIjoiNDcuNzUuMTgyLjAiLCJyZXF1ZXN0X2lkIjoiQzk4ODowQTUxOkYwQzU0QToxNjJFRTM1OjVCMENFMzVBIiwidGltZXN0YW1wIjoxNTI3NTcxMjk5LCJob3N0IjoiZ2l0aHViLmNvbSJ9">

    <meta name="enabled-features" content="UNIVERSE_BANNER,FREE_TRIALS,MARKETPLACE_INSIGHTS,MARKETPLACE_INSIGHTS_CONVERSION_PERCENTAGES,JUMP_TO">

  <meta name="html-safe-nonce" content="1b6bc3045320adc8c06362058a66629ae2ad1399">

  <meta http-equiv="x-pjax-version" content="d61b8f905649c50cd9e9d08c95e4c006">
  

      <link href="https://github.com/cloudmobi/CloudmobiSSP/commits/master.atom" rel="alternate" title="Recent Commits to CloudmobiSSP:master" type="application/atom+xml">

  <meta name="description" content="Contribute to CloudmobiSSP development by creating an account on GitHub.">
  <meta name="go-import" content="github.com/cloudmobi/CloudmobiSSP git https://github.com/cloudmobi/CloudmobiSSP.git">

  <meta name="octolytics-dimension-user_id" content="20926510" /><meta name="octolytics-dimension-user_login" content="cloudmobi" /><meta name="octolytics-dimension-repository_id" content="65290227" /><meta name="octolytics-dimension-repository_nwo" content="cloudmobi/CloudmobiSSP" /><meta name="octolytics-dimension-repository_public" content="true" /><meta name="octolytics-dimension-repository_is_fork" content="false" /><meta name="octolytics-dimension-repository_network_root_id" content="65290227" /><meta name="octolytics-dimension-repository_network_root_nwo" content="cloudmobi/CloudmobiSSP" /><meta name="octolytics-dimension-repository_explore_github_marketplace_ci_cta_shown" content="false" />


    <link rel="canonical" href="https://github.com/cloudmobi/CloudmobiSSP/blob/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md" data-pjax-transient>


  <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">

  <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">

  <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#000000">
  <link rel="icon" type="image/x-icon" class="js-site-favicon" href="https://assets-cdn.github.com/favicon.ico">

<meta name="theme-color" content="#1e2327">


  <meta name="u2f-support" content="true">

<link rel="manifest" href="/manifest.json" crossOrigin="use-credentials">

  </head>

  <body class="logged-in env-production emoji-size-boost page-blob">
    

  <div class="position-relative js-header-wrapper ">
    <a href="#start-of-content" tabindex="1" class="p-3 bg-blue text-white show-on-focus js-skip-to-content">Skip to content</a>
    <div id="js-pjax-loader-bar" class="pjax-loader-bar"><div class="progress"></div></div>

    
    
    



        
<header class="Header  f5" role="banner">
  <div class="d-flex flex-justify-between px-3 container-lg">
    <div class="d-flex flex-justify-between ">
      <div class="">
        <a class="header-logo-invertocat" href="https://github.com/" data-hotkey="g d" aria-label="Homepage" data-ga-click="Header, go to dashboard, icon:logo">
  <svg height="32" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="32" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>

      </div>

    </div>

    <div class="HeaderMenu d-flex flex-justify-between flex-auto">
      <div class="d-flex">
            <div class="">
              <div class="header-search scoped-search site-scoped-search js-site-search position-relative" role="search">
  <div class="position-relative">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-site-search-form" data-scope-type="Repository" data-scope-id="65290227" data-scoped-search-url="/cloudmobi/CloudmobiSSP/search" data-unscoped-search-url="/search" action="/cloudmobi/CloudmobiSSP/search" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
      <label class="form-control header-search-wrapper header-search-wrapper-jump-to position-relative d-flex flex-justify-between flex-items-center js-chromeless-input-container">
        <input type="text"
          class="form-control header-search-input jump-to-field js-jump-to-field js-site-search-focus js-site-search-field is-clearable"
          data-hotkey="s,/"
          name="q"
          value=""
          placeholder="Search or jump to…"
          aria-label="Search this repository"
          data-unscoped-placeholder="Search or jump to…"
          data-scoped-placeholder="Search or jump to…"
          data-jump-to-suggestions-path="/_graphql/GetSuggestedNavigationDestinations#csrf-token=hJElCTU/EkgNmXthVQneu0rWTb9H1+sqe2VH16Nc5t7Fb4yc/RHEThgGTZSXmz7GzpMj58V5C1eroeINgtxHhA=="
          spellcheck="false"
          autocomplete="off"
          autocapitalize="off"
          >
          <input type="hidden" class="js-site-search-type-field" name="type" >
            <img src="https://assets-cdn.github.com/images/search-shortcut-hint.svg" alt="" class="mr-2 header-search-key-slash">

            <div class="Box position-absolute overflow-hidden d-none jump-to-suggestions js-jump-to-suggestions-container">
              <ul class="d-none js-jump-to-suggestions-template-container">
                <li class="d-flex flex-justify-start flex-items-center p-0 f5 navigation-item js-navigation-item">
                  <a class="no-underline d-flex flex-auto flex-items-center p-2 jump-to-suggestions-path js-jump-to-suggestion-path js-navigation-open" aria-label="Jump to..." href="">
                    <div class="jump-to-octicon js-jump-to-octicon mr-2 text-center d-none"></div>
                    <img class="avatar mr-2 flex-shrink-0 js-jump-to-suggestion-avatar" alt="" src="" width="28" height="28">
                    <div class="jump-to-suggestion-name js-jump-to-suggestion-name flex-auto overflow-hidden no-wrap css-truncate css-truncate-target">
                    </div>

                    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-search">
                      In this repository
                      <span class="d-inline-block ml-1 v-align-middle">↵</span>
                    </div>

                    <div class="border rounded-1 flex-shrink-0 bg-gray px-1 text-gray-light ml-1 f6 d-none d-on-nav-focus js-jump-to-badge-jump">
                      Jump to
                      <span class="d-inline-block ml-1 v-align-middle">↵</span>
                    </div>
                  </a>
                </li>
                <svg height="16" width="16" class="octicon octicon-repo flex-shrink-0 js-jump-to-repo-octicon-template" title="Repository" viewBox="0 0 12 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
                <svg height="16" width="16" class="octicon octicon-project flex-shrink-0 js-jump-to-project-octicon-template" title="Project" viewBox="0 0 15 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
                <svg height="16" width="16" class="octicon octicon-search flex-shrink-0 js-jump-to-search-octicon-template" title="Search" viewBox="0 0 16 16" version="1.1" aria-hidden="true"><path fill-rule="evenodd" d="M15.7 13.3l-3.81-3.83A5.93 5.93 0 0 0 13 6c0-3.31-2.69-6-6-6S1 2.69 1 6s2.69 6 6 6c1.3 0 2.48-.41 3.47-1.11l3.83 3.81c.19.2.45.3.7.3.25 0 .52-.09.7-.3a.996.996 0 0 0 0-1.41v.01zM7 10.7c-2.59 0-4.7-2.11-4.7-4.7 0-2.59 2.11-4.7 4.7-4.7 2.59 0 4.7 2.11 4.7 4.7 0 2.59-2.11 4.7-4.7 4.7z"/></svg>
              </ul>
              <ul class="d-none js-jump-to-no-results-template-container">
                <li class="d-flex flex-justify-center flex-items-center p-3 f5 d-none">
                  <span class="text-gray">No suggested jump to results</span>
                </li> 
              </ul>

              <ul class="js-navigation-container jump-to-suggestions-results-container js-jump-to-suggestions-results-container">
                <li class="d-flex flex-justify-center flex-items-center p-0 f5">
                  <img src="https://assets-cdn.github.com/images/spinners/octocat-spinner-128.gif" alt="Octocat Spinner Icon" class="m-2" width="28">
                </li>
              </ul>
            </div>
      </label>
</form>  </div>
</div>

            </div>

          <ul class="d-flex pl-2 flex-items-center text-bold list-style-none" role="navigation">
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-hotkey="g p" data-ga-click="Header, click, Nav menu - item:pulls context:user" aria-label="Pull requests you created" data-selected-links="/pulls /pulls/assigned /pulls/mentioned /pulls" href="/pulls">
                Pull requests
</a>            </li>
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-hotkey="g i" data-ga-click="Header, click, Nav menu - item:issues context:user" aria-label="Issues you created" data-selected-links="/issues /issues/assigned /issues/mentioned /issues" href="/issues">
                Issues
</a>            </li>
                <li>
                  <a class="js-selected-navigation-item HeaderNavlink px-2" data-ga-click="Header, click, Nav menu - item:marketplace context:user" data-octo-click="marketplace_click" data-octo-dimensions="location:nav_bar, group:apps_text" data-selected-links=" /marketplace" href="/marketplace">
                    Apps
</a>                </li>
            <li>
              <a class="js-selected-navigation-item HeaderNavlink px-2" data-ga-click="Header, click, Nav menu - item:explore" data-selected-links="/explore /trending /trending/developers /integrations /integrations/feature/code /integrations/feature/collaborate /integrations/feature/ship showcases showcases_search showcases_landing /explore" href="/explore">
                Explore
</a>            </li>
          </ul>
      </div>

      <div class="d-flex">
        
<ul class="user-nav d-flex flex-items-center list-style-none" id="user-links">
  <li class="dropdown js-menu-container">
    <span class="d-inline-block  px-2">
      
    <a aria-label="You have unread notifications" class="notification-indicator tooltipped tooltipped-s  js-socket-channel js-notification-indicator" data-hotkey="g n" data-ga-click="Header, go to notifications, icon:unread" data-channel="notification-changed:15391506" href="/notifications">
        <span class="mail-status unread"></span>
        <svg class="octicon octicon-bell" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M13.99 11.991v1H0v-1l.73-.58c.769-.769.809-2.547 1.189-4.416.77-3.767 4.077-4.996 4.077-4.996 0-.55.45-1 .999-1 .55 0 1 .45 1 1 0 0 3.387 1.229 4.156 4.996.38 1.879.42 3.657 1.19 4.417l.659.58h-.01zM6.995 15.99c1.11 0 1.999-.89 1.999-1.999H4.996c0 1.11.89 1.999 1.999 1.999z"/></svg>
</a>
    </span>
  </li>

  <li class="dropdown js-menu-container">
    <details class="details-expanded details-reset js-dropdown-details d-flex px-2 flex-items-center">
      <summary class="HeaderNavlink"
         aria-label="Create new…"
         data-ga-click="Header, create new, icon:add">
        <svg class="octicon octicon-plus float-left mr-1 mt-1" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 9H7v5H5V9H0V7h5V2h2v5h5v2z"/></svg>
        <span class="dropdown-caret mt-1"></span>
      </summary>

      <ul class="dropdown-menu dropdown-menu-sw">
        
<a class="dropdown-item" href="/new" data-ga-click="Header, create new repository">
  New repository
</a>

  <a class="dropdown-item" href="/new/import" data-ga-click="Header, import a repository">
    Import repository
  </a>

<a class="dropdown-item" href="https://gist.github.com/" data-ga-click="Header, create new gist">
  New gist
</a>

  <a class="dropdown-item" href="/organizations/new" data-ga-click="Header, create new organization">
    New organization
  </a>



  <div class="dropdown-divider"></div>
  <div class="dropdown-header">
    <span title="cloudmobi/CloudmobiSSP">This repository</span>
  </div>
    <a class="dropdown-item" href="/cloudmobi/CloudmobiSSP/issues/new" data-ga-click="Header, create new issue">
      New issue
    </a>

      </ul>
    </details>
  </li>

  <li class="dropdown js-menu-container">

    <details class="details-expanded details-reset js-dropdown-details d-flex pl-2 flex-items-center">
      <summary class="HeaderNavlink name mt-1"
        aria-label="View profile and more"
        data-ga-click="Header, show menu, icon:avatar">
        <img alt="@lanxuping" class="avatar float-left mr-1" src="https://avatars3.githubusercontent.com/u/15391506?s=40&amp;v=4" height="20" width="20">
        <span class="dropdown-caret"></span>
      </summary>

      <ul class="dropdown-menu dropdown-menu-sw">
        <li class="dropdown-header header-nav-current-user css-truncate">
          Signed in as <strong class="css-truncate-target">lanxuping</strong>
        </li>

        <li class="dropdown-divider"></li>

        <li><a class="dropdown-item" href="/lanxuping" data-ga-click="Header, go to profile, text:your profile">
          Your profile
        </a></li>
        <li><a class="dropdown-item" href="/lanxuping?tab=stars" data-ga-click="Header, go to starred repos, text:your stars">
          Your stars
        </a></li>
          <li><a class="dropdown-item" href="https://gist.github.com/" data-ga-click="Header, your gists, text:your gists">Your gists</a></li>

        <li class="dropdown-divider"></li>

        <li><a class="dropdown-item" href="https://help.github.com" data-ga-click="Header, go to help, text:help">
          Help
        </a></li>

        <li><a class="dropdown-item" href="/settings/profile" data-ga-click="Header, go to settings, icon:settings">
          Settings
        </a></li>

        <li><!-- '"` --><!-- </textarea></xmp> --></option></form><form class="logout-form" action="/logout" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="waYKg+HpIYZAPK0c696Fg6iTr4gg7rxlQh90Qv6MdZN7j9etwQYwNegZ/YgqhBJC+Kg06D0+fuYTFd3UK12wAA==" />
          <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
            Sign out
          </button>
        </form></li>
      </ul>
    </details>
  </li>
</ul>



        <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="sr-only right-0" action="/logout" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="yDIvyE9SJNIlyIfcS2OEJ/sCnmNeg4k9yDBihizLH5RyG/Lmb701YY3t10iKORPmqzkFA0NTS76ZOssQ+RraBw==" />
          <button type="submit" class="dropdown-item dropdown-signout" data-ga-click="Header, sign out, icon:logout">
            Sign out
          </button>
</form>      </div>
    </div>
  </div>
</header>

      

  </div>

  <div id="start-of-content" class="show-on-focus"></div>

    <div id="js-flash-container">
</div>



  <div role="main" class="application-main ">
        <div itemscope itemtype="http://schema.org/SoftwareSourceCode" class="">
    <div id="js-repo-pjax-container" data-pjax-container >
      





  



  <div class="pagehead repohead instapaper_ignore readability-menu experiment-repo-nav  ">
    <div class="repohead-details-container clearfix container">

      <ul class="pagehead-actions">
  <li>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form data-autosubmit="true" data-remote="true" class="js-social-container" action="/notifications/subscribe" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="bb4kKzXQwdvU3QncIBQshTBQkPJFz5Kb3jccUlwT6YanCa2OOOZsDiTT5IqpyMlFiYdM6fhYq2mSPBw9klH5Ng==" />      <input type="hidden" name="repository_id" id="repository_id" value="65290227" class="form-control" />

        <div class="select-menu js-menu-container js-select-menu">
          <a href="/cloudmobi/CloudmobiSSP/subscription"
            class="btn btn-sm btn-with-count select-menu-button js-menu-target"
            role="button"
            aria-haspopup="true"
            aria-expanded="false"
            aria-label="Toggle repository notifications menu"
            data-ga-click="Repository, click Watch settings, action:blob#show">
            <span class="js-select-button">
                <svg class="octicon octicon-eye" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                Watch
            </span>
          </a>
          <a class="social-count js-social-count"
            href="/cloudmobi/CloudmobiSSP/watchers"
            aria-label="2 users are watching this repository">
            2
          </a>

        <div class="select-menu-modal-holder">
          <div class="select-menu-modal subscription-menu-modal js-menu-content">
            <div class="select-menu-header js-navigation-enable" tabindex="-1">
              <svg class="octicon octicon-x js-menu-close" role="img" aria-label="Close" viewBox="0 0 12 16" version="1.1" width="12" height="16"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
              <span class="select-menu-title">Notifications</span>
            </div>

              <div class="select-menu-list js-navigation-container" role="menu">

                <div class="select-menu-item js-navigation-item selected" role="menuitem" tabindex="0">
                  <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
                  <div class="select-menu-item-text">
                    <input type="radio" name="do" id="do_included" value="included" checked="checked" />
                    <span class="select-menu-item-heading">Not watching</span>
                    <span class="description">Be notified when participating or @mentioned.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg class="octicon octicon-eye" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                      Watch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
                  <div class="select-menu-item-text">
                    <input type="radio" name="do" id="do_subscribed" value="subscribed" />
                    <span class="select-menu-item-heading">Watching</span>
                    <span class="description">Be notified of all conversations.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg class="octicon octicon-eye" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.06 2C3 2 0 8 0 8s3 6 8.06 6C13 14 16 8 16 8s-3-6-7.94-6zM8 12c-2.2 0-4-1.78-4-4 0-2.2 1.8-4 4-4 2.22 0 4 1.8 4 4 0 2.22-1.78 4-4 4zm2-4c0 1.11-.89 2-2 2-1.11 0-2-.89-2-2 0-1.11.89-2 2-2 1.11 0 2 .89 2 2z"/></svg>
                        Unwatch
                    </span>
                  </div>
                </div>

                <div class="select-menu-item js-navigation-item " role="menuitem" tabindex="0">
                  <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
                  <div class="select-menu-item-text">
                    <input type="radio" name="do" id="do_ignore" value="ignore" />
                    <span class="select-menu-item-heading">Ignoring</span>
                    <span class="description">Never be notified.</span>
                    <span class="js-select-button-text hidden-select-button-text">
                      <svg class="octicon octicon-mute" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 2.81v10.38c0 .67-.81 1-1.28.53L3 10H1c-.55 0-1-.45-1-1V7c0-.55.45-1 1-1h2l3.72-3.72C7.19 1.81 8 2.14 8 2.81zm7.53 3.22l-1.06-1.06-1.97 1.97-1.97-1.97-1.06 1.06L11.44 8 9.47 9.97l1.06 1.06 1.97-1.97 1.97 1.97 1.06-1.06L13.56 8l1.97-1.97z"/></svg>
                        Stop ignoring
                    </span>
                  </div>
                </div>

              </div>

            </div>
          </div>
        </div>
</form>
  </li>

  <li>
    
  <div class="js-toggler-container js-social-container starring-container ">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="starred js-social-form" action="/cloudmobi/CloudmobiSSP/unstar" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="xq9wola5idrEfzF/zCNT3Gpx1JLhqAK99Rt/dJHtRa72XJFjKc06s5mCyMqom9ZWCtZVGz9l0gsf6VK7bcs2xw==" />
      <input type="hidden" name="context" value="repository"></input>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Unstar this repository" title="Unstar cloudmobi/CloudmobiSSP"
        data-ga-click="Repository, click unstar button, action:blob#show; text:Unstar">
        <svg class="octicon octicon-star" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
        Unstar
      </button>
        <a class="social-count js-social-count" href="/cloudmobi/CloudmobiSSP/stargazers"
           aria-label="21 users starred this repository">
          21
        </a>
</form>
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="unstarred js-social-form" action="/cloudmobi/CloudmobiSSP/star" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="qUKRglZxMy4qGDdDQytp9nbsFuBpez+TvqCxfGkfoNWBYT42CX2jwVvAHBrPfTNHU5yMZRBFm3iJFv/IM17XYw==" />
      <input type="hidden" name="context" value="repository"></input>
      <button
        type="submit"
        class="btn btn-sm btn-with-count js-toggler-target"
        aria-label="Star this repository" title="Star cloudmobi/CloudmobiSSP"
        data-ga-click="Repository, click star button, action:blob#show; text:Star">
        <svg class="octicon octicon-star" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M14 6l-4.9-.64L7 1 4.9 5.36 0 6l3.6 3.26L2.67 14 7 11.67 11.33 14l-.93-4.74L14 6z"/></svg>
        Star
      </button>
        <a class="social-count js-social-count" href="/cloudmobi/CloudmobiSSP/stargazers"
           aria-label="21 users starred this repository">
          21
        </a>
</form>  </div>

  </li>

  <li>
          <a href="#fork-destination-box" class="btn btn-sm btn-with-count"
              title="Fork your own copy of cloudmobi/CloudmobiSSP to your account"
              aria-label="Fork your own copy of cloudmobi/CloudmobiSSP to your account"
              rel="facebox"
              data-ga-click="Repository, show fork modal, action:blob#show; text:Fork">
              <svg class="octicon octicon-repo-forked" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8 1a1.993 1.993 0 0 0-1 3.72V6L5 8 3 6V4.72A1.993 1.993 0 0 0 2 1a1.993 1.993 0 0 0-1 3.72V6.5l3 3v1.78A1.993 1.993 0 0 0 5 15a1.993 1.993 0 0 0 1-3.72V9.5l3-3V4.72A1.993 1.993 0 0 0 8 1zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3 10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm3-10c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
            Fork
          </a>

          <div id="fork-destination-box" style="display: none;">
            <h2 class="facebox-header" data-facebox-id="facebox-header">Where should we fork this repository?</h2>
            <include-fragment src=""
                class="js-fork-select-fragment fork-select-fragment"
                data-url="/cloudmobi/CloudmobiSSP/fork?fragment=1">
              <img alt="Loading" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-128.gif" width="64" height="64" />
            </include-fragment>
          </div>

    <a href="/cloudmobi/CloudmobiSSP/network" class="social-count"
       aria-label="10 users forked this repository">
      10
    </a>
  </li>
</ul>

      <h1 class="public ">
  <svg class="octicon octicon-repo" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9H3V8h1v1zm0-3H3v1h1V6zm0-2H3v1h1V4zm0-2H3v1h1V2zm8-1v12c0 .55-.45 1-1 1H6v2l-1.5-1.5L3 16v-2H1c-.55 0-1-.45-1-1V1c0-.55.45-1 1-1h10c.55 0 1 .45 1 1zm-1 10H1v2h2v-1h3v1h5v-2zm0-10H2v9h9V1z"/></svg>
  <span class="author" itemprop="author"><a class="url fn" rel="author" href="/cloudmobi">cloudmobi</a></span><!--
--><span class="path-divider">/</span><!--
--><strong itemprop="name"><a data-pjax="#js-repo-pjax-container" href="/cloudmobi/CloudmobiSSP">CloudmobiSSP</a></strong>

</h1>

    </div>
    
<nav class="reponav js-repo-nav js-sidenav-container-pjax container"
     itemscope
     itemtype="http://schema.org/BreadcrumbList"
     role="navigation"
     data-pjax="#js-repo-pjax-container">

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a class="js-selected-navigation-item selected reponav-item" itemprop="url" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches repo_packages /cloudmobi/CloudmobiSSP" href="/cloudmobi/CloudmobiSSP">
      <svg class="octicon octicon-code" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M9.5 3L8 4.5 11.5 8 8 11.5 9.5 13 14 8 9.5 3zm-5 0L0 8l4.5 5L6 11.5 2.5 8 6 4.5 4.5 3z"/></svg>
      <span itemprop="name">Code</span>
      <meta itemprop="position" content="1">
</a>  </span>

    <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
      <a itemprop="url" data-hotkey="g i" class="js-selected-navigation-item reponav-item" data-selected-links="repo_issues repo_labels repo_milestones /cloudmobi/CloudmobiSSP/issues" href="/cloudmobi/CloudmobiSSP/issues">
        <svg class="octicon octicon-issue-opened" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7 2.3c3.14 0 5.7 2.56 5.7 5.7s-2.56 5.7-5.7 5.7A5.71 5.71 0 0 1 1.3 8c0-3.14 2.56-5.7 5.7-5.7zM7 1C3.14 1 0 4.14 0 8s3.14 7 7 7 7-3.14 7-7-3.14-7-7-7zm1 3H6v5h2V4zm0 6H6v2h2v-2z"/></svg>
        <span itemprop="name">Issues</span>
        <span class="Counter">0</span>
        <meta itemprop="position" content="2">
</a>    </span>

  <span itemscope itemtype="http://schema.org/ListItem" itemprop="itemListElement">
    <a data-hotkey="g p" itemprop="url" class="js-selected-navigation-item reponav-item" data-selected-links="repo_pulls checks /cloudmobi/CloudmobiSSP/pulls" href="/cloudmobi/CloudmobiSSP/pulls">
      <svg class="octicon octicon-git-pull-request" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 11.28V5c-.03-.78-.34-1.47-.94-2.06C9.46 2.35 8.78 2.03 8 2H7V0L4 3l3 3V4h1c.27.02.48.11.69.31.21.2.3.42.31.69v6.28A1.993 1.993 0 0 0 10 15a1.993 1.993 0 0 0 1-3.72zm-1 2.92c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zM4 3c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v6.56A1.993 1.993 0 0 0 2 15a1.993 1.993 0 0 0 1-3.72V4.72c.59-.34 1-.98 1-1.72zm-.8 10c0 .66-.55 1.2-1.2 1.2-.65 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2zM2 4.2C1.34 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
      <span itemprop="name">Pull requests</span>
      <span class="Counter">0</span>
      <meta itemprop="position" content="3">
</a>  </span>

    <a data-hotkey="g b" class="js-selected-navigation-item reponav-item" data-selected-links="repo_projects new_repo_project repo_project /cloudmobi/CloudmobiSSP/projects" href="/cloudmobi/CloudmobiSSP/projects">
      <svg class="octicon octicon-project" viewBox="0 0 15 16" version="1.1" width="15" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M10 12h3V2h-3v10zm-4-2h3V2H6v8zm-4 4h3V2H2v12zm-1 1h13V1H1v14zM14 0H1a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h13a1 1 0 0 0 1-1V1a1 1 0 0 0-1-1z"/></svg>
      Projects
      <span class="Counter" >0</span>
</a>
    <a class="js-selected-navigation-item reponav-item" data-hotkey="g w" data-selected-links="repo_wiki /cloudmobi/CloudmobiSSP/wiki" href="/cloudmobi/CloudmobiSSP/wiki">
      <svg class="octicon octicon-book" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M3 5h4v1H3V5zm0 3h4V7H3v1zm0 2h4V9H3v1zm11-5h-4v1h4V5zm0 2h-4v1h4V7zm0 2h-4v1h4V9zm2-6v9c0 .55-.45 1-1 1H9.5l-1 1-1-1H2c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h5.5l1 1 1-1H15c.55 0 1 .45 1 1zm-8 .5L7.5 3H2v9h6V3.5zm7-.5H9.5l-.5.5V12h6V3z"/></svg>
      Wiki
</a>

  <a class="js-selected-navigation-item reponav-item" data-selected-links="repo_graphs repo_contributors dependency_graph pulse /cloudmobi/CloudmobiSSP/pulse" href="/cloudmobi/CloudmobiSSP/pulse">
    <svg class="octicon octicon-graph" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M16 14v1H0V0h1v14h15zM5 13H3V8h2v5zm4 0H7V3h2v10zm4 0h-2V6h2v7z"/></svg>
    Insights
</a>

</nav>


  </div>

<div class="container new-discussion-timeline experiment-repo-nav  ">
  <div class="repository-content ">

    
  <a class="d-none js-permalink-shortcut" data-hotkey="y" href="/cloudmobi/CloudmobiSSP/blob/39c024d747e941115149c387daa73ac603b599ba/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md">Permalink</a>

  <!-- blob contrib key: blob_contributors:v21:87178b2cd4923c78dcf3d348383ec0fc -->

  <div class="file-navigation">
    
<div class="select-menu branch-select-menu js-menu-container js-select-menu float-left">
  <button class=" btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    
    type="button" aria-label="Switch branches or tags" aria-expanded="false" aria-haspopup="true">
      <i>Branch:</i>
      <span class="js-select-button css-truncate-target">master</span>
  </button>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax>

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <svg class="octicon octicon-x js-menu-close" role="img" aria-label="Close" viewBox="0 0 12 16" version="1.1" width="12" height="16"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
        <span class="select-menu-title">Switch branches/tags</span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Find or create a branch…" id="context-commitish-filter-field" class="form-control js-filterable-field js-navigation-enable" placeholder="Find or create a branch…">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Find or create a branch…" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/cloudmobi/CloudmobiSSP/blob/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <svg class="octicon octicon-check select-menu-item-icon" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M12 5l-8 8-4-4 1.5-1.5L4 10l6.5-6.5L12 5z"/></svg>
              <span class="select-menu-item-text css-truncate-target js-select-menu-filter-text">
                master
              </span>
            </a>
        </div>

          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-create-branch select-menu-item select-menu-new-item-form js-navigation-item js-new-item-form" action="/cloudmobi/CloudmobiSSP/branches" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="708BL1td67QxAmv0KVZj7JiEpWTjDNwqUInmJB2uSGqXQunx2VbWyxMF/Y74Ogg8S6N2voaBODhlLwF5fH8z8w==" />
          <svg class="octicon octicon-git-branch select-menu-item-icon" viewBox="0 0 10 16" version="1.1" width="10" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M10 5c0-1.11-.89-2-2-2a1.993 1.993 0 0 0-1 3.72v.3c-.02.52-.23.98-.63 1.38-.4.4-.86.61-1.38.63-.83.02-1.48.16-2 .45V4.72a1.993 1.993 0 0 0-1-3.72C.88 1 0 1.89 0 3a2 2 0 0 0 1 1.72v6.56c-.59.35-1 .99-1 1.72 0 1.11.89 2 2 2 1.11 0 2-.89 2-2 0-.53-.2-1-.53-1.36.09-.06.48-.41.59-.47.25-.11.56-.17.94-.17 1.05-.05 1.95-.45 2.75-1.25S8.95 7.77 9 6.73h-.02C9.59 6.37 10 5.73 10 5zM2 1.8c.66 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2C1.35 4.2.8 3.65.8 3c0-.65.55-1.2 1.2-1.2zm0 12.41c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2zm6-8c-.66 0-1.2-.55-1.2-1.2 0-.65.55-1.2 1.2-1.2.65 0 1.2.55 1.2 1.2 0 .65-.55 1.2-1.2 1.2z"/></svg>
            <div class="select-menu-item-text">
              <span class="select-menu-item-heading">Create branch: <span class="js-new-item-name"></span></span>
              <span class="description">from ‘master’</span>
            </div>
            <input type="hidden" name="name" id="name" class="js-new-item-value">
            <input type="hidden" name="branch" id="branch" value="master">
            <input type="hidden" name="path" id="path" value="CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md">
</form>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

    <div class="BtnGroup float-right">
      <a href="/cloudmobi/CloudmobiSSP/find/master"
            class="js-pjax-capture-input btn btn-sm BtnGroup-item"
            data-pjax
            data-hotkey="t">
        Find file
      </a>
      <clipboard-copy for="blob-path" class="btn btn-sm BtnGroup-item">
        Copy path
      </clipboard-copy>
    </div>
    <div id="blob-path" class="breadcrumb">
      <span class="repo-root js-repo-root"><span class="js-path-segment"><a data-pjax="true" href="/cloudmobi/CloudmobiSSP"><span>CloudmobiSSP</span></a></span></span><span class="separator">/</span><strong class="final-path">CloudMobi-iOS_CTSDK_入门指南.md</strong>
    </div>
  </div>


  <include-fragment src="/cloudmobi/CloudmobiSSP/contributors/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md" class="commit-tease">
    <div>
      Fetching contributors&hellip;
    </div>

    <div class="commit-tease-contributors">
      <img alt="" class="loader-loading float-left" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32-EAF2F5.gif" width="16" height="16" />
      <span class="loader-error">Cannot retrieve contributors at this time</span>
    </div>
</include-fragment>


  <div class="file">
    <div class="file-header">
  <div class="file-actions">

    <div class="BtnGroup">
      <a id="raw-url" class="btn btn-sm BtnGroup-item" href="/cloudmobi/CloudmobiSSP/raw/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md">Raw</a>
        <a class="btn btn-sm js-update-url-with-hash BtnGroup-item" data-hotkey="b" href="/cloudmobi/CloudmobiSSP/blame/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md">Blame</a>
      <a rel="nofollow" class="btn btn-sm BtnGroup-item" href="/cloudmobi/CloudmobiSSP/commits/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md">History</a>
    </div>

        <a class="btn-octicon tooltipped tooltipped-nw"
           href="github-mac://openRepo/https://github.com/cloudmobi/CloudmobiSSP?branch=master&amp;filepath=CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md"
           aria-label="Open this file in GitHub Desktop"
           data-ga-click="Repository, open with desktop, type:mac">
            <svg class="octicon octicon-device-desktop" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M15 2H1c-.55 0-1 .45-1 1v9c0 .55.45 1 1 1h5.34c-.25.61-.86 1.39-2.34 2h8c-1.48-.61-2.09-1.39-2.34-2H15c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm0 9H1V3h14v8z"/></svg>
        </a>

          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form js-update-url-with-hash" action="/cloudmobi/CloudmobiSSP/edit/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="ordFtRnEIwcz/OQBiPbR1dEFL/uIM8Z0rEW9JxpObSpyhPseAWGeFrPvkPCvGCoUKH4IM4j5qo/OIA7TA2b8BQ==" />
            <button class="btn-octicon tooltipped tooltipped-nw" type="submit"
              aria-label="Edit this file" data-hotkey="e" data-disable-with>
              <svg class="octicon octicon-pencil" viewBox="0 0 14 16" version="1.1" width="14" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M0 12v3h3l8-8-3-3-8 8zm3 2H1v-2h1v1h1v1zm10.3-9.3L12 6 9 3l1.3-1.3a.996.996 0 0 1 1.41 0l1.59 1.59c.39.39.39 1.02 0 1.41z"/></svg>
            </button>
</form>
        <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form" action="/cloudmobi/CloudmobiSSP/delete/master/CloudMobi-iOS_CTSDK_%E5%85%A5%E9%97%A8%E6%8C%87%E5%8D%97.md" accept-charset="UTF-8" method="post"><input name="utf8" type="hidden" value="&#x2713;" /><input type="hidden" name="authenticity_token" value="/LhLd0TASwbl7GNUAcJ62X0UiWW5RwLDRt27z2WlTLvuIf+eJ+oRSmtCCgsh7lAu0qGPDdg+BuU3HQiADVg5rw==" />
          <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
            aria-label="Delete this file" data-disable-with>
            <svg class="octicon octicon-trashcan" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M11 2H9c0-.55-.45-1-1-1H5c-.55 0-1 .45-1 1H2c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1v9c0 .55.45 1 1 1h7c.55 0 1-.45 1-1V5c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm-1 12H3V5h1v8h1V5h1v8h1V5h1v8h1V5h1v9zm1-10H2V3h9v1z"/></svg>
          </button>
</form>  </div>

  <div class="file-info">
      <span class="file-mode" title="File mode">executable file</span>
      <span class="file-info-divider"></span>
      401 lines (329 sloc)
      <span class="file-info-divider"></span>
    18.4 KB
  </div>
</div>

    
  <div id="readme" class="readme blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="text"><h3><a id="user-content-cloudmobi---ios-ctsdk-对接指南" class="anchor" aria-hidden="true" href="#cloudmobi---ios-ctsdk-对接指南"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>CloudMobi - iOS CTSDK 对接指南</h3>
<p>按照CloudMobi SDK对接指南，将我们的 SDK 集成到您的应用程序，方便您对接！这里引用的源代码可以在我们的公共 <a href="https://github.com/cloudmobi/CloudmobiSSP/blob/master/iOS-SDK-Demo.zip">demo</a> 存储库中获得。</p>
<h5><a id="user-content-目录" class="anchor" aria-hidden="true" href="#目录"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>目录</h5>
<ul>
<li><a href="#begin">在您对接SDK之前需要注意以下几点</a></li>
<li><a href="#install">将CloudMobi SDKt添加到Xcode项目中</a></li>
<li><a href="#use">SDK广告接口及其使用</a></li>
</ul>
<h6><a id="user-content-在您对接sdk之前需要注意以下几点" class="anchor" aria-hidden="true" href="#在您对接sdk之前需要注意以下几点"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a name="user-content-begin">在您对接SDK之前需要注意以下几点</a></h6>
<ul>
<li><a href="https://github.com/cloudmobi/CloudmobiSSP/blob/master/(CT)iOS-SDK.zip">CloudMobi iOS SDK（点击下载）</a> 支持iOS7+，并支持32位和64位应用程序</li>
<li>集成需要 CloudMobi 账号，所以如果您目前还没有该账号的话，请联系我们的运营人员。</li>
</ul>
<h6><a id="user-content-将cloudmobi-ios-sdk添加到xcode项目中" class="anchor" aria-hidden="true" href="#将cloudmobi-ios-sdk添加到xcode项目中"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a name="user-content-install">将CloudMobi iOS SDK添加到Xcode项目中</a></h6>
<ol>
<li>
<p>将<a href="https://github.com/cloudmobi/CloudmobiSSP/blob/master/(CT)iOS-SDK.zip">CloudMobi iOS SDK</a>下载解压之后将 CTSDK.framework 放到 Frameworks 下的 Xcode 中。</p>
</li>
<li>
<p>添加其他的必需的框架
CloudMobi iOS SDK 需要一些其他本地框架来链接到您的项目，因此请点击您的项目，并前往：</p>
<p>General &gt; Linked Frameworks and Libraries
许多这些框架已经包括在内，因为它们是大多数 Xcode 项目的默认框架，但请务必添加以下任何尚未包含在内的框架：</p>
<ul>
<li>AdSupport.framework</li>
<li>AVFoundation.framework</li>
<li>Foundation.framework</li>
<li>StoreKit.framework</li>
<li>SystemConfiguration.framework</li>
<li>UIKit.framework</li>
<li>CTSDK.framework</li>
</ul>
<p>同时应该检查 <a href="https://github.com/cloudmobi/CloudmobiSSP/blob/master/(CT)iOS-SDK.zip">CTSDK</a> 框架是否出现在链接框架和库下面。如果先前的拖放步骤没有自动链接，我们可以通过点击 '+' 然后'添加其他'手动添加它。</p>
</li>
<li>
<p>添加 -ObjC 链接器标志
这可以通过导航到构建设置并将 -ObjC 添加到其他链接器标志，前往Build Settings-&gt;Other Link Flags 进行添加</p>
</li>
<li>
<p>应用程序传输安全 (ATS)
从 iOS 9（使用 Xcode 7 构建）开始，应用程序传输安全性需要通过 HTTPS 保护的应用程序所做的所有网络流量。来自CloudMobi iOS SDK 的流量还有一部分未支持 HTTPS。在此之前，我们建议您将 NSAllowsArbitraryLoads 值设置为 YES。</p>
<pre><code> &lt;key&gt;NSAppTransportSecurity&lt;/key&gt;
 &lt;dict&gt;
 	&lt;key&gt;NSAllowsArbitraryLoads&lt;/key&gt;
 	&lt;true/&gt;
 &lt;/dict&gt;
</code></pre>
</li>
<li>
<p>SDK的初始化
务必尽快初始化 SDK，以确保广告SDK拉取配置并预先缓存。 对于我们的 <a href="https://github.com/cloudmobi/CloudmobiSSP/blob/master/iOS-SDK-Demo.zip">demo</a>（以及我们对所有 iOS 项目的建议），我们会将初始化调用添加到主 AppDelegate 上的 didFinishLaunchingWithOptions 方法。</p>
<p>**注意：**如果您尝试导入 并且找不到它，请删除该引用并再次添加它，并选择“根据需要复制项目”选项。</p>
</li>
</ol>
<ul>
<li><strong>AppDelegate.h:</strong></li>
</ul>
<pre><code>#import &lt;CTSDK/CTSDK.h&gt;

</code></pre>
<ul>
<li><strong>AppDelegate.m : didFinishLaunchingWithOptions:</strong></li>
</ul>
<pre><code>NSString* slotid = @"你的CloudMobi账户当前App下的任意一个广告ID";
[[CTService shareManager] loadRequestGetCTSDKConfigBySlot_id:slotID];

</code></pre>
<p><strong>注意：</strong> loadRequestGetCTSDKConfigBySlot_id 方法应只调用一次，如果您的APP中有激励视频广告，<strong>请务必用激励视频广告位ID做初始化</strong>。</p>
<h6><a id="user-content-cloudmobi-ios-sdk广告接口及其使用" class="anchor" aria-hidden="true" href="#cloudmobi-ios-sdk广告接口及其使用"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a><a name="user-content-use">CloudMobi iOS SDK广告接口及其使用</a></h6>
<p>我们支持的广告类型有以下几种：</p>
<ul>
<li><a href="#native">元素广告</a></li>
<li><a href="#Appwall">应用墙</a></li>
<li><a href="#rewardvideo">激励视频</a></li>
<li><a href="#template">模板广告（包括条幅广告、插屏广告和原生模板广告）</a></li>
<li><a href="#nativevideo">原生视频广告</a></li>
<li><a href="#NewInterstitial">新插屏广告</a></li>
</ul>
<hr>
<p>**注意:**首先你应该通过CTSDK中CTService类提供的单例方法来获取单例对象。然后通过该对象请求不同的广告接口获取不同类型的广告。</p>
<hr>
<p><a name="user-content-native">获取元素(Native)广告</a></p>
<pre><code>通过CTNative接口来获取元素对象，通过该元素对象获取不同的广告元素自己拼接广告展示。

    /**
     * 获取元素广告对象,使用继承CTNativeAd广告视图定制广告展示,在显示之前添加到父视图
     * 由于GDPR，因此广告角标需要媒体手动添加touch事件，可以通过safai打开返回的choices_link_url。角标使用ADsignImage对象
     * @param slot_Id       Native元素广告SlotID
     * @param delegate      设置遵守 &lt;CTNativeAdDelegate&gt; 的代理对象
     * @param WHRate        设置获取广告元素中大图的图片比例1.9:1/1:1
     * @param isTest        是否开启Debug模式，保留参数
     * @param success       请求成功的回调接口，返回广告元素对象
     * @param failure       请求失败的回调接口，返回错误信息
     */
    -(void)getNativeADswithSlotId:(NSString *)slot_id
                     delegate:(id)delegate
          imageWidthHightRate:(CTImageWidthHightRate)WHRate
                       isTest:(BOOL)isTest
                      success:(void (^)(CTNativeAdModel *nativeModel))success
                      failure:(void (^)(NSError *error))failure;
/**
     * 获取多元素广告对象,使用继承CTNativeAd广告视图定制广告展示,在显示之前添加到父视图
     * 由于GDPR，因此广告角标需要媒体手动添加touch事件，可以通过safai打开返回的choices_link_url。角标使用ADsignImage对象
     * @param slot_Id       Native元素广告SlotID
     * @param num                要获取多少个元素对象
     * @param delegate      设置遵守 &lt;CTNativeAdDelegate&gt; 的代理对象
     * @param WHRate        设置获取广告元素中大图的图片比例1.9:1/1:1
     * @param isTest        是否开启Debug模式，保留参数
     * @param success       请求成功的回调接口，返回广告元素对象
     * @param failure       请求失败的回调接口，返回错误信息
     */
    -(void)getMultitermNativeADswithSlotId:(NSString *)slot_id
                             adNumbers:(NSInteger)num
                              delegate:(id)delegate
                   imageWidthHightRate:(CTImageWidthHightRate)WHRate
                                isTest:(BOOL)isTest
                               success:(void (^)(NSArray *nativeArr))success
                               failure:(void (^)(NSError *error))failure;
                               
    CTNativeAdDelegate 代理回调方法
    -(void)CTNativeAdDidClick:(UIView *)nativeAd;              //用户点击广告
    -(void)CTNativeAdDidIntoLandingPage:(UIView *)nativeAd;    //用户将要进入落地页
    -(void)CTNativeAdDidLeaveLandingPage:(UIView *)nativeAd;   //用户离开落地页
    -(void)CTNativeAdWillLeaveApplication:(UIView *)nativeAd;  //离开App


**示例代码如下，多广告接口以数组形式返回，数组中的对象是CTNativeAdModel**
    CTService *service = [CTService shareManager];
     [service getNativeADswithSlotId:@"260" delegate:self imageWidthHightRate:CTImageWHRateOnePointNineToOne isTest:NO success:^(CTNativeAdModel *nativeModel) {
        CTView *cview = [[CTView alloc]init]; //CTView是继承自CTNativeAd的View
        cview.adNativeModel = nativeModel;
        cview.frame = CGRectMake(30, 30, self.view.frame.size.width -60, 450);
        cview.titleLable.text = nativeModel.title;
        cview.iconImage.image = [self getImageFromURL:nativeModel.icon];
        cview.imageImage.image = [self getImageFromURL:nativeModel.image];
        cview.descLable.text = nativeModel.desc;
        [cview.button setTitle:nativeModel.button forState:UIControlStateNormal];
        cview.starLable.text = [NSString stringWithFormat:@"%f",nativeModel.star];
        cview.logoImage.image = nativeModel.ADsignImage;
        [self.view addSubview:cview];
        
    } failure:^(NSError *error) {
        NSLog(@"请求广告失败：%@",error);
    }];

</code></pre>
<p><a name="user-content-Appwall">获取应用墙</a></p>
<pre><code>    /**
     * 获取应用墙控制器
     * 首先，你应该调用preloadAppWallWithSlotID接口来获取广告数据，然后在回调成功之后调用showAppWallViewController接口获取应用墙控制器并推出展示
     * @param slot_Id       Appwall广告SlotID
     * @param customColor   如果你想自定义UI颜色，需要创建出CTCustomColor对象并赋值相应颜色
     * @param delegate      设置遵守 &lt;CTAppWallDelegate&gt; 的代理对象
     * @param isTest        是否开启Debug模式，保留参数
     * @param success       请求数据成功
     * @param failure       请求数据失败
     */
     - (void)preloadAppWallWithSlotID:(NSString *)slot_id
                customColor:(CTCustomColor *)customColor
                   delegate:(id)delegate
                     isTest:(BOOL)isTest
                    success:(void(^)())success
                    failure:(void(^)(NSError *error))failure;
                    
     - (UIViewController *)showAppWallViewController;
     
     CTAppWallDelegate 代理回调方法 
     -(void)CTAppWallDidClick:(CTElementAd *)ElementAd;             //点击广告
     -(void)CTAppWallDidIntoLandingPage:(CTElementAd *)ElementAd;   //进入落地页
     -(void)CTAppWallDidLeaveLandingPage:(CTElementAd *)ElementAd;  //离开落地页
     -(void)CTAppWallWillLeaveApplication:(CTElementAd *)ElementAd; //离开应用
     -(void)CTAppWallClosed;                                        //关闭应用墙
    

</code></pre>
<p><a name="user-content-rewardvideo">获取激励视频</a></p>
<pre><code>    /**
     * 获取激励视频
     * 首先，你需要调用loadRewardVideoWithSlotId:delegate:方法来获取RewardVideo，然后在成功的回调中通过show接口展示广告
     * @param slot_Id       RewardVideo广告SlotID
     * @param delegate      设置遵守 &lt;CTRewardVideoDelegate&gt; 的代理对象
     */
    - (void)loadRewardVideoWithSlotId:(NSString *)slot_id delegate:(id)delegate;
    /**
     展示激励视频
     @param viewController 设置用于推出激励视频的Viewcontroller
     */
    - (void)showRewardVideoWithPresentingViewController:(UIViewController *)viewController;
    /**
     展示广告之前再次检查广告是否可以播放
     */
    - (BOOL)checkRewardVideoIsReady;
    /**
    设置激励视频自定义参数
    @param customParams         自定义参数
    */
    - (void)setCustomParameters:(NSString *)customParams;
    
    CTRewardVideoDelegate 代理回调方法
    - (void)CTRewardVideoLoadSuccess;                       //激励视频请求成功
    - (void)CTRewardVideoDidStartPlaying;                   //激励视频开始播放
    - (void)CTRewardVideoDidFinishPlaying;                  //激励视频播放完成
    - (void)CTRewardVideoDidClickRewardAd;                  //激励视频点击代理
    - (void)CTRewardVideoWillLeaveApplication;              //激励视频将要离开应用
    - (void)CTRewardVideoJumpfailed;                        //激励视频点击跳转失败
    - (void)CTRewardVideoLoadingFailed:(NSError *)error;    //激励视频请求失败
    - (void)CTRewardVideoClosed;                            //关闭激励视频
    - (void)CTRewardVideoAdRewardedName:(NSString *)rewardName rewardAmount:(NSString *)rewardAmount customParams:(NSString*) customParams;//奖励回调接口

</code></pre>
<p><a name="user-content-template">获取模板广告（包括横幅广告，插屏广告和原生模板广告）</a></p>
<pre><code>/**
 获取条幅广告
 @param slot_id         Banner广告SlotID
 @param delegate        设置遵守 &lt;CTBannerDelegate&gt; 的代理对象
 @param frame           设置广告Frame
 @param isNeedBtn       是否在右上角显示关闭按钮
 @param isTest          是否开启Debug模式，保留参数
 @param success         请求成功回调接口，并返回bannerView对象
 @param failure         请求失败回调接口
 */
- (void)getBannerADswithSlotId:(NSString *)slot_id
                      delegate:(id)delegate
                         frame:(CGRect)frame
               needCloseButton:(BOOL)isNeedBtn
                        isTest:(BOOL)isTest
                       success:(void (^)(UIView *bannerView))success
                       failure:(void (^)(NSError *error))failure;
                       
CTBannerDelegate 代理回调方法
-(void)CTBannerDidClick:(CTBanner*)banner;                  //点击广告
-(void)CTBannerDidIntoLandingPage:(CTBanner*)banner;        //进入落地页
-(void)CTBannerDidLeaveLandingPage:(CTBanner*)banner;       //离开落地页
-(void)CTBannerClosed:(CTBanner*)banner;                    //关闭广告
-(void)CTBannerWillLeaveApplication:(CTBanner*)banner;      //将要离开应用
-(void)CTBannerHtml5Closed:(CTBanner*)banner;               //关闭广告
-(void)CTBannerJumpfail:(CTBanner*)banner;                  //跳转失败

/**
 获取插屏广告，并返回InterstitialView对象
 @param slot_id         Interstitial广告SlotID
 @param delegate        设置遵守 &lt;CTInterstitialDelegate&gt; 的代理对象
 @param isFull          设置是否是全屏显示
 @param isTest          是否开启Debug模式，保留参数
 @param success         请求成功回调接口，并返回InterstitialView对象
 @param failure         请求失败回调接口
 */
- (void)preloadInterstitialWithSlotId:(NSString *)slot_id
                             delegate:(id)delegate
                         isFullScreen:(BOOL)isFull
                               isTest:(BOOL)isTest
                              success:(void (^)(UIView *InterstitialView))success
                              failure:(void (^)(NSError *error))failure;
/**
 展示插屏
 */
- (BOOL)interstitialShow;
/**
 关闭插屏
 */
- (BOOL)interstitialClose;
/**
 Interstitial Screen Direction
 如果使用了interstitialShow来展示广告，你可以通过以下接口来设置横竖屏
 */
- (void)ScreenIsVerticalScreen:(BOOL)isVerticalScreen;
/**
 通过Viewcontroller的形式展示广告
 */
- (BOOL)interstitialShowWithControllerStyleFromRootViewController:(UIViewController *)rootViewController;

CTInterstitialDelegate 代理回调方法
-(void)CTInterstitialDidClick:(CTInterstitial*)interstitialAD;              //点击广告
-(void)CTInterstitialDidIntoLandingPage:(CTInterstitial*)interstitialAD;    //进入落地页
-(void)CTInterstitialDidLeaveLandingPage:(CTInterstitial*)interstitialAD;   //离开落地页
-(void)CTInterstitialClosed:(CTInterstitial*)interstitialAD;                //关闭插屏
-(void)CTInterstitialWillLeaveApplication:(CTInterstitial*)interstitialAD;  //离开应用
-(void)CTInterstitialJumpfail:(CTInterstitial*)interstitialAD;              //跳转失败

/**
 请求NATemplate广告，并返回NaTemplateView对象
 @param slot_id         NATemplate广告SlotID
 @param delegate        设置遵守 &lt;CTNaTemplateDelegate&gt; 的代理对象
 @param frame           设置广告Frame
 @param isNeedBtn       是否在右上角显示关闭按钮
 @param isTest          是否开启Debug模式，保留参数
 @param success         请求成功回调接口，并返回NaTemplateView对象
 @param failure         请求失败回调接口
 */
- (void)getNaTemplateADswithSlotId:(NSString *)slot_id
                          delegate:(id)delegate
                             frame:(CGRect)frame
                   needCloseButton:(BOOL)isNeedBtn
                            isTest:(BOOL)isTest
                           success:(void (^)(UIView *NaTemplateView))success
                           failure:(void (^)(NSError *error))failure;
                           
CTNaTemplateDelegate 代理回调方法
-(void)CTNaTemplateDidClick:(CTNaTemplate*)naTemplate;              //点击广告
-(void)CTNaTemplateDidIntoLandingPage:(CTNaTemplate*)naTemplate;    //进入落地页
-(void)CTNaTemplateDidLeaveLandingPage:(CTNaTemplate*)naTemplate;   //离开落地页
-(void)CTNaTemplateClosed:(CTNaTemplate*)naTemplate;                //关闭广告
-(void)CTNaTemplateWillLeaveApplication:(CTNaTemplate*)naTemplate;  //将要离开应用
-(void)CTNaTemplateHtml5Closed:(CTNaTemplate*)naTemplate;           //关闭模板
-(void)CTNaTemplateJumpfail:(CTNaTemplate*)naTemplate;              //跳转失败
</code></pre>
<p><a name="user-content-nativevideo">获取原生视频广告</a></p>
<pre><code>/**
 请求原生视频广告
 由于GDPR，因此广告角标需要媒体手动添加touch事件，可以通过safai打开返回的choices_link_url。角标使用ADsignImage对象
 @param slot_id         Native Video广告SlotID，否则会请求不到广告
 @param delegate        设置遵守 &lt;CTNativeVideoDelegate&gt; 的代理对象
 @param WHRate          设置获取广告元素中大图的图片比例1.9:1/1:1
 @param isTest          是否开启Debug模式，保留参数
 */
- (void)getNativeVideoADswithSlotId:(NSString*)slot_id
                           delegate:(id)delegate
                imageWidthHightRate:(CTImageWidthHightRate)WHRate
                             isTest:(BOOL)isTest;
			     
CTNativeVideoDelegate 代理回调方法
-(void)CTNativeVideoLoadSuccess:(CTNativeVideoModel *)nativeVideoModel;  //广告请求成功回调函数
-(void)CTNativeVideoLoadFailed:(NSError *)error;                         //广告请求失败回调函数
</code></pre>
<p><a name="user-content-NewInterstitial">获取插屏(New)</a></p>
<pre><code>  /**
   预加载插屏广告.
 
 参数 slot_id         广告位
 参数 delegate        广告代理对象 &lt;CTADInterstitialDelegate&gt;
 参数 isTest          是否是测试模式(填入NO即可) 
 */
- (void)preloadInterstitialAdWithSlotId:(NSString *)slot_id
                             delegate:(id)delegate
                               isTest:(BOOL)isTest;

/**
 展示差评广告,会默认在app最上层UIViewController上present出广告
 在预加载接口返回成功后调用
 */
- (void)interstitialAdShow;

/**
 展示差评广告,会在app传入的UIViewController上present出广告,如果填写nil,则与interstitialAdShow功能相同.
 在预加载接口返回成功后调用
 */
- (void)interstitialAdShowWithController:(UIViewController *)VC;

/**
检查广告是否准备好了,如果返回了YES 就可以调用广告展示接口了.返回NO则广告没有准备好
 */
- (BOOL)interstitialAdIsReady;

广告返回代理接口&lt;CTADInterstitialDelegate&gt;,需app实现

//广告获取成功
-(void)CTADInterstitialGetAdSuccess;

//广告获取失败
-(void)CTADInterstitialGetAdFailed:(NSError *)error;

//广告展示失败
- (void)CTADInterstitialAdShowFailed:(NSError *)error;

//广告被点击
-(void)CTADInterstitialDidClick;

//广告跳到落地页
- (void)CTADInterstitialDidIntoLandingPage;

//广告跳往落地页失败
- (void)CTADInterstitialJumpFailed;

//广告被关闭
-(void)CTADInterstitialClosed;

</code></pre>
</article>
  </div>

  </div>

  <button type="button" data-facebox="#jump-to-line" data-facebox-class="linejump" data-hotkey="l" class="d-none">Jump to Line</button>
  <div id="jump-to-line" style="display:none">
    <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form" action="" accept-charset="UTF-8" method="get"><input name="utf8" type="hidden" value="&#x2713;" />
      <input class="form-control linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
      <button type="submit" class="btn">Go</button>
</form>  </div>


  </div>
  <div class="modal-backdrop js-touch-events"></div>
</div>

    </div>
  </div>

  </div>

      
<div class="footer container-lg px-3" role="contentinfo">
  <div class="position-relative d-flex flex-justify-between pt-6 pb-2 mt-6 f6 text-gray border-top border-gray-light ">
    <ul class="list-style-none d-flex flex-wrap ">
      <li class="mr-3">&copy; 2018 <span title="0.34269s from unicorn-2858632128-p1s9s">GitHub</span>, Inc.</li>
        <li class="mr-3"><a data-ga-click="Footer, go to terms, text:terms" href="https://github.com/site/terms">Terms</a></li>
        <li class="mr-3"><a data-ga-click="Footer, go to privacy, text:privacy" href="https://github.com/site/privacy">Privacy</a></li>
        <li class="mr-3"><a href="https://help.github.com/articles/github-security/" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li class="mr-3"><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
        <li><a data-ga-click="Footer, go to help, text:help" href="https://help.github.com">Help</a></li>
    </ul>

    <a aria-label="Homepage" title="GitHub" class="footer-octicon" href="https://github.com">
      <svg height="24" class="octicon octicon-mark-github" viewBox="0 0 16 16" version="1.1" width="24" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
</a>
   <ul class="list-style-none d-flex flex-wrap ">
        <li class="mr-3"><a data-ga-click="Footer, go to contact, text:contact" href="https://github.com/contact">Contact GitHub</a></li>
      <li class="mr-3"><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li class="mr-3"><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li class="mr-3"><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li class="mr-3"><a href="https://blog.github.com" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>

    </ul>
  </div>
  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 text-gray-light"></span>
  </div>
</div>



  <div id="ajax-error-message" class="ajax-error-message flash flash-error">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
    </button>
    You can’t perform that action at this time.
  </div>


    
    <script crossorigin="anonymous" integrity="sha512-X5Yz1+Qk9VsyD2X8vZkreaq36jjyMgMFXoVdiC7MDatN90E2HMy8SBo1Uv5+rHaLxCmF0icy+NwqIhLkci+Mvw==" type="application/javascript" src="https://assets-cdn.github.com/assets/frameworks-dca882fa8d6991b8dd62fde97105da60.js"></script>
    
    <script crossorigin="anonymous" async="async" integrity="sha512-kpxVF+qfFly5M8M2v23YqSkKSG4kyX5ogznAfp4NYEUT2xw7tljrvxsvRp6p45Qbd0CBJdbqU6+eI9Vs3w5I3A==" type="application/javascript" src="https://assets-cdn.github.com/assets/github-1722dc72485ba337f44cbc55877c7584.js"></script>
    
    
    
  <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner d-none">
    <svg class="octicon octicon-alert" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M8.893 1.5c-.183-.31-.52-.5-.887-.5s-.703.19-.886.5L.138 13.499a.98.98 0 0 0 0 1.001c.193.31.53.501.886.501h13.964c.367 0 .704-.19.877-.5a1.03 1.03 0 0 0 .01-1.002L8.893 1.5zm.133 11.497H6.987v-2.003h2.039v2.003zm0-3.004H6.987V5.987h2.039v4.006z"/></svg>
    <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
  <div class="facebox" id="facebox" style="display:none;">
  <div class="facebox-popup">
    <div class="facebox-content" role="dialog" aria-labelledby="facebox-header" aria-describedby="facebox-description">
    </div>
    <button type="button" class="facebox-close js-facebox-close" aria-label="Close modal">
      <svg class="octicon octicon-x" viewBox="0 0 12 16" version="1.1" width="12" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.48 8l3.75 3.75-1.48 1.48L6 9.48l-3.75 3.75-1.48-1.48L4.52 8 .77 4.25l1.48-1.48L6 6.52l3.75-3.75 1.48 1.48L7.48 8z"/></svg>
    </button>
  </div>
</div>

  <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box box-shadow-large" style="width:360px;">
  </div>
</div>

<div id="hovercard-aria-description" class="sr-only">
  Press h to open a hovercard with more details.
</div>


  </body>
</html>

