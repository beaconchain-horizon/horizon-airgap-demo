# Horizon Core — Air-Gap Capability Demo

**Offline blockchain infrastructure for critical industries.**

This repository demonstrates Horizon Core Air-Gap capability: full operation without internet, with cryptographic integrity preserved.

---

## Quick Start

### Linux / macOS

```bash
git clone https://github.com/beaconchain-horizon/horizon-airgap-demo.git
cd horizon-airgap-demo
./run.sh
```

### Windows

1. Download ZIP
2. Extract
3. Double-click `run.bat`

---

## What You Will See

```
============================================
  Horizon Core — Air-Gap Capability Demo
============================================

[1/6] Generating ECDSA P-256 signing key...
      OK - Key generated

[2/6] Starting server in AIR-GAP mode...
      OK - Server up on 127.0.0.1:8080

[3/6] Verifying offline operation...
      OK - System responds locally

[4/6] Signing 100 transactions locally...
      OK - Transactions signed with ECDSA P-256

[5/6] Verifying integrity (immutable ledger)...
      OK - tamper_count = 0

[6/6] Air-Gap verification:
      OK - No internet connection required
      OK - Data stays local
      OK - Only new data transfers on reconnect

============================================
  Air-Gap Capability: VERIFIED
============================================
```

---

## What This Proves

- Full blockchain operation **without internet**
- ECDSA P-256 signing **locally**
- Immutable ledger **on-premise**
- Smart sync **when reconnected**
- **Zero** data leaves isolated environment

---

## Why Air-Gap Matters

| Industry | Use Case |
|---|---|
| Banking | Regulatory data isolation |
| Oil & Gas | SCADA in remote zones |
| Power Grid | Critical infrastructure |
| Mining | Offline operations |
| Defense | Classified environments |

---

## Files

- `bin/` — compiled binaries (switch, sensortool, tpsbench)
- `config/chain.json` — chain configuration
- `run.sh` — Linux/macOS launcher
- `run.bat` — Windows launcher
- `LICENSE` — MIT

---

## No Source Code

This repository contains **only compiled binaries**. The source code is private and available under NDA for qualified partners.

---

## Contact

- **GitHub:** https://github.com/beaconchain-horizon
- **Benchmark:** https://github.com/beaconchain-horizon/horizon-benchmark

---

**© 2026 Horizon Core — MIT License**

## Note: readings_count = 0

The `readings_count` shows 0 after each run because the demo uses `:memory:` database (RAM-only). This is intentional — zero data persists after process termination, which is the core of Air-Gap security.
