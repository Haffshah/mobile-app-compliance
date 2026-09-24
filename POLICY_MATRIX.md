# Mobile Policy Matrix

**Last verified / verification date:** 2026-09-24 · **Policy status:** mixed; see notes · **Official source / type:** [Google deadlines](https://support.google.com/googleplay/android-developer/table/12921780), [Apple guidelines](https://developer.apple.com/app-store/review/guidelines/) / first-party · **Next review:** 2026-10-24.

| Area | Google Play | Apple | Current status | Future deadline | Code impact | Store impact |
| --- | --- | --- | --- | --- | --- | --- |
| Location | Minimum scope/declaration | Purpose string/privacy | Active | Play 2027-01-27 for precise scope | Permission/UI | Play declaration; App Privacy |
| Background location | Core function/disclosure/video | Legitimate background mode | Active | Monitor | Background APIs | Declaration/reviewer notes |
| Contacts | Broad access restricted | Scoped use/purpose | Active | Play 2027-01-27 | Contact Picker | Play justification |
| Photos/camera/mic | Necessary/minimum | Purpose strings | Active | Monitor | Scoped APIs | Privacy declarations |
| Notifications | Non-deceptive use | Permission/purpose | Active | Monitor | Runtime flow | Metadata/privacy if data |
| Tracking | Data Safety/identifiers | ATT + App Privacy | Active | Monitor | Consent/SDKs | Both declarations |
| Payments/subscriptions | Billing; regional programs | IAP/StoreKit; regional terms | Active | Regional | Payment architecture | Console/products/terms |
| Account deletion | In-app + web path | In-app when required | Active | Monitor | Deletion workflow | Data deletion/privacy |
| Privacy | Data Safety/privacy policy | App Privacy/policy/manifests | Active | Monitor | Data controls | Console labels |
| AI / UGC | Safety/moderation | Safety/moderation | Active | Monitor | Reporting/controls | Ratings/reviewer evidence |
| Children/ads | Families/child safety | Kids/age rating | Active | Monitor | SDK/ad restrictions | Audience/rating |
| SDKs | Developer responsible | Manifest/reason APIs | Active | Monitor | Upgrade/remove SDK | Privacy disclosures |
| Background services | FGS limits | No background abuse | Active | Play 2027-01-27 | Geofence migration | Declaration/evidence |
| Target SDK/API | API 36 new/update | Xcode 26/iOS 26 SDK | Active | Monitor | Build upgrades | Upload eligibility |

This matrix is a triage view; follow each linked platform policy for scope and territorial exceptions.
