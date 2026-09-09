# FX Option Volume signal endpoint

Public delivery repository for the MT5 EA.

Only the generated execution signal and a small health file are published here. Strategy code, DTCC parsing logic, research data, and validation remain in the private `tanaka-doctor/fx-option-volume-ea` repository.

MT5 endpoint:

`https://raw.githubusercontent.com/tanaka-doctor/fx-option-volume-signal/main/signal.json`

Health endpoint:

`https://raw.githubusercontent.com/tanaka-doctor/fx-option-volume-signal/main/health.json`

The publishing workflow is fail-safe: when signal generation is blocked, a blocked payload is published instead of silently retaining an executable stale signal.
