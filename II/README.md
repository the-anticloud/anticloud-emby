# Independent Insurance — EMBY

**Project:** EMBY  
**Category:** SOCIAL_MEDIA  
**Upstream:** https://github.com/MediaBrowser/Emby  
**Pinned commit:** `1d7c2ab4bfebdae31f89fdaabd3b68782ccf495a`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `47261cdfbb4480f9f0695f20a3f96f5f6bdf8d36f9155f8bbc9c4da4af13ca68`  
**Date:** October 2026

## Why AI-specific cover matters

Deploying AI in a regulated sector creates liability surfaces that ordinary
technology cover does not reach: inference liability, audit-trail liability,
data-breach liability and IP-infringement liability.

## How this project's architecture reduces insurable risk

| Risk | Cloud AI | EMBY with AIOSS |
|---|---|---|
| Audit-trail loss | high — vendor-controlled logs | low — append-only chain, verifiable offline |
| Data breach in transit | high — data transits external servers | low — no external endpoint |
| Compliance violation | high — cannot satisfy air-gap requirements | low — structural |
| IP liability | moderate | low — pinned provenance chain |

## Evidence package for an insurer

- AIOSS chain verification for head `47261cdfbb4480f9f0695f20a3f96f5f6bdf8d36f9155f8bbc9c4da4af13ca68`
- The 16-check register with per-check evidence hashes
- Framework control mapping in `BENCH.json`

## Contact

lois@0-1.gg
