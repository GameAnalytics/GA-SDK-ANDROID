GA-SDK-ANDROID
==========

GameAnalytics native Android SDK.

Documentation in the [wiki](https://github.com/GameAnalytics/GA-SDK-ANDROID/wiki).

> :information_source:
> Requirements:<br/>
> **Android:** Ice Cream Sandwich 4.0 (API level 14) and up

Changelog
---------
<!--(CHANGELOG_TOP)-->
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
