# SMURPH legal pages

This folder contains the Terms of Service and Privacy Policy pages for the SMURPH Discord bot.

## Publish with GitHub Pages

1. Create a **public** GitHub repository named `smurph-legal`.
2. Upload `index.html` (optional), `terms.html`, and `privacy.html` from this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then save.
6. Wait for GitHub Pages to publish the site.

Your URLs will normally be:

- `https://YOUR-GITHUB-USERNAME.github.io/smurph-legal/terms.html`
- `https://YOUR-GITHUB-USERNAME.github.io/smurph-legal/privacy.html`

Replace `YOUR-GITHUB-USERNAME` with your GitHub username. Open both URLs in a private/incognito window to confirm they work, then paste them into the corresponding Terms of Service URL and Privacy Policy URL fields in Discord Developer Portal.

## Important security action

The reviewed Python source contained a bot token written directly in the file. Treat that token as compromised: reset it in Discord Developer Portal (**Bot → Reset Token**) and store the replacement outside the source code (for example, in an environment variable). Never publish the Python file or database in this repository.

## Review before publishing

These pages describe the source code that was reviewed. Re-check them if you add features, hosting providers, analytics, external APIs, or other integrations. The Bot's local SQLite records have no automatic expiry in the reviewed code.
