# Sumit Sharma Tools — GitHub Pages package

This ZIP contains a standalone static website in `docs/` and its optional generator in `scripts/generate-docs.mjs`. Extract both folders into your GitHub repository's root. In GitHub Pages, choose Deploy from a branch → your branch → `/docs`. The site itself needs no framework runtime, build step or backend.

## Before publishing: edit these values

1. Edit `docs/config.json`: confirm `siteRoot` matches your HTTPS domain (currently `https://thesumitsharma.in`), optionally add a monitored `contactEmail`, and set `links.dehla` only once its real destination is known.
2. Review every external destination and the privacy/terms templates against actual deployed behaviour and applicable rules. Dehla Pakad stays non-clickable until configured.
3. From the repository root, run `node scripts/generate-docs.mjs` to regenerate `docs/`. Check canonical URLs, sitemap and README values before upload.
4. Verify the GitHub Pages site, mobile navigation, search/filter, all internal links, external destinations and 404 behaviour. Add a custom domain only after configuring DNS and HTTPS.

The generator reads `docs/config.json` before emitting links, page metadata and sitemap values. Edit that file, then regenerate; it is the single editable publishing configuration.

## Current project destinations

- GitHub profile: https://github.com/sumitsharmag
- MSBU study portal: https://site.thesumitsharma.in
- Private Chat App: https://chat-room-three-pied.vercel.app/
- P2P File Transfer: https://asheesh.in/
- Dehla Pakad: **unknown; intentionally unconfigured**
- Contact email: **not supplied; the public GitHub contact link is shown**

Six native app pages are honest nonfunctional starter workspaces. They do not claim to perform the described functions. No account, database, backend, live ad script or publisher ID is included.

## Advertising note

Ad slots are visibly labelled, non-clickable placeholders on content-rich pages only. They are omitted from starter app workspaces. Do not insert ad code until the publisher has obtained approval; then audit placement, consent, privacy disclosures and current platform requirements. This starter does not promise approval or earnings.

Review Google's current [AdSense Program policies](https://support.google.com/adsense/answer/48182) and [ad placement policies](https://support.google.com/adsense/answer/1346295) before adding live ads. In particular, keep ads distinct from navigation and interactive controls; accidental clicks and low-value or under-construction inventory can violate policy.

## Files

- `index.html`: searchable, filterable ten-project directory.
- `tools/<slug>/index.html`: ten project guides.
- `tools/<native-slug>/app.html`: six starter workspace shells.
- `about.html`, `contact.html`, `privacy-policy.html`, `terms.html`, `disclaimer.html`: supporting pages.
- `assets/site.css`, `assets/site.js`: small shared presentation and directory behaviour.
- `sitemap.xml`, `robots.txt`, `404.html`: GitHub Pages support.
