# Google Play Compliance

## Source of truth

Google Play Developer Program Policies are the primary authority. This file is a structured engineering checklist and must be re-verified against the current official policy.

## High-risk domains

### User data and privacy
Verify:
- Data Safety section is accurate.
- Privacy policy is present and consistent.
- In-app disclosures are provided where required.
- Consent is obtained when required.
- Data collection/sharing by every SDK is understood.
- Permissions are necessary and proportionate.
- Data is not collected or shared deceptively.

### Permissions
Before adding any dangerous/special permission:
- establish the exact user-facing feature requiring it;
- verify the current permission-specific policy;
- verify whether a more privacy-preserving API exists;
- verify Play Console declaration requirements;
- remove unused permissions.

High-risk examples:
- Background location
- Contacts
- SMS
- Call logs
- Accessibility
- VPN
- Device administration
- All-files access
- Notification access
- Exact alarms
- Health data

### Background location
Must be treated as HIGH RISK.
Verify:
- location is core to the app's functionality;
- the use case is permitted by current policy;
- minimum necessary access is requested;
- user disclosure/consent requirements are met;
- Play Console declarations are completed;
- implementation does not track users without legitimate app functionality.

### Contacts
Check the current Contacts Permissions policy.
Prefer privacy-preserving contact picker APIs when broad contacts access is not required.

### Payments
Identify whether the transaction involves:
- digital goods/services;
- physical goods/services;
- subscriptions;
- donations;
- financial services.

Then verify the current Google Play Billing/Payments policy and any applicable regional programs.

### User-generated content
If users can upload/post/share content:
- terms/user policy;
- objectionable-content definitions;
- reporting mechanism;
- moderation;
- blocking/reporting where applicable;
- child-safety handling;
must be reviewed.

### AI-generated content
If the app generates text, images, audio, or video:
- identify restricted-content risks;
- add appropriate safety controls;
- verify current AI-generated-content requirements;
- review user reporting/feedback mechanisms where applicable.

### Children
If children are a target audience or can reasonably use the app:
- review Families Policy;
- review data collection restrictions;
- review ads/SDK restrictions;
- review child-safety requirements.

### Ads
Verify:
- ad placement is not deceptive;
- notifications are not used for prohibited ads;
- ad SDK behavior is understood;
- child-directed rules are satisfied where applicable.

### Store listing
Check:
- title;
- short/full description;
- screenshots;
- icon;
- claims;
- ratings/reviews claims;
- functionality descriptions;
- regional behavior;
- subscription/price claims.

Metadata must accurately represent the app.

### Functionality
Before submission:
- no crashes;
- no broken flows;
- no dead-end screens;
- core functionality works;
- reviewer can access the complete experience;
- app behaves consistently.

### Third-party SDKs
The developer remains responsible for third-party code.
For every SDK:
- identify data collected;
- identify data shared;
- identify permissions;
- check policy reputation/requirements;
- check SDK-specific Play requirements;
- remove unnecessary SDKs.

## Common rejection-risk categories

- deceptive behavior
- privacy/data disclosure mismatch
- excessive permissions
- unauthorized background behavior
- misleading metadata
- broken functionality
- low-quality/repetitive apps
- prohibited content
- payment violations
- unsafe UGC
- child-safety violations
- malicious or abusive SDK behavior
- review manipulation
