<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/345bca60-25d0-4fdd-ace5-fd03f5fc6d0d

## Run Locally

**Prerequisites:**  Node.js


1. Install dependencies:
   `npm install`
2. Set the `GEMINI_API_KEY` in [.env.local](.env.local) to your Gemini API key
3. Run the app:
   `npm run dev`

## GitHub Pages

This project is deployed with GitHub Actions using
[.github/workflows/deploy.yml](.github/workflows/deploy.yml).

The custom domain is managed through `public/CNAME` so Vite includes it in the
build output. The primary domain is `91up.tw`.

If `www.91up.tw` is opened, the app
redirects back to the apex domain early in `index.html` to avoid stale `www`
custom-domain or DNS configurations showing a blank page after a repo reset.
