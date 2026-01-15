# Yashovardhan Chaturvedi - Personal Website

This is my personal website and portfolio, built with [Hugo](https://gohugo.io) and hosted on GitHub Pages.

## About

This site showcases my work, resume, and blog posts.

## Technology Stack

- **Static Site Generator**: Hugo v0.154.4 (Extended)
- **Hosting**: GitHub Pages
- **Deployment**: GitHub Actions (automatic)

## Local Development

### Prerequisites

- Hugo Extended v0.154.4 or later ([installation guide](https://gohugo.io/installation/))
- Git

### Running Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/yshvrdhn/yshvrdhn.github.io.git
   cd yshvrdhn.github.io
   ```

2. Start the Hugo development server:
   ```bash
   hugo server -D
   ```

3. Open your browser to `http://localhost:1313`

### Building the Site

To build the site for production:

```bash
hugo --gc --minify
```

The generated site will be in the `public/` directory.

## Content Management

### Adding a New Blog Post

Create a new markdown file in `content/posts/`:

```bash
hugo new posts/my-new-post.md
```

Edit the file and set `draft: false` when ready to publish.

### Updating About/CV Pages

Edit the markdown files in the `content/` directory:
- `content/about.md` - About page
- `content/cv.md` - Resume/CV page

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the `main` branch.

### GitHub Pages Setup

1. Go to your repository **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. The workflow in `.github/workflows/hugo.yaml` will handle the build and deployment

### Manual Deployment

The GitHub Actions workflow can also be triggered manually:
1. Go to the **Actions** tab in your repository
2. Select the "Build and deploy" workflow
3. Click "Run workflow"

## Project Structure

```
.
├── .github/
│   └── workflows/
│       └── hugo.yaml          # GitHub Actions deployment workflow
├── content/                   # Markdown content files
│   ├── posts/                # Blog posts
│   ├── about.md              # About page
│   └── cv.md                 # CV/Resume page
├── layouts/                   # HTML templates
│   ├── _default/
│   │   ├── baseof.html       # Base template
│   │   ├── single.html       # Single page template
│   │   └── list.html         # List template
│   └── index.html            # Homepage template
├── static/                    # Static files (copied as-is)
│   └── css/
│       └── main.css          # Stylesheets
├── hugo.yaml                  # Hugo configuration
└── README.md                  # This file
```

## License

© Yashovardhan Chaturvedi. All rights reserved.

## Contact

- Email: yash.chaturvedi91@gmail.com
- GitHub: [@yshvrdhn](https://github.com/yshvrdhn)