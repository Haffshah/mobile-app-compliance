# Google Play Compliance

**Last verified / verification date:** 2026-09-24; **Policy status:** ACTIVE, with dated future requirements below; **Effective / enforcement date:** see each item; **Official source / source type:** [Developer Program Policies](https://play.google.com/about/developer-content-policy/) / first-party policy
**Next review:** 2026-10-24 and before every Play submission

## Active controls

- Keep Data safety, privacy policy, in-app disclosures and actual first-/third-party data practices accurate and consistent. Account-creating apps need in-app deletion plus a web deletion-request resource. [User Data](https://support.google.com/googleplay/android-developer/answer/10144311).
- Request only necessary permissions and complete applicable declarations. Background location is HIGH RISK: core functionality, prominent in-app disclosure before runtime permission, declaration evidence and a reviewer video where applicable. [Guidance](https://support.google.com/googleplay/android-developer/answer/9799150).
- Classify purchases. Digital goods/services normally use the applicable Play billing path; regional alternative-billing/external-link programs are territory- and enrollment-specific. Never generalize an exception. [US update](https://support.google.com/googleplay/android-developer/answer/15582165).
- UGC needs reporting/moderation and suitable blocking; audit Families, ads, financial/health claims, identifiers and SDKs. Metadata and reviewer access must match the app.
- New apps/updates target Android 16/API 36; existing availability needs Android 15/API 35. **Enforcement:** 2026-08-31; Google notes an extension path to 2026-11-01. [Source](https://developer.android.com/google/play/requirements/target-sdk).

## Confirmed future requirements

| Policy | Announcement | Enforcement | Status | Who / required change | Consequence / prepare by |
| --- | --- | --- | --- | --- | --- |
| Contacts broad access | 2026-04-15 | 2027-01-27 | FUTURE REQUIREMENT | Use Contact Picker unless broad access is justified. | Enforcement risk; audit by 2026-11-01. |
| Precise location minimum scope | 2026-04-15 | 2027-01-27 | FUTURE REQUIREMENT | Use Location Button where applicable; fine-location declaration/justification for ongoing access. Declaration available Nov. 2026. | Enforcement risk; complete by 2026-12-15. |
| SMS / call-log verification | 2026-07-15 | 2027-01-27 | FUTURE REQUIREMENT | Remove READ_CALL_LOG phone-call verification; use Digital Credentials or SMS Retriever. | Migrate by 2026-11-30. |
| Foreground service geofencing | 2026-04-15 | 2027-01-27 | FUTURE REQUIREMENT | Geofencing is not an approved FGS use case; use Geofence API. | Change architecture by 2026-11-30. |

Canonical details: [Google Play Policy Deadlines](https://support.google.com/googleplay/android-developer/table/12921780). Monitor for later 2027 announcements.
