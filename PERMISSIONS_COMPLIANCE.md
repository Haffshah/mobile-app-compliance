# Permissions Compliance

## Rule

Request the minimum permission necessary for the feature.

For each permission:

PERMISSION:
PLATFORM:
FEATURE JUSTIFICATION:
WHY ALTERNATIVE API IS NOT SUFFICIENT:
USER DISCLOSURE:
WHEN REQUESTED:
DATA COLLECTED:
STORE DECLARATION:
GOOGLE POLICY:
APPLE REQUIREMENT:
RISK:

## High-risk permission checklist

- Location
- Background location
- Contacts
- SMS
- Call logs
- Camera
- Microphone
- Photos
- Bluetooth
- Notifications
- Accessibility
- VPN
- All files access
- Exact alarms
- Health data
- Motion/fitness

## Anti-patterns

Never:
- request permission at startup without a clear reason;
- request unused permissions;
- request broader access when a picker/API provides a narrower alternative;
- silently collect data after permission;
- continue collecting after the user has disabled the relevant feature unless permitted and clearly disclosed.
