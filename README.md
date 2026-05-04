# fold-landing

Static landing page for [Fold](https://fold.intent-design.tech) /
[`@intent-driven/mcp-server`](https://www.npmjs.com/package/@intent-driven/mcp-server).

Hosted via GitHub Pages on the `main` branch with the custom domain
`fold.intent-design.tech` (CNAME file in repo root).

## DNS setup (one-time)

In the DNS panel for `intent-design.tech`, add a CNAME record:

| Name | Type  | Value                       | TTL  |
|------|-------|-----------------------------|------|
| fold | CNAME | dubovskiyim.github.io.      | 3600 |

Then in repo settings → Pages → Custom domain → `fold.intent-design.tech`.
Wait 1-5 min for HTTPS cert provisioning. Done.

## Updates

Plain HTML, single file, zero build step. Edit `index.html`, commit,
push — GitHub Pages serves the new version within ~30 seconds.

## Loom embed

Search the file for `LOOM_EMBED_REPLACE_ME` and replace the placeholder
`<div>` with the Loom `<iframe>` snippet (Loom → Share → Embed).

## OG-image

Place `og-image.png` (1200×630) at the repo root. The `<meta>` tags
already point to it as a relative path.
