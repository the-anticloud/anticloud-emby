# Educators — EMBY

**Project:** EMBY  
**Category:** SOCIAL_MEDIA  
**Upstream:** https://github.com/MediaBrowser/Emby  
**Pinned commit:** `1d7c2ab4bfebdae31f89fdaabd3b68782ccf495a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `47261cdfbb4480f9f0695f20a3f96f5f6bdf8d36f9155f8bbc9c4da4af13ca68`  
**Date:** October 2026

## Teaching with EMBY

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `47261cdfbb4480f9f0695f20a3f96f5f6bdf8d36f9155f8bbc9c4da4af13ca68` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
