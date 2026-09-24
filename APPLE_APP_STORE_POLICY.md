# Apple App Store Compliance

## Source of truth

Apple App Review Guidelines and current Apple Developer/App Store Connect documentation are the primary authorities.

This file is an engineering checklist, not a substitute for the current guidelines.

## High-risk domains

### Privacy
Verify:
- App Privacy answers are accurate.
- Privacy policy is accessible.
- Data collected by first-party code and SDKs is understood.
- Tracking is declared correctly.
- Required permissions have appropriate purpose strings.
- Data collection is necessary and proportionate.

### Permissions
Review:
- Location
- Camera
- Microphone
- Photos
- Contacts
- Bluetooth
- Notifications
- Calendar
- Health
- Motion/fitness
- Local network

Every permission must have a legitimate feature purpose and appropriate user-facing explanation.

### Background execution
Treat background location, audio, VoIP, processing, and other background modes as HIGH RISK.

Verify:
- correct background capability;
- legitimate use case;
- correct Info.plist configuration;
- no abuse of background execution;
- battery impact is reasonable;
- behavior matches the declared functionality.

### Location
If location is collected:
- determine whether foreground or background access is truly necessary;
- request the minimum necessary access;
- provide accurate usage descriptions;
- verify App Store privacy disclosure;
- verify background mode requirements.

### Payments
Determine whether the purchase is:
- digital content;
- digital feature;
- subscription;
- physical goods;
- real-world service.

Verify the current Apple payment rules and applicable regional exceptions/programs.

### Account creation and deletion
If the app supports account creation:
- review current Apple requirements for account deletion;
- ensure deletion can be initiated in-app where required;
- ensure associated data handling is consistent with the privacy policy.

### Login
If third-party/social login is used:
- review Apple's current login-service requirements and exceptions;
- verify required privacy choices and disclosure.

### User-generated content
If users can create/share content:
- content moderation;
- reporting;
- blocking;
- contact/support;
- objectionable-content handling
must be reviewed.

### AI
If AI is a central or material feature:
- review current Apple rules applicable to the generated content;
- verify privacy implications;
- verify user safety;
- verify content moderation;
- ensure marketing claims match actual functionality.

### Subscriptions
Verify:
- correct StoreKit implementation;
- pricing disclosure;
- subscription terms;
- restore functionality;
- cancellation/manage-subscription path;
- metadata consistency.

### Store metadata
Check:
- app name;
- subtitle;
- description;
- screenshots;
- previews;
- age rating;
- privacy labels;
- subscription information;
- claims;
- reviewer notes.

Everything must accurately represent the app.

### Review access
Provide:
- demo/test account if needed;
- valid credentials;
- setup instructions;
- required environment information;
- explanations for hardware/background/location functionality;
- reviewer notes for features that cannot be tested immediately.

### Third-party SDKs
Audit:
- privacy manifests;
- required reason APIs;
- tracking;
- SDK data collection;
- SDK permissions;
- binary behavior;
- outdated/deprecated APIs.

## Common rejection-risk categories

- privacy disclosure mismatch
- excessive/unjustified permissions
- background-mode misuse
- payment violations
- account deletion problems
- login-service issues
- UGC moderation gaps
- misleading metadata
- incomplete/restricted functionality
- broken app flows
- missing reviewer access
- third-party SDK privacy issues
- required privacy manifest/reason API issues
