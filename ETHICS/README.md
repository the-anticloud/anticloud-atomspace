# Ethics — ATOMSPACE

**Project:** ATOMSPACE  
**Category:** PHILOSOPHY_SEMANTICS  
**Upstream:** https://github.com/opencog/atomspace  
**Pinned commit:** `c8d633bf272b838c2132c21b7c8ddf169a18dd22`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `53eb37d1c744c2b4351c5920d558b111ae4be2a7b5900c49ad7fbec3ab8673ce`  
**Date:** October 2026

## Position

ATOMSPACE is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
