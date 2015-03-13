#About chrome-api-vsdoc

# About chrome-api-vsdoc #

This project was designed to aid authors in the creation of Google Chrome Extensions when authoring in the Visual Studio IDE.

By referencing the chrome-api-vsdoc.js file in your extension's source code, Visual Studio can provide intellisense when programming against the Chrome APIs.

# Supported APIs #

All of the API calls listed on the [Chrome API](http://code.google.com/chrome/extensions/api_index.html) page as of December 7th, 2013 are supported.
  * chrome.alarms
  * chrome.bookmarks
  * chrome.browserAction
  * chrome.browsingData
  * chrome.commands
  * chrome.contentSettings
  * chrome.contextMenu
  * chrome.cookies
  * chrome.extension
  * chrome.debugger
  * chrome.devtools.inspectedWindow
  * chrome.devtools.network
  * chrome.devtools.panels
  * chrome.downloads
  * chrome.events
  * chrome.extension
  * chrome.fileBrowserHandler (Chrome OS only)
  * chrome.fontSettings
  * chrome.history
  * chrome.i18n
  * chrome.identity
  * chrome.idle
  * chrome.input
  * chrome.management
  * chrome.notifications
  * chrome.omniBox
  * chrome.pageAction
  * chrome.pageCapture
  * chrome.permissions
  * chrome.power
  * chrome.privacy
  * chrome.proxy
  * chrome.pushMessaging
  * chrome.runtime
  * chrome.storage
  * chrome.system.storage
  * chrome.tabCapture
  * chrome.tabs
  * chrome.topSites
  * chrome.tts
  * chrome.ttsEngine
  * chrome.types
  * chrome.webNavigation
  * chrome.webRequest
  * chrome.webstore
  * chrome.windows

# How to use #

To take advantage of this project when authoring your Chrome Extensions, take the following steps:
  * Make sure you are using Visual Studio 2008 or higher to take advantage of intellisense for JavaScript.
  * Copy the chrome-api-vsdoc.js file into your extension's source code directory.
  * Add the following reference inside any of your extension's source code files
```
///<reference path="chrome-api-vsdoc.js"/>
```

Please be aware that this file is intended to be used for intellisense only and should not be used inside _script_ tags in your project. You can safely remove the chrome-api-vsdoc.js file before publishing your extension.