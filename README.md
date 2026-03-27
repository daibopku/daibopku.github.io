# Bo Dai's Homepage

[![Deploy GitHub Pages](https://github.com/daibo/daibo.github.io/actions/workflows/pages.yml/badge.svg)](https://github.com/daibo/daibo.github.io/actions/workflows/pages.yml)

This is my personal academic homepage powered by [GitHub Pages](https://pages.github.com/) with [GitHub Actions](https://github.com/features/actions) for automated deployment.

🔗 **Live Site**: https://daibo.github.io

## Features

- 🚀 **GitHub Actions CI/CD** - Automated build and deployment
- 📝 **Jekyll Collections** - Easy management of projects with individual pages
- 🎨 **Modern, responsive design** - Mobile-friendly interface
- 📱 **Project showcase** - Each project has its own detailed page
- 🔗 **Social media integration** - GitHub, Twitter, LinkedIn, Google Scholar
- 📚 **Publications showcase** with DOI links
- ⚡ **Fast loading** with GitHub Pages CDN

## Project Structure

```
.
├── .github/
│   └── workflows/
│       └── pages.yml          # GitHub Actions workflow
├── _config.yml                # Jekyll configuration
├── _layouts/
│   ├── default.html           # Main layout template
│   └── project.html           # Project page layout
├── _projects/                 # Project collection (each file becomes a page)
│   ├── voe-intuitive-physics.md
│   ├── physics-simulator.md
│   └── cognitive-vision.md
├── _includes/                 # Reusable components (optional)
├── index.md                   # Homepage
├── projects.html              # Projects listing page
├── Gemfile                    # Ruby dependencies
└── README.md                  # This file
```

## Quick Start

### 1. Fork this repository

Click the "Fork" button at the top right of this repository.

### 2. Enable GitHub Pages with Actions

1. Go to your forked repository → **Settings** → **Pages**
2. Under "Source", select "GitHub Actions"
3. The workflow will automatically deploy your site

### 3. Customize your info

Edit `_config.yml`:

```yaml
title: "Your Name"
description: "Your description"
author:
  name: "Your Name"
  email: "your.email@example.com"
  github: "your-github-username"
  twitter: "your-twitter-handle"
  linkedin: "your-linkedin-username"
  google_scholar: "your-scholar-id"

# Optional: Add a profile photo
avatar: "https://your-photo-url.jpg"

# Institution info
institution: "Your Institution"
institution_url: "https://your-institution.edu"
advisor: "Your Advisor's Name"
advisor_url: "https://advisor-website.com"
```

### 4. Add your projects

Create a new Markdown file in `_projects/` folder:

```markdown
---
title: "Your Project Title"
description: "Short description of your project"
date: 2024-01-15
tags: ["Tag1", "Tag2", "Tag3"]
github: https://github.com/yourusername/project-name
demo: https://your-demo-url.com (optional)
paper: https://arxiv.org/abs/xxxx.xxxxx (optional)
image: https://your-image-url.jpg (optional)
---

## Overview

Your project description here...

## Features

- Feature 1
- Feature 2
- Feature 3

## Installation

```bash
pip install your-project
```

## Usage

```python
import your_project
# Your code example
```

## Citation

```bibtex
@article{yourname2024,
  title={Your Paper Title},
  author={Your Name},
  journal={arXiv preprint},
  year={2024}
}
```
```

The front matter (between `---`) is required and contains metadata. The content below supports full Markdown syntax including:
- Headers
- Lists
- Code blocks with syntax highlighting
- Tables
- Images
- Math equations (using LaTeX syntax)

### 5. Update publications

Edit `index.md` to update your publications list.

### 6. Push changes

```bash
git add .
git commit -m "Update site content"
git push origin main
```

GitHub Actions will automatically build and deploy your site!

## Local Development

### Prerequisites

- Ruby 3.0+ 
- Bundler

### Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io

# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve --watch

# Open http://localhost:4000
```

### With Docker

```bash
docker run --rm -it \
  --volume="$PWD:/srv/jekyll" \
  --publish 4000:4000 \
  jekyll/jekyll:latest \
  jekyll serve --watch --drafts
```

## Adding New Projects

### Method 1: Create a new file

1. Create a new `.md` file in `_projects/` folder
2. Add front matter and content
3. Commit and push

### Method 2: Use GitHub web interface

1. Go to `_projects/` folder in your repository
2. Click "Add file" → "Create new file"
3. Name it `your-project-name.md`
4. Add content using the template above
5. Commit directly to main branch

The project will automatically appear on your projects page!

## Customization

### Colors

Edit CSS variables in `_layouts/default.html`:

```css
:root {
  --primary-color: #2563eb;    /* Main accent color */
  --text-primary: #1f2937;     /* Primary text */
  --text-secondary: #6b7280;   /* Secondary text */
  --bg-primary: #ffffff;       /* Primary background */
  --bg-secondary: #f9fafb;     /* Secondary background */
}
```

### Fonts

The template uses [Inter](https://fonts.google.com/specimen/Inter) from Google Fonts. To change:

1. Update the Google Fonts link in `_layouts/default.html` and `_layouts/project.html`
2. Update the `font-family` CSS property

### Adding new sections

You can add new sections to `_config.yml` by creating new collections:

```yaml
collections:
  projects:
    output: true
    permalink: /projects/:name/
  tutorials:  # New collection
    output: true
    permalink: /tutorials/:name/
```

Then create `_tutorials/` folder and add tutorial files.

## Troubleshooting

### Build fails on GitHub Actions

Check the Actions tab for error messages. Common issues:
- Invalid YAML in front matter
- Missing required fields in `_config.yml`
- Syntax errors in HTML/CSS

### Changes not appearing

1. Check that the workflow completed successfully (Actions tab)
2. Clear browser cache
3. Wait 2-3 minutes for CDN propagation

### Local build fails

```bash
# Clean and rebuild
bundle exec jekyll clean
bundle exec jekyll serve
```

## Advanced Features

### SEO

The site uses `jekyll-seo-tag` plugin for automatic SEO optimization:
- Meta tags
- Open Graph tags
- Twitter Cards
- JSON-LD structured data

### Sitemap

Automatic sitemap generation at `/sitemap.xml` for better search engine indexing.

### RSS Feed

Automatic RSS feed at `/feed.xml` for blog posts (if you add a blog).

## Contributing

Feel free to fork this template for your own use. If you find bugs or have suggestions, please open an issue.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Built with [Jekyll](https://jekyllrb.com/)
- Deployed with [GitHub Actions](https://github.com/features/actions)
- Icons by [Font Awesome](https://fontawesome.com/)
- Fonts by [Google Fonts](https://fonts.google.com/)
