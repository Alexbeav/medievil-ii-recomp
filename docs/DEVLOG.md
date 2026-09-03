# MediEvil II development log

## 2026-09-03 — canonical Track 01 identity

The release audit found a merged two-track BIN identity in the prepared
source. A read-only prefix hash of the owned merged BIN produced the exact
canonical Track 01 size, MD5, SHA-1, and CRC32. The SHA-1 matched the earlier
portfolio audit.

The source now keeps the merged identity as a compatibility entry and adds the
canonical Track 01 identity. `disc_probe.json` and `catalog_identity.json` now
name `MediEvil II (USA).cue` and `MediEvil II (USA) (Track 1).bin`. No retail
data was copied.

Consulted leads:

- `_runs/knowledge/reviews/2026-09-02-public-disc-identity-audit.md`
- `https://openretro.org/game/e205ac64-81fd-42df-bc0a-0fc5d7d5006c/edit`
- `https://forums.libretro.com/t/cue-file-causing-soundtrack-problems/3889`

The web sources were used only to confirm canonical filenames. The owned
read-only hashes remain the identity evidence. No package or publication gate
has passed yet.
