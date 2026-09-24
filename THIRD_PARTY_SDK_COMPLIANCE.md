# Third-Party SDK Compliance

**Last verified / verification date:** 2026-09-24 · **Policy status:** ACTIVE · **Effective / enforcement:** ongoing; Apple required-reason enforcement active · **Official source:** [Google SDK Index](https://play.google.com/sdks), [Apple privacy manifests](https://developer.apple.com/documentation/bundleresources/privacy_manifest_files) · **Source type:** first-party · **Next review:** each dependency change/release.

For every dependency record version, purpose, direct/transitive origin, data collection/sharing, tracking domains, permissions, native APIs, privacy manifest, required-reason APIs, Data safety/App Privacy impact, owner, official vendor documentation and verification date.

Flutter audit must inspect `pubspec.yaml`, `pubspec.lock`, `android/AndroidManifest.xml`, Gradle files, Android native code, `ios/Info.plist`, `PrivacyInfo.xcprivacy`, `Runner.entitlements`, Podfile/Podfile.lock and iOS native code. A harmless-looking Dart package can embed native SDK behavior. Update or remove unverified SDKs; do not rely on an app privacy manifest to declare SDK-owned API use.
