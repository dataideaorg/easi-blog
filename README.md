# Easi Blog

A personal blog built with MkDocs and the Material theme.

## Features

- 📝 Clean, responsive blog design
- 🌓 Dark/light mode toggle
- 🔍 Built-in search functionality
- 🎨 Syntax highlighting for code
- 📊 Mathematical notation support (MathJax)
- 📱 Mobile-friendly responsive layout

## Development

### Prerequisites

- Python 3.13+
- Poetry for dependency management

### Getting Started

1. Install dependencies:
   ```bash
   poetry install
   ```

2. Start the development server:
   ```bash
   poetry run mkdocs serve
   ```

3. Open your browser and navigate to `http://localhost:8000`

### Building for Production

To build the static site for deployment:

```bash
poetry run mkdocs build
```

The built site will be in the `site/` directory.

## Writing Blog Posts

1. Create new markdown files in the `docs/blog/` directory
2. Update the navigation in `mkdocs.yml` to include your new posts
3. Use Markdown with all the supported extensions (admonitions, code blocks, math, etc.)

## Project Structure

```
easi-blog/
├── docs/                 # Documentation source
│   ├── blog/            # Blog posts
│   ├── stylesheets/     # Custom CSS
│   ├── javascripts/     # Custom JavaScript
│   └── includes/        # Reusable snippets
├── mkdocs.yml           # MkDocs configuration
├── pyproject.toml       # Poetry configuration
└── README.md           # This file
```

## Deployment

This blog can be deployed to any static hosting service like:
- GitHub Pages
- Netlify
- Vercel
- AWS S3

For GitHub Pages, you can use the built-in GitHub Actions workflow or the `mkdocs gh-deploy` command.