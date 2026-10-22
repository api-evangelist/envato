---
name: envato-verify-purchase-code
description: As an author, verify a buyer's purchase code and review sales of your items.
api: Envato API
operations:
  - getAuthorSale
  - getAuthorSales
---
# Verify a purchase code (author)

1. Call `getAuthorSale` (`GET /v3/market/author/sale?code=`) with the buyer's purchase code. A successful response returns the sale's item, license and support details. An error means the code is not a sale of your items.
2. To review sales, page through `getAuthorSales` (`GET /v3/market/author/sales?page=`). It lists unrefunded sales of your items.

Rules: use the author's own token. Sale amounts are reported before deductions, as the operation descriptions note. Both calls are read-only. Never log purchase codes in full.
