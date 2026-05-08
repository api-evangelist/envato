# Envato (envato)

Envato runs Envato Market (per-asset marketplaces like ThemeForest, CodeCanyon, AudioJungle, VideoHive, GraphicRiver, 3DOcean, PhotoDune) and Envato Elements (subscription-based unlimited stock media). The Envato API exposes Market endpoints for items, search, downloads, user accounts, and earnings; Elements has a separate affiliate API.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/apis.yml)

## Type
- **x-type:** company

## Tags
- Stock Media, Marketplace, Themes, Audio, Video, Graphics, Subscription

## Timestamps
- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## APIs

### Envato Market API
REST API for ThemeForest, CodeCanyon, AudioJungle, VideoHive, GraphicRiver, 3DOcean, and PhotoDune. Endpoints cover catalog (search, popular, new files), item detail, item downloads (for buyers), user (collections, badges, items), and author (earnings, sales). OAuth 2.0 authorization code or personal token authentication.
- **Base URL:** `https://api.envato.com`
- **Docs:** https://build.envato.com/api/

### Envato Elements Affiliate API
Affiliate-only API for Envato Elements (subscription-based stock media). Provides search and metadata for catalog discovery within affiliate properties; not a general-purpose download API.
- **Base URL:** `https://elements.envato.com/api`
- **Docs:** https://elements.envato.com/affiliates

## Common Properties
- [Website](https://envato.com/)
- [Developer Portal](https://build.envato.com/)
- [Plans](plans/envato-plans-pricing.yml) — reconciled (Market per-asset; Elements subscription)
- [RateLimits](rate-limits/envato-rate-limits.yml) — partial (per-app throttle; RPS not published)
- [FinOps](finops/envato-finops.yml) — reconciled (FOCUS-aligned)

## Maintainers
**FN:** Kin Lane

**Email:** kin@apievangelist.com
