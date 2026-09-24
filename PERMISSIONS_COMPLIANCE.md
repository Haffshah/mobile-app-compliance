# Permissions Compliance

**Last verified / verification date:** 2026-09-24 · **Policy status:** ACTIVE + future Play changes · **Effective / enforcement:** see Google 2027 table · **Official source:** [Google sensitive permissions](https://support.google.com/googleplay/android-developer/answer/9888170), [Apple App Review](https://developer.apple.com/app-store/review/guidelines/) · **Source type:** first-party · **Next review:** before implementation/release.

Request the minimum permission at the moment the user invokes the feature. For each permission document: platform, feature justification, narrower alternative rejected, runtime timing/disclosure, data, console declaration, Info.plist purpose string, SDK origin, policy URL, risk and verification date.

High risk: precise/background location, contacts, SMS/call log, camera/microphone/photos, Bluetooth, notifications, accessibility, VPN, all-files access, exact alarms and health/motion. Do not request at startup, retain unused permissions, or hide collection. For Play, audit contacts, precise location, call log and FGS uses now against the confirmed 2027 requirements in [GOOGLE_PLAY_POLICY.md](GOOGLE_PLAY_POLICY.md). For Apple, validate every `NS*UsageDescription` against actual behavior.
