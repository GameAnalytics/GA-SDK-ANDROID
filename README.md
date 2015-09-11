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