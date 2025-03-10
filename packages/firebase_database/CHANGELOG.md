## 5.0.0

 - Update a dependency to the latest release.
 - **BREAKING** **FEAT**: forward port to firebase-ios-sdk v7.3.0.
   - Due to this SDK upgrade, iOS 10 is now the minimum supported version by FlutterFire. Please update your build target version.

## 4.4.0

 - **FEAT**: bump android `com.android.tools.build` & `'com.google.gms:google-services` versions (#4269).
 - **CHORE**: publish packages.
 - **CHORE**: bump gradle wrapper to 5.6.4 (#4158).

## 4.3.0

 - **FEAT**: bump compileSdkVersion to 29 (#3975).
 - **FEAT**: bump `compileSdkVersion` to 29 in preparation for upcoming Play Store requirement.
 - **CHORE**: publish packages.
 - **CHORE**: publish packages.

## 4.2.0

 - **FEAT**: bump compileSdkVersion to 29 (#3975).
 - **FEAT**: update Firebase iOS SDK version to 6.33.0 (from 6.26.0).

## 4.1.1

 - Update a dependency to the latest release.

## 4.1.0

 - **FIX**: local dependencies in example apps (#3319).
 - **FEAT**: implement support for `ServerValue.increment(delta)` (#3109).
 - **CHORE**: intellij cleanup (#3326).

## 4.0.0

* Add MacOS support.
* Add MacOS example.
* Firebase iOS SDK versions are now locked to use the same version defined in
  `firebase_core`.
* Firebase Android SDK versions are now using the Firebase Bill of Materials (BoM)
  to specify individual SDK versions. BoM version is also sourced from
  `firebase_core`.
* Allow iOS & MacOS plugins to be imported as modules.

## 3.1.6

* Update lower bound of dart dependency to 2.0.0.

## 3.1.5

* Fix (#81) Android setPersistenceCacheSizeBytes crash when Long value was provided.

## 3.1.4

* Fix for missing UserAgent.h compilation failures.

## 3.1.3

* Replace deprecated `getFlutterEngine` call on Android.

## 3.1.2

* Make the pedantic dev_dependency explicit.

## 3.1.1

* Remove the deprecated `author:` field from pubspec.yaml
* Migrate the plugin to the pubspec platforms manifest.
* Bump the minimum Flutter version to 1.10.0.

## 3.1.0

* Support Android V2 embedding.
* Migrate to using the new e2e test binding.

## 3.0.9

* Updated README instructions for contributing for consistency with other Flutterfire plugins.

## 3.0.8

* Remove AndroidX warning.

## 3.0.7

* Fix possible NullPointerException when plugin is registered without a valid Activity.

## 3.0.6

* Update documentation to reflect new repository location.
* Update unit tests to call `TestWidgetsFlutterBinding.ensureInitialized`.
* Remove executable bit on LICENSE file.

## 3.0.5

* Update google-services Android gradle plugin to 4.3.0 in documentation and examples.

## 3.0.4

* Updated transactions implementation on Android for compatibility with
  newer versions of Flutter engine that require channel calls be made
  on the UI thread.

## 3.0.3

* Automatically use version from pubspec.yaml when reporting usage to Firebase.

## 3.0.2

* Add missing template type parameter to `invokeMethod` calls.
* Bump minimum Flutter version to 1.5.0.

## 3.0.1

* Suppress deprecation warning for BinaryMessages. See: https://github.com/flutter/flutter/issues/33446

## 3.0.0

* Update Android dependencies to latest.

## 2.0.3

* Provide a `toString` implementation for `DatabaseError`.

## 2.0.2+1

* Added an integration test for transactions.

## 2.0.2

* Fix the issue that `getDictionaryFromError` always returns non nil result even when the parameter is nil.

## 2.0.1+3

* Fixing DatabaseReference.set unhandled exception which happened when a successful operation was performed.

## 2.0.1+2

* Log messages about automatic configuration of the default app are now less confusing.

## 2.0.1+1

* Remove categories.

## 2.0.1

* Log a more detailed warning at build time about the previous AndroidX
  migration.

## 2.0.0

* **Breaking change**. Migrate from the deprecated original Android Support
  Library to AndroidX. This shouldn't result in any functional changes, but it
  requires any Android apps using this plugin to [also
  migrate](https://developer.android.com/jetpack/androidx/migrate) if they're
  using the original support library.

  This was originally incorrectly pushed in the `1.1.0` update.

## 1.1.0+1

* **Revert the breaking 1.1.0 update**. 1.1.0 was known to be breaking and
  should have incremented the major version number instead of the minor. This
  revert is in and of itself breaking for anyone that has already migrated
  however. Anyone who has already migrated their app to AndroidX should
  immediately update to `2.0.0` instead. That's the correctly versioned new push
  of `1.1.0`.

## 1.1.0

* **BAD**. This was a breaking change that was incorrectly published on a minor
  version upgrade, should never have happened. Reverted by 1.1.0+1.

  "**Breaking change**. Migrate from the deprecated original Android Support
  Library to AndroidX. This shouldn't result in any functional changes, but it
  requires any Android apps using this plugin to [also
  migrate](https://developer.android.com/jetpack/androidx/migrate) if they're
  using the original support library."

## 1.0.5

* Bumped Android dependencies to latest.

## 1.0.4

* Bumped test and mockito versions to pick up Dart 2 support.

## 1.0.3

* Bump Android and Firebase dependency versions.

## 1.0.2

* Add `onDisconnect` support.

## 1.0.1

* Updated Gradle tooling to match Android Studio 3.1.2.

## 1.0.0

* Bump to released version

## 0.4.6

* Allow null value for `startAt`, `endAt` and `equalTo` queries on Android.

## 0.4.5

* Updated Google Play Services dependencies to version 15.0.0.

## 0.4.4

* Updated firebase_core dependency to ^0.2.2

## 0.4.3

* Simplified podspec for Cocoapods 1.5.0, avoiding link issues in app archives.

## 0.4.2

* Updated `firebase_core` dependency.
* Removed `meta` dependency.

## 0.4.1

* Fixes Dart 2 runtime cast error.

## 0.4.0

* **Breaking change**. Set SDK constraints to match the Flutter beta release.

## 0.3.6

* Fixed Dart 2 type errors.

## 0.3.5

* Enabled use in Swift projects.

## 0.3.4

* Allow null values for Query startAt, endAt, and equalTo

## 0.3.3

* Support to specify a database by URL if required

## 0.3.2

* Fix warnings from the Dart 2.0 analyzer.
* Simplified and upgraded Android project template to Android SDK 27.
* Updated package description.

## 0.3.1

* Fix function name collision when using Firebase Database and Cloud Firestore together on iOS.

## 0.3.0

* **Breaking change**. Upgraded to Gradle 4.1 and Android Studio Gradle plugin
  3.0.1. Older Flutter projects need to upgrade their Gradle setup as well in
  order to use this version of the plugin. Instructions can be found
  [here](https://github.com/flutter/flutter/wiki/Updating-Flutter-projects-to-Gradle-4.1-and-Android-Studio-Gradle-plugin-3.0.1).

## 0.2.0

* Support for multiple databases, new dependency on firebase_core
* Relax GMS dependency to 11.+

## 0.1.4

* Add FLT prefix to iOS types
* Avoid error when clearing FirebaseSortedList

## 0.1.3

* Fix memory leak in FirebaseAnimatedList
* Change GMS dependency to 11.4.+

## 0.1.2

* Change GMS dependency to 11.+

## 0.1.1

* Add RTDB transaction support.

## 0.1.0+1

* Aligned author name with rest of repo.

## 0.1.0

* **Breaking Change**: Added current list index to the type signature of itemBuilder for FirebaseAnimatedList.

## 0.0.14

* Fix FirebaseSortedList to show data changes.

## 0.0.13

* Fixed lingering value/child listeners.

## 0.0.12

* Updated to Firebase SDK to always use latest patch version for 11.0.x builds

## 0.0.11

* Fixes startAt/endAt on iOS when used without a key

## 0.0.10

* Added workaround for inconsistent numeric types when using keepSynced on iOS
* Bug fixes to Query handling

## 0.0.9

* Updated to Firebase SDK Version 11.0.1

## 0.0.8

* Added missing offline persistence and query functionality on Android
* Fixed startAt query behavior on iOS
* Persistence methods no longer throw errors on failure, return false instead
* Updates to docs and tests

## 0.0.7

* Fixed offline persistence on iOS

## 0.0.6

* Various APIs added to FirebaseDatabase and Query
* Added removal and priority to DatabaseReference
* Improved documentation
* Added unit tests

## 0.0.5

* Fixed analyzer warnings

## 0.0.4

* Removed stub code and replaced it with support for more event types, paths, auth
* Improved example

## 0.0.3

* Updated README.md
* Bumped buildToolsVersion to 25.0.3
* Added example app

## 0.0.2

* Fix compilation error

## 0.0.1

* Initial Release
