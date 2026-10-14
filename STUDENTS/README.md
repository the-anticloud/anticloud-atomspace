# Students — ATOMSPACE

**Project:** ATOMSPACE  
**Category:** PHILOSOPHY_SEMANTICS  
**Upstream:** https://github.com/opencog/atomspace  
**Pinned commit:** `c8d633bf272b838c2132c21b7c8ddf169a18dd22`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `53eb37d1c744c2b4351c5920d558b111ae4be2a7b5900c49ad7fbec3ab8673ce`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `c8d633bf272b838c2132c21b7c8ddf169a18dd22`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `53eb37d1c744c2b4351c5920d558b111ae4be2a7b5900c49ad7fbec3ab8673ce`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
