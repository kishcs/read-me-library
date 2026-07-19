# Read Me — Open Ebook Library

A curated collection of free and open-source ebooks, organized by category,
served via jsDelivr CDN for the Read Me Android app.

## Structure
- `metadata/catalog.json` — book list and metadata
- `metadata/categories.json` — category definitions
- `covers/` — cover images by category
- `books/` — ebook files by category

## Adding a book
1. Add the file under `books/<category>/`
2. Add a cover under `covers/<category>/`
3. Add an entry to `metadata/catalog.json`, bump `catalogVersion`
4. Update `metadata/CHANGELOG.md`

## License
All books included are public domain, Creative Commons, or otherwise
open-licensed. See each book's `license` and `sourceUrl` field in
`catalog.json` for attribution. This repo's own code/structure is MIT
licensed — see LICENSE.
