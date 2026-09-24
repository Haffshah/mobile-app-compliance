# Third-Party SDK Compliance

Every SDK is part of the compliance surface.

For every dependency record:

SDK:
VERSION:
PURPOSE:
DATA COLLECTED:
DATA SHARED:
PERMISSIONS:
TRACKING:
PRIVACY MANIFEST:
REQUIRED REASON APIs:
GOOGLE PLAY IMPACT:
APPLE IMPACT:
KNOWN POLICY REQUIREMENTS:
OFFICIAL DOCUMENTATION:
LAST VERIFIED:

## Flutter-specific audit

Inspect:
- pubspec.yaml
- pubspec.lock
- AndroidManifest.xml
- Info.plist
- PrivacyInfo.xcprivacy
- Gradle dependencies
- CocoaPods dependencies
- native Android code
- native iOS code

Do not assume a Flutter package is compliant because the Dart package itself appears harmless. Native dependencies may collect data or use restricted APIs.
