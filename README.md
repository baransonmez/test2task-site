# test2task Public Documentation

This directory is the complete allowlisted content for a separate public documentation repository, `baransonmez/test2task-site`. It does not contain extension source, settings exports, credentials, real captured evidence, or reviewer credentials.

The homepage explains the workflow, compatibility, evidence types, and sharing controls. The support page includes setup, first-report instructions, recording guidance, and troubleshooting. Product images in `images/` show the actual built interface using fictional test data; they are copied from the Store asset captures by the site generator. The site loads no external fonts, analytics, scripts, or embedded video.

## Public URLs
- Home: https://baransonmez.github.io/test2task-site/
- Privacy: https://baransonmez.github.io/test2task-site/privacy.html
- Support information: https://baransonmez.github.io/test2task-site/support.html
- Public issue tracker: https://github.com/baransonmez/test2task-site/issues

GitHub Pages publishes this documentation from the `main` branch, root (`/`), with HTTPS enforced. The public pages and support tracker were verified on 2026-11-16. Viewing the documentation and issue tracker requires no authentication; submitting a support issue requires a GitHub account.

## Maintaining the Site
1. Regenerate `privacy.html`, `icon.png`, and `images/` from the extension workspace using `node scripts/generate-public-site.mjs` after policy or screenshot changes. Regenerate the Store screenshots first if the extension UI has changed.
2. Review changes and publish only approved documentation files to this repository's `main` branch. Keep `.nojekyll` and the public issue templates. Do not expose the extension source or private captured data.
3. Verify that Pages deployment succeeds and all public URLs still load without authentication.
4. Keep Chrome Web Store disclosures synchronized with the hosted policy and the actual extension build. Store submission is a separate publisher action.
5. Never place Jira reviewer credentials in this public repository. Supply reviewer access only through the Store dashboard's private testing instructions.

The extension workspace's `privacy-policy.md` is the policy source of truth. Regenerate and redeploy the public privacy page whenever that policy changes.
