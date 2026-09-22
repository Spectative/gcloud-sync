# gcloud sync

A small, responsive website with a home page and privacy policy. It uses plain HTML and CSS, with no installation or build step.

## Preview

Open `index.html` in your web browser. Both pages work directly from the folder.

## Make it yours

1. Replace every bracketed placeholder in `index.html` and `privacy.html`, including the introduction, website owner name, policy date, and contact details. Update the copyright year as needed.
2. Read and complete the privacy policy, especially the contact-information section. It describes the supplied static website, not a separate app or business service. Confirm your hosting provider and actual data practices, and add any disclosures required for your circumstances. It is a starting template, not a guarantee of legal compliance.
3. Remove the “Draft template” notice from `privacy.html` once the policy is complete.
4. Edit `styles.css` if you want to change colors or spacing.

The supplied website has no JavaScript, forms, analytics, cookies, browser storage, external fonts, or embedded media. If you add those features, review the privacy policy again.

## Publish on GitHub Pages

1. Create or open the GitHub repository you want to use.
2. Copy `index.html`, `privacy.html`, `styles.css`, `robots.txt`, and the included `.nojekyll` file into the root of the repository. Copy the files themselves, not the enclosing `website` folder. Commit the files to your chosen branch, usually `main`. You can also include this README.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select your branch and **/(root)**, then select **Save**.
6. Once publishing completes, GitHub will show your website address in the Pages settings. Publishing can take up to 10 minutes.

A project website typically has an address like `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`. All local links use relative paths, so they also work inside a repository subpath or with a custom domain.

GitHub Pages availability depends on your account plan and repository visibility. Do not upload secrets or private content with the website.

Official instructions: [Configuring a publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

GitHub’s hosting documentation states that visitor IP addresses are logged and stored for security: [What is GitHub Pages?](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages).

## Google OAuth branding

Use the exact app name `gcloud sync` in Google’s OAuth consent screen. This name appears in both pages’ HTML titles and headers, and in the homepage heading.

The supplied static files have no login gate, JavaScript redirect, or crawler restrictions. Both pages explicitly permit indexing. The included `robots.txt` permits crawling when served from your domain root. For a GitHub Pages project site, the domain-root `robots.txt` controls crawling, not a file under the repository subpath.

Before requesting verification, complete the app-specific purpose and data-use disclosures, and ensure the privacy policy covers the app itself. Google requires disclosures of how the app accesses, uses, stores, and shares Google user data. A website-only policy is insufficient for that purpose.

After publishing, verify the exact homepage and privacy URLs without signing in, check that each returns a successful response without an authentication redirect or challenge, and confirm the domain-root `robots.txt` and hosting configuration do not block crawlers. The local files alone cannot establish that a live deployment is public.

Set the homepage and privacy URLs in the OAuth consent screen and complete Google’s authorized-domain ownership requirements. See [Google’s brand verification requirements](https://developers.google.com/identity/verification/authentication-verification).
