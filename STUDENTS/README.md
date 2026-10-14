# Students — EMBY

**Project:** EMBY  
**Category:** SOCIAL_MEDIA  
**Upstream:** https://github.com/MediaBrowser/Emby  
**Pinned commit:** `1d7c2ab4bfebdae31f89fdaabd3b68782ccf495a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `47261cdfbb4480f9f0695f20a3f96f5f6bdf8d36f9155f8bbc9c4da4af13ca68`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `1d7c2ab4bfebdae31f89fdaabd3b68782ccf495a`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `47261cdfbb4480f9f0695f20a3f96f5f6bdf8d36f9155f8bbc9c4da4af13ca68`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
