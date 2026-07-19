# Read Me — Open Ebook Library

A curated collection of free and open-source ebooks, organized by category,
served via jsDelivr CDN for the **Read Me** Android app.

## Structure

```
read-me-library/
├── metadata/
│   ├── catalog.json       # book list and metadata
│   ├── categories.json    # category definitions
│   └── CHANGELOG.md        # human-readable version history
├── covers/                 # cover images, organized by category
│   ├── self-help/
│   ├── engineering/
│   └── novels/
└── books/                  # ebook files, organized by category
    ├── self-help/
    ├── engineering/
    └── novels/
```

## Adding a book

1. Add the ebook file under `books/<category>/`
2. Add a cover image under `covers/<category>/`
3. Add an entry to `metadata/catalog.json` and bump `catalogVersion`
4. Update `metadata/CHANGELOG.md`

## Accessing files (via jsDelivr CDN)

```
https://cdn.jsdelivr.net/gh/kishcs/read-me-library@main/metadata/catalog.json
https://cdn.jsdelivr.net/gh/kishcs/read-me-library@main/books/<category>/<file>
```

## License

All books included are public domain, Creative Commons, or otherwise
open-licensed. See each book's `license` and `sourceUrl` field in
`metadata/catalog.json` for attribution details.

This repository's own structure and code (JSON schemas, scripts, etc.)
is MIT licensed — see [LICENSE](LICENSE).
