# Extension Creator's Guide

Reference repository for the [Novalon extension library](https://novalon.studio/extensions.html). This repo stays listed on the site so creators can see the expected layout — it is **not** an extension you install into Studio.

## Repo layout

```
extension-creators-guide/
├── .novalon/                  ← website listing (auto-loaded by novalon.studio)
│   ├── extension.json
│   ├── Image1.png             ← optional preview screenshots
│   ├── Image2.png
│   └── Image3.png
├── extension/                 ← your installable package (empty in this reference repo)
└── README.md
```

## How the website uses this repo

1. Novalon staff add approved GitHub repos to `extensions/registry.json` on the website, then deploy.
2. The site fetches `.novalon/extension.json` and preview images from your `main` branch on each page load.
3. Users open your listing and use **View on GitHub** to download install files from `extension/` or GitHub Releases.

## For creators preparing a real extension

1. Fork or copy this structure into your own public GitHub repository.
2. Edit `.novalon/extension.json` with your extension name, summary, overview, and install steps.
3. Add `Image1`–`Image3` previews under `.novalon/`.
4. Put your installable package in `extension/` or publish a GitHub Release.
5. Email **support@novalon.studio** with your GitHub link and a short description when ready for review.

After approval, update your listing by pushing to GitHub — no resubmission needed. To leave the library, email support to request removal.

## Manifest template

See also: [extensions/template/extension.json](https://novalon.studio/extensions/template/extension.json) on the Novalon website.
