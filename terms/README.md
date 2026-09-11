# Terms of Use hosting

The approved source is `../terms-of-use.md`. Regenerate this page offline with `node tools/legal/build-terms.cjs` from the Android project root. No JavaScript runs on the public page.

Upload `legal-site/terms/index.html` to `terms/index.html` in the existing GitHub Pages publishing directory. The page uses the existing root `style.css`; preserve that file and the root Privacy Policy `index.html` unchanged. If `style.css` is missing from the hosted repository, also upload the unchanged `legal-site/style.css` to its root.

No source Markdown, build tools, app files, credentials or private configuration are needed for hosting.

With the existing site structure, the expected path after upload is `/all-time-xi-legal/terms/`. This has not been deployed or verified. After GitHub Pages finishes publishing, open the page on mobile and desktop, check all 25 sections and its Privacy Policy link, then supply the confirmed HTTPS URL for `terms_url` in `app/src/main/res/values/release_config.xml`. That field remains empty until then.

The Privacy Policy remains at its existing root URL. No deployment is performed by these files.
