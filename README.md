# Mobile App Compliance Knowledge Base

Purpose: reusable policy/compliance gate for Flutter, Android, and iOS projects.

This repository is designed to be used by an AI coding agent before and after feature implementation.

## Important
This is a compliance checklist and decision framework, not legal advice and not a replacement for the current official policies. Policies change. The AI agent MUST verify current official Google Play and Apple sources before making a final compliance decision.

## Core workflow

1. Understand the requested feature.
2. Identify affected policy domains.
3. Read the relevant local compliance files.
4. Verify current official Google Play and Apple rules.
5. Produce a compliance decision BEFORE implementation.
6. If conditional/high-risk, list required changes.
7. Implement only after the compliance gate passes.
8. Run a post-implementation compliance audit.
9. Re-check store metadata, declarations, privacy disclosures, permissions, SDKs, and reviewer instructions before submission.

## Decision levels

- PASS: no material policy issue identified.
- PASS WITH CONDITIONS: allowed only if listed requirements are implemented.
- NEEDS REVIEW: policy interpretation or current source verification is needed.
- HIGH RISK: likely to trigger additional review or rejection if implemented incorrectly.
- BLOCKED: do not implement/submission until the blocking issue is resolved.

## Official source directories

Google Play:
- Developer Program Policies
- Policy Announcements
- Policy Deadlines
- Policy Archive
- Data Safety / User Data
- Permissions policies
- Payments policies
- Target API requirements
- SDK requirements

Apple:
- App Review Guidelines
- App Store Connect Help
- App Privacy
- Privacy Manifest / required reason APIs
- StoreKit / payments
- Human Interface Guidelines
- Developer Program Agreement

See POLICY_SOURCES.md for the canonical URLs.
