GA-SDK-ANDROID
==========

GameAnalytics native Android SDK.

Documentation can be found [here](https://gameanalytics.com/docs/android-sdk).

If you have any issues or feedback regarding the SDK, please contact our friendly support team [here](https://gameanalytics.com/contact).

> :information_source:
> Requirements:   
> **Android:** Jelly Bean 4.1 (API level 16) and up   
>   
> **Build size:**   
> Note that download size differ from the actual build size. The SDK build size is only around **49Kb** and the dependencies take up to **820Kb** depending if your app already uses some of the same dependencies.

Changelog
---------
<!--(CHANGELOG_TOP)-->
**6.7.0**
* bugfix: setGAIDTracking now properly affects OAID
* added identifier type and reworked user id retrieval logic

**6.6.3**
* bugfix for GetUserId
* updated to java 11

**6.6.2**
* increased SDK target version
* health event bugfix for unreal engine builds

**6.6.1**
* removed com.google.android.gms.games dependency:removed redundant exception logs

**6.6.0**
* added checks to safely upgrade from 6.4.0 without having any impact on existing metrics
* last used SDK version will be cached

**6.5.2**
* removed WAKE_LOCK permission

**6.5.1**
* calculate app boot metric more accurately

**6.5.0**
* added optional session performance metrics collection
* added optional app boot-time metric collection

**6.4.3**
* increased resource currency limit from 20 to 50
* added external user id
* bug fixes

**6.4.2**
* fixed an important bug when generating user ids which could affect metrics

**6.4.1**
* added optional local event caching for disabled submission
* support for app open ads

**6.4.0**
* possibility to opt out of GAID tracking
* bug fixes

**6.3.4**
* new version of the health event
* better internal error tracking
* additonal validation for the impression events
* various bug fixes

**6.3.3**
* Temporary removal of FPS tracking due to rare issues observed. FPS tracking will be reintroduced in the future once the cause is identified and fixed.

**6.3.2**
* bugfix for health event error reporting

**6.3.1**
* fixed fps crash if the SDK doesn't run on the main thread (will output an error instead)

**6.3.0**
* Added health event
* Includes FPS data measurement automatically sent at the end of the session

**6.2.10**
* small changes

**6.2.9**
* small correct for event uuid field name

**6.2.8**
* changed event uuid field name

**6.2.7**
* added event uuid to events sent

**6.2.6**
* changed target sdk to be 30 instead of 31

**6.2.5**
* removed imei identifiers and other alternative identifiers from user identifier logic

**6.2.4**
* fixed impression event methods for wrapper SDKs

**6.2.3**
* added app set id to events when it is available

**6.2.2**
* added error events to be sent for invalid custom event fields used
* added optional mergeFields argument to event methods to merge with global custom fields instead of overwrite them

**6.2.1**
* fixed missing custom event fields for when trying to fix missing session end events

**6.2.0**
* added global custom event fields function to allow to add custom fields to events sent automatically by the SDK

**6.1.1**
* added missing function for impression events
* added functionality to force a new user in a/b testing without having to uninstall app first, simply use custom user id function to set a new user id which hasn't been used yet

**6.1.0**
* added custom events fields feature

**6.0.1**
* added flutter to sdk version validator

**6.0.0**
* Changed user identifier logic in preparation for Google changes to GAID. User id for a new install is now a randomised GUID. Existing installs that update SDK will continue using previous identifier logic. It is recommended to update as soon as possible to reduce impact on calculated metrics.

**5.4.4**
* prepared for google advertising identifier changes (will not use google advertising identifier when user has opted out)

**5.4.3**
* added support for max and aequus for impression events

**5.4.2**
* added helper methods for topon and hyperbid impression events

**5.4.1**
* fix for OAID logic

**5.4.0**
* added support for OAID
* renamed a lot of function names in the gameanalytics api so this might break your build

**5.3.7**
* correction in validator for client ts

**5.3.6**
* fix to validator for client ts

**5.3.5**
* updated validator for client ts

**5.3.4**
* removed memory info in crash log for automatic crash reproting

**5.3.3**
* fixed C++ wrapper

**5.3.2**
* corrected ad event annotation

**5.3.1**
* updated validator for impression events

**5.3.0**
* added ad network version as argument for impression events

**5.2.7**
* improved user identifier flow

**5.2.6**
* fixed google ad id not updating after reset id only if you totally kill the app and then restart it, now it will update after starting a new session

**5.2.5**
* removed android:allowBackup="true" from manifest file since the value by default is true anyway

**5.2.4**
* fixed progression events with scores

**5.2.3**
* added godot engine version validator

**5.2.2**
* fix instant app bug

**5.2.1**
* fix to instant app fallback

**5.2.0**
* added new impression event, see documentation for more info

**5.1.4**
* added support for instant apps

**5.1.3**
* improved event processing queue thread

**5.1.2**
* added session_num init requests

**5.1.1**
* removed gender, birth year and facebook methods

**5.1.0**
* added option to auto detect app version to use for build field

**5.0.2**
* small remote configs fix

**5.0.1**
* corrected naming of function

**5.0.0**
* Remote Config calls have been updated and the old calls have deprecated. Please see GA documentation for the new SDK calls and migration guide
* A/B testing support added
* new ad event added

**4.4.0**
* improved device identifier flow
* OPS: refactored IMEI code out into a seperate library, please check the documentation page for how to use it now (only relevant for apps using IMEI ids)
* removed dependency to google play services

**4.3.4**
* correct urls for events

**4.3.3**
* added more internal error logging

**4.3.2**
* added better internal error logging

**4.3.1**
* removed unused fabric vesion file

**4.3.0**
* added enable/disable event submission function

**4.2.0**
* added automatic error reporting

**4.1.2**
* fixed validation for business events

**4.1.1**
* fixes to c++ wrapper

**4.1.0**
* added generic c++ wrapper

**4.0.1**
* updated google play services version

**4.0.0**
* added command center functionality

**3.6.3**
* fix to collecting channel id

**3.6.2**
* added stencyl version validator

**3.6.1**
* added custom dimensions to design and error events

**3.6.0**
* fixes for session handling

**3.5.12**
* events are now prevented from being added to internal database when no session has started yet
* fixed bug which could potentially skew session length metrics

**3.5.11**
* fixed various bugs
* updated version of google play services library that the SDK is compiled against

**3.5.10**
* added 'construct' to version validator

**3.5.9**
* added 'cordova' value to version validator

**3.5.8**
* 'install' field added to session start events when called for the first time

**3.5.7**
* added 'nativescript' value to version validator

**3.5.6**
* added more general exception around http requests

**3.5.5**
* small correction to use int instead of double for session num

**3.5.4**
* small fix to IMEI request code

**3.5.3**
* fixed IMEI request code to be within a valid range (16-bits)

**3.5.2**
* added defold version validator

**3.5.1**
* stop sending events http request if there is no events to send

**3.5.0**
* changed the behaviour of using IMEI with the 'READ_PHONE_STATE' permission to guarantee precise analytics for certain regions

**3.4.18**
* updated to v10.2.1 of Google Play Services libraries

**3.4.17**
* added fallback if sdk is used without google play services libraries

**3.4.16**
* bug fix for end session when using manual session handling

**3.4.15**
* minor fix for app version validation

**3.4.14**
* session length precision improvement

**3.4.13**
* validator bug fixes

**3.4.12**
* version validator updated with gamemaker

**3.4.11**
* bug fix to google AID fallback

**3.4.10**
* added app signature and channel id (which app store was the app installed from)
* added IMEI as fallback option for identifier when Google AID and Android ID is not available on the device (requires to add optional READ_PHONE_STATE permission)

**3.4.9**
* updated to use https instead of http for sending events

**3.4.8**
* added bundle_id, app version and app build tracking

**3.4.7**
* fixed onstop crash when using manual session handling

**3.4.6**
* possible to set custom dimensions and demographics before initialising sdk

**3.4.5**
* fixed bug when using manual session handling

**3.4.4**
* allowing not to send value with design events instead of sending 0

**3.4.3**
* bug fix to design events sent without value

**3.4.2**
* changed from using com.google.android.gms:play-services-basement:9.4.0 and com.google.android.gms:play-services-ads:9.4.0 to only use com.google.android.gms:play-services-base:9.4.0 dependency

**3.4.1**
* small fix related to manual session handling

**3.4.0**
* updated google play services libraries to 9.4.0

**3.3.1**
* fixed bug for client timestamp handling and session length in certain edge cases

**3.3.0**
* manual session handling functionality added

**3.2.6**
* external storage read and write permissions are now optional

**3.2.5**
* fixed validator to allow 'cocos2d' as sdk wrapper

**3.2.4**
* fixed the AndroidManifest.xml inside the .aar file

**3.2.3**
* fixed bug related to network changes for Android API level 23 and above

**3.2.2**
* updated google play services libraries to 8.4.0

**3.2.1**
* moved custom id from initialize method to separate configuration method

**3.2.0**
* added custom user id option
* minor refactoring

**3.1.0**
* modified session end detection when using third party ads
* minor bug fixes

**3.0.1**
* fix issue for offline initialization

**3.0.0**
* new java-only implementation
* install size reduced

**2.3.1**
* android.permission.WRITE_EXTERNAL_STORAGE not needed anymore

**2.3.0**
* fixed tracking bug with ad opt out enabled

**2.2.2**
* no network connection bug fix

**2.2.1**
* fix related to connection changes

**2.2.0**
* 'Receiver not registered' bug fix

**2.1.0**
* improved code structure
* added new (optional) initialization process (see wiki documentation)
* minor bug fixes

**2.0.4**
* increased allowed character count to 64 for many parameters

**2.0.4**
* increased allowed character count to 64 for many parameters

**2.0.3**
* fix for session length

**2.0.2**
* improved session handling
* GAPlatform.initializeWithContext(Context context) is now deprecated use GAPlatform.initializeWithActivity(Activity activity) instead, see https://github.com/GameAnalytics/GA-SDK-ANDROID/wiki/Using-the-SDK for more details
* minor bug fixes

**2.0.1**
* minor bug fixes

**2.0.0**
* Android SDK for V2 api
* progression event
* validated business event
* resource event
* custom dimensions
