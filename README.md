# Paul T Hanson Portfolio

A simple portfolio site starter built with Vite.

## Setup

```bash
cd /Users/paulhanson/Documents/GitHub/-portfolio-website
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

## Desktop App

This site now includes a macOS desktop wrapper and iPad-friendly install support.

```bash
npm install
npm run app      # build and launch the desktop app
npm run dist     # build installable app packages into release/
```

## iPad App Support

Open the site in Safari on your iPad and use Share → Add to Home Screen. The site is configured as a standalone PWA with an Apple touch icon and manifest.

## Deployment

This repository is configured to automatically deploy to GitHub Pages when code is pushed to `main`.

The site should be available at:

`https://paulthanson082-glitch.github.io/-portfolio-website/`

> Note: GitHub Pages may require a moment to publish after the first workflow run.

## Custom domain

This repo now includes a `CNAME` file pointing to:

`paulhanson.design`

To complete the setup:

1. Configure a `CNAME` record in your DNS provider to `paulthanson082-glitch.github.io`.
2. Confirm the custom domain in GitHub Pages settings.

## Notes

- Update `index.html` with your real projects and contact info.
- Replace the email address in the contact section.
- Make sure GitHub Pages is enabled for the `gh-pages` branch in repository settings if needed.
