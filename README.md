GA-SDK-ANDROID
==========

GameAnalytics native Android SDK.

Documentation can be found [here](https://gameanalytics.com/docs/android-sdk).

If you have any issues or feedback regarding the SDK, please contact our friendly support team [here](https://gameanalytics.com/contact).

> :information_source:
> Requirements:   
> **Android:** Ice Cream Sandwich 4.0 (API level 14) and up   
>   
> **Build size:**   
> Note that download size differ from the actual build size. The SDK build size is only around **49Kb** and the dependencies take up to **820Kb** depending if your app already uses some of the same dependencies.

Changelog
---------
<!--(CHANGELOG_TOP)-->
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
