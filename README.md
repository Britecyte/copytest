# Britecyte preview (`copytest`)

Team preview for copy that needs a look before approval. It intentionally has no
`CNAME`, so publishing this repository cannot replace the live britecyte.com
site.

**Team preview:** https://britecyte.github.io/copytest/

The homepage is the Lipoderma email preview, synced from Launchpad’s live
mailers (same content as
`https://lipoderma-launchpad.onrender.com/copy_review/email_preview.html`).
Every nav item is an email Launchpad sends, with role-based From/To.

Interactive Launchpad screen/copy review (with submissions) lives in Launchpad
at `/copy_review/`, not in this repo.

To refresh this homepage after mailer copy changes:

```bash
# from launchpadNew
bin/rails copy_review:regenerate_email_preview
# then copy public/copy_review/email_preview.html → this repo’s index.html
# with logo paths rewritten to assets/logos/
```

The previous website redesign preview is in `_archive/2026-08-24-website-preview/`.

## Local preview

```bash
python3 serve.py
```

Open http://127.0.0.1:8002/. This is only for local work. Do not use a public
tunnel. Share the GitHub Pages link above.

Deploys to GitHub Pages through `.github/workflows/deploy-pages.yml` on pushes
to `main`.
