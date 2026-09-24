# 2027 Mobile App Compliance Readiness

**Baseline verification:** 2026-09-24 · **Next review:** 2026-10-24 and monthly thereafter. Statuses: NOT STARTED, IN PROGRESS, READY, BLOCKED, MONITORING, NOT APPLICABLE.

| Policy | Platform | Deadline | Current implementation status | Required code/configuration change | Store-console/privacy change | Owner | Priority | Verification date | Official source |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Broad contacts access | Google Play | 2027-01-27 | NOT STARTED | Replace broad access with Contact Picker or document core justification | Permission declaration; Data Safety review | Mobile lead | High | — | [Deadlines](https://support.google.com/googleplay/android-developer/table/12921780) |
| Precise location minimum scope | Google Play | 2027-01-27 | NOT STARTED | Location Button where applicable; test fine-location need | Complete declaration (available Nov. 2026); update disclosures | Mobile lead | High | — | [Location Button](https://support.google.com/googleplay/android-developer/answer/17033915) |
| Call-log verification | Google Play | 2027-01-27 | NOT STARTED | Migrate to Digital Credentials or SMS Retriever | Remove restricted-permission declaration if removed | Identity lead | High | — | [Deadlines](https://support.google.com/googleplay/android-developer/table/12921780) |
| FGS geofencing | Google Play | 2027-01-27 | NOT STARTED | Replace FGS geofencing with Geofence API | Update background evidence if applicable | Android lead | High | — | [Deadlines](https://support.google.com/googleplay/android-developer/table/12921780) |
| Medical-device status | Apple | Early 2027, exact date unknown | MONITORING | Determine scope/regulatory status | Provide App Store Connect status for in-scope EEA/UK/US app | Compliance owner | High if in scope | — | [Apple News](https://developer.apple.com/news/) |
| New general 2027 announcements | Both | Unknown | MONITORING | Monthly policy/dependency/platform review | Update declarations and changelog as required | Compliance owner | Medium | — | [Sources](POLICY_SOURCES.md) |

Before marking READY, record tested implementation, current policy source, owner sign-off, store-console completion and privacy-policy review. Do not turn MONITORING items into requirements without a primary source.
