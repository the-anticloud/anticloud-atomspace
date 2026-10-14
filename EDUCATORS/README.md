# Educators — ATOMSPACE

**Project:** ATOMSPACE  
**Category:** PHILOSOPHY_SEMANTICS  
**Upstream:** https://github.com/opencog/atomspace  
**Pinned commit:** `c8d633bf272b838c2132c21b7c8ddf169a18dd22`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `53eb37d1c744c2b4351c5920d558b111ae4be2a7b5900c49ad7fbec3ab8673ce`  
**Date:** October 2026

## Teaching with ATOMSPACE

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `53eb37d1c744c2b4351c5920d558b111ae4be2a7b5900c49ad7fbec3ab8673ce` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
