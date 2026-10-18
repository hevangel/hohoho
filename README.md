# HoHoHo — Holy House of Horace

A fictional, satirical religious worldbuilding website devoted to gift, joy, and wonder.

Site: https://holy-house-of-horace.epicbass1.chatgpt.site (currently owner-private; requires ChatGPT sign-in).

## Preview locally

This is a buildless static site. No installation is required. With Node.js installed:

```sh
node scripts/serve.mjs
```

Open http://127.0.0.1:4173. Stop with Ctrl+C. Alternatively, serve the `dist/` directory with any static HTTP server.

## Source map

- `dist/index.html`: page shell and header branding.
- `dist/style.css`: responsive layout, icon gallery, and certificate print styles.
- `dist/app.js`: nine sections, routing, scripture and catechism search, calendar export, and certificates.
- `dist/canon.js`: the original 32 Book of Ho verses, nine Psalm verses, 21 catechism entries, creeds, oath, and blessings.
- `dist/assets/`: PNG artwork, small header icons, and SVG certificate emblems.
- `.openai/hosting.json`: the existing Sites project ID and static directory; contains no credentials.

## Check changes

```sh
node --check dist/app.js
node --check dist/canon.js
```

Preview relevant pages at desktop and mobile sizes. Check icon orientation (stocking toe points left), search, calendar, and certificate printing when touching those features.

## Version control and publishing

This repository is the user-facing source of record. Commit source and artwork together on a branch, then merge reviewed changes into `main`. Sites also keeps its own deployment source history; a GitHub push alone does **not** publish this site.

To publish an update through Sites, use the existing project ID, synchronize the reviewed source, and deploy that exact revision while preserving the current audience. Keep the site private until the owner explicitly approves public access. Never commit access tokens or repository credentials.

The initial website import captures Sites source revision `f9686987f1bd2971c0aef3685ffcc58c3f8bb464`. The GitHub repository's original commit and MIT license are preserved.

## Editorial rules

Preserve supplied scripture in its original archaic English. Clearly distinguish original canon from newly written expansions. Membership certificates are fictional souvenirs; form values remain in page memory and are not submitted or stored.

## License

See [LICENSE](LICENSE).
