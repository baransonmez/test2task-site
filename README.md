# test2task Public Documentation

This directory is the complete allowlisted content for a separate public documentation repository, `baransonmez/test2task-site`. It does not contain extension source, settings exports, credentials, real captured evidence, or reviewer credentials.

## Planned Public URLs
- Home: https://baransonmez.github.io/test2task-site/
- Privacy: https://baransonmez.github.io/test2task-site/privacy.html
- Support information: https://baransonmez.github.io/test2task-site/support.html
- Public issue tracker: https://github.com/baransonmez/test2task-site/issues

These URLs must be verified after deployment. Preparing these files does not create or publish the repository.

## Publishing
1. Restore GitHub authentication and verify the intended account can create `baransonmez/test2task-site`.
2. Obtain explicit approval to publish these documentation files to a public repository. Do not change the visibility of the extension's source repository.
3. Regenerate `privacy.html` and `icon.png` from the extension workspace using `node scripts/generate-public-site.mjs`.
4. Publish only the contents of this directory to the documentation repository's `main` branch. Keep `.nojekyll` and the public issue templates.
5. Enable Issues and GitHub Pages from `main`, root (`/`). Verify that all public URLs load without authentication.
6. Configure the verified URLs in the Chrome Web Store dashboard. Never place Jira reviewer credentials in this public repository.

The extension workspace's `privacy-policy.md` is the policy source of truth. Regenerate and redeploy the public privacy page whenever that policy changes.
