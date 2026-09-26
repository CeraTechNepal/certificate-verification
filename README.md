# Cera Tech Nepal certificate verification

This static site verifies certificate IDs against `certificates.json`. The page and the registry are intended to be published from the public GitHub organization repository `CeraTechNepal/certificate-verification` using GitHub Pages. No paid hosting or custom domain is required.

## Publish

1. Sign in to GitHub CLI with `gh auth login` using an account allowed to create repositories in CeraTechNepal.
2. Create a **public** repository named `certificate-verification` under the organization and upload this folder's contents to its root (`index.html`, `certificates.json`, `.nojekyll`, and `assets/logo.png`).
3. In the repository, open **Settings → Pages** and choose **GitHub Actions** as the build and deployment source.
4. The included workflow deploys the site on each push to `main`. Wait for its first deployment to finish. The QR destination is `https://ceratechnepal.github.io/certificate-verification/?id=CTN-U56-SK26F`.
5. Open that URL in a private/incognito browser and verify the certificate details before distributing the certificate.

The QR opens the matching record directly. The organization must keep the public record aligned with certificates it has actually issued. A GitHub Pages site is static, so edits are visible in the repository history but are not a cryptographic signature.