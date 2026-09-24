# Background Services Compliance

Treat all background execution as HIGH RISK.

## Before implementation

Identify:
- exact background task;
- frequency;
- trigger;
- required data;
- user-visible purpose;
- battery impact;
- foreground/background/terminated behavior;
- platform APIs;
- fallback behavior.

## Location

For background location:
- prove it is core functionality;
- use minimum necessary accuracy/frequency;
- explain why foreground-only access is insufficient;
- verify platform policy;
- verify store declarations;
- provide user controls;
- stop tracking when the feature/session ends where appropriate.

## Battery

Prefer:
- event-driven APIs;
- significant-change/geofencing where appropriate;
- adaptive intervals;
- batching;
- OS-managed scheduling;
- stopping work when no longer needed.

Avoid:
- permanent high-frequency GPS polling;
- unnecessary foreground services;
- hidden tracking;
- aggressive wake locks;
- battery-intensive loops.

## Compliance report

BACKGROUND FEATURE:
USER BENEFIT:
TRIGGER:
FREQUENCY:
DATA:
ANDROID API:
IOS API:
BATTERY IMPACT:
USER CONTROL:
GOOGLE REQUIREMENTS:
APPLE REQUIREMENTS:
DECISION:
