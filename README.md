# Incinta Fertility Center Website

This is the Hugo-based website for Incinta Fertility Center, a leading fertility clinic providing comprehensive reproductive health services.

## Features

- **Static Site Generator**: Built with Hugo for fast, secure, and scalable performance
- **Responsive Design**: Mobile-first design using the Ananke theme
- **Blog Functionality**: Regular articles on fertility, reproductive health, and patient education
- **SEO Optimized**: Built-in SEO features and meta tags
- **Multiple Deployment Options**: Ready for Netlify, GitHub Pages, or any static hosting

## Content Structure

- **Home Page**: Welcome message and overview of services
- **Services**: Comprehensive list of fertility treatments and procedures
- **About**: Information about the clinic, team, and facility
- **Blog**: Educational articles and resources
- **Contact**: Location, hours, and contact information

## Local Development

### Prerequisites

- Hugo Extended v0.132.2 or later
- Git

### Setup

1. Clone the repository:
```bash
git clone https://github.com/your-username/incinta-fertility.git
cd incinta-fertility
```

2. Initialize submodules (for the theme):
```bash
git submodule update --init --recursive
```

3. Start the development server:
```bash
hugo server --buildDrafts
```

4. Open your browser to `http://localhost:1313`

## Content Management

### Adding Blog Posts

Create a new blog post:
```bash
hugo new content blog/your-post-title.md
```

Edit the front matter and content, then set `draft: false` when ready to publish.

### Updating Pages

Main pages are located in the `content/` directory:
- `content/_index.md` - Home page
- `content/services/_index.md` - Services page
- `content/about/_index.md` - About page
- `content/contact/_index.md` - Contact page

## Configuration

The main configuration file is `hugo.toml`. Key settings include:

- **baseURL**: Set to your domain name
- **title**: Site title
- **menu**: Navigation menu structure
- **params**: Theme-specific parameters

## Deployment

### Netlify

The site includes a `netlify.toml` configuration file for easy deployment to Netlify:

1. Connect your Git repository to Netlify
2. The build settings will be automatically detected
3. Your site will be deployed on every push to the main branch

### GitHub Pages

The site includes a GitHub Actions workflow (`.github/workflows/hugo.yml`) for automatic deployment to GitHub Pages:

1. Enable GitHub Pages in your repository settings
2. Set the source to "GitHub Actions"
3. Push to the main branch to trigger deployment

### Manual Build

To build the site manually:
```bash
hugo --gc --minify
```

The built site will be in the `public/` directory.

## Theme Customization

The site uses the [Ananke theme](https://github.com/theNewDynamic/gohugo-theme-ananke). To customize:

1. Create overrides in the `layouts/` directory
2. Add custom CSS in `assets/sass/`
3. Modify theme parameters in `hugo.toml`

## Content Guidelines

- Use clear, patient-friendly language
- Include relevant meta descriptions for SEO
- Add featured images for better visual appeal
- Include internal links to related content
- Always include medical disclaimers where appropriate

## Support

For technical issues with the website, please contact the development team. For content updates and medical information, consult with the clinical team.

## License

This website content is proprietary to Incinta Fertility Center. The Hugo framework and Ananke theme are subject to their respective licenses.