## 0.11.0

 - Update a dependency to the latest release.
 - **BREAKING** **FEAT**: forward port to firebase-ios-sdk v7.3.0.
   - Due to this SDK upgrade, iOS 10 is now the minimum supported version by FlutterFire. Please update your build target version.

## 0.10.3

 - **FEAT**: bump android `com.android.tools.build` & `'com.google.gms:google-services` versions (#4269).
 - **CHORE**: publish packages.
 - **CHORE**: bump gradle wrapper to 5.6.4 (#4158).

## 0.10.2

 - **FEAT**: bump compileSdkVersion to 29 (#3975).
 - **FEAT**: bump `compileSdkVersion` to 29 in preparation for upcoming Play Store requirement.
 - **CHORE**: publish packages.
 - **CHORE**: publish packages.

## 0.10.1

 - **FEAT**: bump compileSdkVersion to 29 (#3975).
 - **FEAT**: update Firebase iOS SDK version to 6.33.0 (from 6.26.0).

## 0.10.0+2

 - Update a dependency to the latest release.

## 0.10.0+1

 - **FIX**: remove `platform` package usage (#3729).

## 0.10.0

 - Graduate package to a stable release. See pre-releases prior to this version for changelog entries.

## 0.10.0-dev.2

 - **FIX**: local dependencies in example apps (#3319).
 - **FEAT**: integrate Admob with new core (#3347).
 - **CHORE**: intellij cleanup (#3326).

## 0.10.0-dev.1

* Depend on `firebase_core` 0.5.0.
* Firebase iOS SDK versions are now locked to use the same version defined in
  `firebase_core`.
* Firebase Android SDK versions are now using the Firebase Bill of Materials (BoM)
  to specify individual SDK versions. BoM version is also sourced from
  `firebase_core`.

## 0.9.3+4

* Bump Dart version requirement.

## 0.9.3+3

* Provide a default `MobileAdTargetingInfo` for `RewardedVideoAd.load()`. `RewardedVideoAd.load()`
would inadvertently cause a crash if `MobileAdTargetingInfo` was excluded.

## 0.9.3+2

* Fixed bug related to simultaneous ad loading behavior on iOS.

## 0.9.3+1

* Modified README to reflect supporting Native Ads.

## 0.9.3

* Support Native Ads on iOS.

## 0.9.2+1

* Added note about required Google Service config files.

## 0.9.2

* Add basic Native Ads support for Android.

## 0.9.1+3

* Replace deprecated `getFlutterEngine` call on Android.

## 0.9.1+2

* Make the pedantic dev_dependency explicit.

## 0.9.1+1

* Enable custom parameters for rewarded video server-side verification callbacks.

## 0.9.1

* Support v2 embedding. This will remain compatible with the original embedding and won't require
  app migration.

## 0.9.0+10

* Remove the deprecated `author:` field from pubspec.yaml
* Migrate the plugin to the pubspec platforms manifest.
* Bump the minimum Flutter version to 1.10.0.

## 0.9.0+9

* Updated README instructions for contributing for consistency with other Flutterfire plugins.

## 0.9.0+8

* Remove AndroidX warning.

## 0.9.0+7

* Update Android gradle plugin, gradle, and Admob versions.
* Improvements to the Android implementation, fixing warnings about a possible null pointer exception.
* Fixed an issue where an advertisement could incorrectly remain displayed when transitioning to another screen.

## 0.9.0+6

* Remove duplicate example from documentation.

## 0.9.0+5

* Update documentation to reflect new repository location.

## 0.9.0+4

* Add the ability to horizontally adjust the ads banner location by specifying a pixel offset from the centre.

## 0.9.0+3

* Update google-services Android gradle plugin to 4.3.0 in documentation and examples.

## 0.9.0+2

* On Android, no longer crashes when registering the plugin if no activity is available.

## 0.9.0+1

* Add missing template type parameter to `invokeMethod` calls.
* Bump minimum Flutter version to 1.5.0.

## 0.9.0

* Update Android dependencies to latest.

## 0.8.0+4

* Update documentation to add AdMob App ID in Info.plist
* Add iOS AdMob App ID in Info.plist in example project

## 0.8.0+3

* Log messages about automatic configuration of the default app are now less confusing.

## 0.8.0+2

* Remove categories.

## 0.8.0+1

* Log a more detailed warning at build time about the previous AndroidX
  migration.

## 0.8.0

* **Breaking change**. Migrate from the deprecated original Android Support
  Library to AndroidX. This shouldn't result in any functional changes, but it
  requires any Android apps using this plugin to [also
  migrate](https://developer.android.com/jetpack/androidx/migrate) if they're
  using the original support library.

## 0.7.0

* Mark Dart code as deprecated where the newer version AdMob deprecates features (Birthday, Gender, and Family targeting).
* Update gradle dependencies.
* Add documentation for new AndroidManifest requirements.

## 0.6.1+1

* Bump Android dependencies to latest.
* __THIS WAS AN UNINTENTIONAL BREAKING CHANGE__. Users should consume 0.6.1 instead if they need the old API, or 0.7.0 for the bumped version.
* Guide how to fix crash with admob version 17.0.0 in README

## 0.6.1

* listener on MobileAd shouldn't be final.
* Ad listeners can to be set in or out of Ad initialization.

## 0.6.0

* Add nonPersonalizedAds option to MobileAdTargetingInfo

## 0.5.7

* Bumped mockito dependency to pick up Dart 2 support.

## 0.5.6

* Bump Android and Firebase dependency versions.

## 0.5.5

* Updated Gradle tooling to match Android Studio 3.1.2.

## 0.5.4+1

* Graduate to beta.

## 0.5.4

* Fixed a bug that was causing rewarded video failure event to be called on the wrong listener.

## 0.5.3

* Updated Google Play Services dependencies to version 15.0.0.
* Added handling of rewarded video completion event.

## 0.5.2

* Simplified podspec for Cocoapods 1.5.0, avoiding link issues in app archives.

## 0.5.1

* Fixed Dart 2 type errors.

## 0.5.0

* **Breaking change**. The BannerAd constructor now requires an AdSize
  parameter. BannerAds can be created with AdSize.smartBanner, or one of
  the other predefined AdSize values. Previously BannerAds were always
  defined with the smartBanner size.

## 0.4.0

* **Breaking change**. Set SDK constraints to match the Flutter beta release.

## 0.3.2

* Fixed Dart 2 type errors.

## 0.3.1

* Enabled use in Swift projects.

## 0.3.0

* Added support for rewarded video ads.
* **Breaking change**. The properties and parameters named "unitId" in BannerAd
  and InterstitialAd have been renamed to "adUnitId" to better match AdMob's
  documentation and UI.

## 0.2.3

* Simplified and upgraded Android project template to Android SDK 27.
* Updated package description.

## 0.2.2

* Added platform-specific App IDs and ad unit IDs to example.
* Separated load and show functionality for interstitials in example.

## 0.2.1

* Use safe area layout to place ad in iOS 11

## 0.2.0

* **Breaking change**. MobileAd TargetingInfo requestAgent is now hardcoded to 'flutter-alpha'.

## 0.1.0

* **Breaking change**. Upgraded to Gradle 4.1 and Android Studio Gradle plugin
  3.0.1. Older Flutter projects need to upgrade their Gradle setup as well in
  order to use this version of the plugin. Instructions can be found
  [here](https://github.com/flutter/flutter/wiki/Updating-Flutter-projects-to-Gradle-4.1-and-Android-Studio-Gradle-plugin-3.0.1).
* Relaxed GMS dependency to [11.4.0,12.0[

## 0.0.3

* Add FLT prefix to iOS types
* Change GMS dependency to 11.4.+

## 0.0.2

* Change GMS dependency to 11.+

## 0.0.1

* Initial Release: not ready for production use
