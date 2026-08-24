# Britecyte preview (`copytest`)

Team preview for copy that needs a look before approval. It intentionally has no
`CNAME`, so publishing this repository cannot replace the live britecyte.com
site.

**Team preview:** https://britecyte.github.io/copytest/

The homepage is the Lipoderma email template preview. White nav items are emails
Launchpad sends. Yellow nav items are unused drafts.

The previous website redesign preview is in `_archive/2026-08-24-website-preview/`.

## Local preview

```bash
python3 serve.py
```

Open http://127.0.0.1:8002/. This is only for local work. Do not use a public
tunnel. Share the GitHub Pages link above.

Deploys to GitHub Pages through `.github/workflows/deploy-pages.yml` on pushes
to `main`.
