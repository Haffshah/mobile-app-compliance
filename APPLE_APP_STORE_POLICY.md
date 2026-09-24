# Apple App Store Compliance

**Last verified / verification date:** 2026-09-24; **Policy status:** ACTIVE, plus monitored 2027 item; **Effective / enforcement date:** see each item; **Official source / source type:** [App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/) / first-party policy
**Next review:** 2026-10-24 and before every submission

## Active controls

- App Privacy answers/privacy policy must match all first-party and SDK data collection, use, sharing and tracking. Request ATT before tracking as Apple defines it.
- Sensitive-data APIs need a clear Info.plist purpose string. Background modes require real supported purpose and correct capability/configuration.
- Required-reason APIs need accurate approved reasons in the relevant privacy manifest; since 2024-05-01 uploads missing them are not accepted. Audit app and SDK manifests/APIs. [Source](https://developer.apple.com/documentation/bundleresources/describing-use-of-required-reason-api).
- Apply App Review rules to StoreKit, deletion, login alternatives, UGC moderation/reporting/blocking, children, AI safety/claims, ads, regional requirements, metadata and review access. Regional payment/link entitlements are not global.
- Uploads require Xcode 26+ with an iOS 26+ SDK since 2026-04-28. [Source](https://developer.apple.com/news/upcoming-requirements/).

## Future / monitored requirement

| Policy | Announcement | Effective / enforcement | Status | Affected developers | Change / consequence | Preparation | Official source |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Regulated medical-device status | Apple Developer News, verified 2026-09-24 | Early 2027; exact date not published | REQUIRES MONITORING / DEADLINE APPROACHING | EEA/UK/US apps in Health & Fitness/Medical, or frequent medical/treatment references in age rating | Provide App Store Connect status/regulatory information; existing apps without it cannot submit updates after deadline. | Assess by 2026-11-30; check monthly. | [Apple Developer News](https://developer.apple.com/news/) |

No separate confirmed general Apple 2027 deadline was found in the official sources reviewed; do not infer one from historic deadlines.
