# Changelog

All notable changes to the Horizon Air-Gap Demo package.

## [1.0.1] - 2026-10-01

### Added

- SECURITY.md - security policy.
- CHANGELOG.md - this file.
- EVIDENCE.md - raw test output evidence.

## [1.0.0] - 2026-09-27

### Added

- Initial Air-Gap capability demo.
- Offline operation (no internet required).
- Local ECDSA P-256 signing (100 transactions).
- Integrity verification (tamper_count = 0).
- TPS benchmark included in demo.

### Verified

- Full operation with network disabled.
- Data remains local; only new data transfers on reconnect.
- ~15,700 TPS in Air-Gap mode (laptop, 8 cores).
