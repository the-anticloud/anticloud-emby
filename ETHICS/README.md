# Ethics — EMBY

**Project:** EMBY  
**Category:** SOCIAL_MEDIA  
**Upstream:** https://github.com/MediaBrowser/Emby  
**Pinned commit:** `1d7c2ab4bfebdae31f89fdaabd3b68782ccf495a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `47261cdfbb4480f9f0695f20a3f96f5f6bdf8d36f9155f8bbc9c4da4af13ca68`  
**Date:** October 2026

## Position

EMBY is packaged for offline deployment with a verifiable audit trail. The
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
