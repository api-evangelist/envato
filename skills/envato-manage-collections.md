---
name: envato-manage-collections
description: Create Envato Market collections, bookmark items into them, and list them.
api: Envato API
operations:
  - getUserCollections
  - postCollectionCreate
  - putBookmarkAdd
  - getUserCollection
  - deleteBookmarkRemove
---
# Manage collections and bookmarks

1. Call `getUserCollections` to list existing collections, and reuse one when the name matches.
2. Otherwise call `postCollectionCreate` with `name`, `public` and `site` (and an optional `description`).
3. Call `putBookmarkAdd` with `collection_id` and `item_id`.
4. Call `getUserCollection` with `id` to confirm the items in the collection. `deleteBookmarkRemove` undoes a bookmark.

Rules: `postCollectionCreate` is not idempotent, so check for an existing collection first to avoid duplicates. Confirm with the user before any POST, PUT or DELETE.
