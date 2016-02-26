GA-SDK-ANDROID
==========

GameAnalytics native Android SDK.

Documentation in the [wiki](https://github.com/GameAnalytics/GA-SDK-ANDROID/wiki).

Read more about our launch of the new events (V2) [here](http://www.gameanalytics.com/update/).

> :information_source:
> Requirements:<br/>
> **Android:** Gingerbread 2.3.3 (API level 10) and up

Changelog
---------
**3.2.2**
* updated google play services libraries to 8.4.0

**3.2.1**
* moved custom id from initialize method to seperate configuration method

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