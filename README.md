# Mobile App Compliance Knowledge Base

Reusable, evidence-based compliance gate for Flutter apps distributed through Google Play and the Apple App Store. It is an engineering workflow, not legal advice and never guarantees store approval.

**Baseline:** verified 2026-09-24. Official current policy always overrides this repository.

## What this covers

- Google Play: policies, User Data/Data safety, permissions, background work, billing, target API, Families/child safety, UGC, ads, financial/health features and SDKs.
- Apple: App Review, App Privacy, ATT/tracking, privacy manifests/required-reason APIs, permissions, background modes, StoreKit, account deletion/login, UGC, age ratings, regional requirements and SDKs.
- Flutter’s complete surface: Dart packages *and* `pubspec.yaml`, `pubspec.lock`, Android manifest/Gradle/native code, iOS `Info.plist`, `PrivacyInfo.xcprivacy`, entitlements, Pods and native code.

## AI compliance gate

### Before development

`Feature request → risk detection → Google check → Apple check → privacy → permissions → SDK → future-policy check → decision`.

Copy [FEATURE_COMPLIANCE.md](FEATURE_COMPLIANCE.md), inventory data/permissions/SDKs, and verify every material finding against [POLICY_SOURCES.md](POLICY_SOURCES.md). Choose **PASS**, **PASS WITH CONDITIONS**, **NEEDS REVIEW**, **HIGH RISK**, or **BLOCKED** before code is written.

### During implementation

Continuously inspect manifests, Info.plist purpose strings, privacy manifests/required-reason APIs, background configuration, packages/native dependencies, data flow, payments, tracking and disclosures. Re-open the feature assessment if the scope changes.

### Before release and after implementation

Run [STORE_SUBMISSION_CHECKLIST.md](STORE_SUBMISSION_CHECKLIST.md) and a post-implementation audit. Reconcile actual behavior with Play Console Data safety/data-deletion forms, App Store Connect App Privacy/age-rating/regional declarations, metadata, reviewer access and privacy policy.

## Verification and change control

Every substantive entry records **Last Verified, Verification Date, Policy Status, Effective Date, Enforcement Date, Official Source, Source Type,** and **Next Review**. Treat an expired review date, policy announcement, platform/SDK release or feature change as stale. Update affected guidance, add [POLICY_CHANGELOG.md](POLICY_CHANGELOG.md), identify feature/code/console/privacy effects, and re-run assessments.

Official Google and Apple sources are authoritative. Future announcements belong in [2027_READINESS.md](2027_READINESS.md) with explicit status/dates. Unknowns are **REQUIRES MONITORING**, not confirmed requirements.

## 2026–2027 strategy

Keep an inventory, target current toolchains early, replace broad permissions with scoped APIs, audit/upgrade SDKs before submission, and review official announcement/deadline pages monthly and before releases. [POLICY_MATRIX.md](POLICY_MATRIX.md) provides the cross-platform view; [2027_READINESS.md](2027_READINESS.md) is the execution tracker.
