# Wearable Learning Website

Modern, accessible website for the Wearable Learning educational platform. Built with Hugo static site generator.

## 🚀 Quick Start

### Local Development

1. Make sure you have Hugo installed:
   ```bash
   brew install hugo
   ```

2. Run the development server:
   ```bash
   hugo server -D
   ```

3. Open your browser to `http://localhost:1313`

### Building for Production

```bash
hugo --minify
```

The site will be built to the `public/` directory.

## 📦 Deployment to Cloudflare Pages

### Via Cloudflare Dashboard

1. Go to Cloudflare Pages → Create a project
2. Connect your GitHub repository
3. Use these build settings:
   - **Build command**: `hugo --minify`
   - **Build output directory**: `public`
   - **Root directory**: (leave blank - build from repository root)
   - **Environment variables**: 
     - `HUGO_VERSION` = `0.152.2`
     - `HUGO_ENV` = `production`

4. Click "Save and Deploy"

### Build Commands

Cloudflare will automatically run:
```bash
hugo --minify
```

## 🎨 Brand Colors

Official Wearable Learning brand colors:
- Primary Blue: `#005EA2`
- Secondary Orange: `#E5700D`
- Accent Teal: `#00A8A3`

## 📁 Project Structure

```
wearable-learning/
├── hugo.toml          # Hugo configuration
├── content/           # Content files
│   └── _index.md      # Home page
├── layouts/           # Templates
│   ├── _default/
│   │   └── baseof.html    # Base template
│   ├── partials/
│   │   └── head.html      # Head partial
│   └── index.html         # Home page template
└── static/            # Static assets
    └── assets/        # CSS, JS, images
```

## 🔧 Tech Stack

- **Static Site Generator**: Hugo v0.152.2
- **Fonts**: Inter, Poppins (Google Fonts)
- **Hosting**: Cloudflare Pages
- **Design**: Custom CSS with modern design system

## 📝 License

Supported by NSF Awards IIS-2041785 and IIS-2026722.

## 👥 Team

- Dr. Ivon Arroyo (UMass Amherst)
- Dr. Erin Ottmar (Worcester Polytechnic Institute)
- Dr. Gillian Smith (Worcester Polytechnic Institute)

## 📧 Contact

For questions: [ivon@cs.umass.edu](mailto:ivon@cs.umass.edu)

---

**Note**: The `hugo-site/` subdirectory is a backup and is gitignored. The Hugo site files are in the repository root for Cloudflare Pages compatibility.
