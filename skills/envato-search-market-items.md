---
name: envato-search-market-items
description: Search Envato Market items, then fetch item details, license prices and similar items.
api: Envato API
operations:
  - getSearchItem
  - getCatalogItem
  - getItemPrices
  - getSearchMoreLikeThis
---
# Search Envato Market items

1. Call `getSearchItem` (`GET /v1/discovery/search/search/item`) with `term` and, optionally, `site` (for example themeforest.net), `category`, `tags`, `rating_min` or `price_min`.
2. For a chosen result, call `getCatalogItem` (`GET /v3/market/catalog/item?id=`) for full details.
3. Call `getItemPrices` (`GET /v1/market/item-prices:{item_id}.json`) to list available licenses and prices.
4. Optionally call `getSearchMoreLikeThis` with `item_id` to find similar items.

Rules: send `Authorization: Bearer <personal token>` (issued at build.envato.com). All calls are read-only GETs. On HTTP 429, back off exponentially with jitter, and cache catalog responses. This skill searches Envato Market. To search Envato Elements, use the MCP server at https://mcp.envato.com/mcp instead.
