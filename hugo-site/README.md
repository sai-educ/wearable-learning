# Wearable Learning - Hugo Site

This is the Hugo-based version of the Wearable Learning website, migrated from Carrd.co.

## Prerequisites

- Hugo Extended (version 0.120.0 or later)
- Install via Homebrew: `brew install hugo`

## Local Development

1. Navigate to the hugo-site directory:
   ```bash
   cd hugo-site
   ```

2. Start the Hugo development server:
   ```bash
   hugo server -D
   ```

3. Open your browser to `http://localhost:1313`

## Building for Production

To build the site for deployment:

```bash
cd hugo-site
hugo --cleanDestinationDir --minify
```

The built site will be in the `public/` directory.

## Deployment to Cloudflare Pages

### Via Cloudflare Dashboard

1. Log in to your Cloudflare account
2. Go to Pages → Create a project
3. Connect your GitHub repository
4. Configure build settings:
   - **Build command:** `hugo --minify`
   - **Build output directory:** `public`
   - **Root directory:** `hugo-site`
   - **Environment variables:** HUGO_VERSION = `0.152.2`

### Via Git push

After setting up the Cloudflare Pages project, simply push to your repository's main branch and Cloudflare will automatically build and deploy.

## Project Structure

```
hugo-site/
├── hugo.toml           # Hugo configuration
├── content/            # Content files
│   └── _index.md       # Home page content
├── layouts/            # Templates
│   ├── _default/
│   │   └── baseof.html # Base HTML template
│   ├── partials/
│   │   └── head.html   # HTML head section
│   └── index.html      # Home page template
└── static/             # Static assets (copied as-is)
    └── assets/         # CSS, JS, images, icons
```

## Features Preserved from Original Site

- ✅ All 15 sections (Home, About, Games, Design, News, Research, Teachers, Tutorials, FAQ, etc.)
- ✅ Navigation with dropdown menus
- ✅ Responsive hamburger menu for mobile
- ✅ Video embeds (YouTube)
- ✅ Image galleries with lightbox
- ✅ FAQ accordion functionality
- ✅ Back-to-top button
- ✅ Google Analytics integration
- ✅ All original CSS and JavaScript

## Maintenance

All content is contained in `layouts/index.html`. To make content updates, edit this file.

For asset updates (images, CSS, JS), place files in the `static/assets/` directory.

## Support

For questions about the Wearable Learning platform, visit [wearablelearning.org](https://wearablelearning.org) or contact the team.
