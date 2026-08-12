# Britecyte preview (`copytest`)

Team preview and reusable static-site test repository. It intentionally has no
`CNAME`, so publishing this repository cannot replace the live britecyte.com
site.

## Local preview

```bash
python3 serve.py
```

Open http://127.0.0.1:8002/.

## Structure

- `assets/`, `data/`, `js/`, `css/` — live site files
- `news/` — public news pages
- `scripts/` and `content/` — news authoring tools
- `_archive/` — versioned source and retired assets; excluded from GitHub Pages deployment

Deploys to its own GitHub Pages preview through
`.github/workflows/deploy-pages.yml` on pushes to `main`.
