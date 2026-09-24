# Background Services Compliance

**Last verified / verification date:** 2026-09-24 · **Policy status:** ACTIVE + FUTURE REQUIREMENT · **Effective / enforcement:** Play FGS geofencing change 2027-01-27 · **Official source:** [Google deadlines](https://support.google.com/googleplay/android-developer/table/12921780), [background location](https://support.google.com/googleplay/android-developer/answer/9799150), [Apple guidelines](https://developer.apple.com/app-store/review/guidelines/) · **Source type:** first-party · **Next review:** design, implementation and release.

Treat background execution as HIGH RISK. Record task, trigger, frequency, foreground/background/terminated behavior, APIs, data, battery impact, user benefit/control, fallback, manifest/Info.plist/entitlement, declarations and reviewer evidence.

Prefer OS scheduling, event-driven work, batching and stopping work when unused. Background location requires a core, user-expected feature and Play declaration/disclosure evidence where applicable. Do not use geofencing as a foreground-service use case after 2027-01-27; migrate to Geofence API. Apple background modes must match genuine app function, never a keep-alive workaround.
