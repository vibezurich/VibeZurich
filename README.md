# VibeZurich Landing Page

[![Hugo](https://img.shields.io/badge/Hugo-0.58+-blue.svg)](https://gohugo.io/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-1.4+-38B2AC.svg)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub Pages](https://img.shields.io/badge/Hosted_on-GitHub_Pages-000000.svg)](https://pages.github.com/)

A dynamic landing page for **VibeZurich**, a one-day coding event where teams build and deploy apps in just 8 hours on **29 November 2025**. Built with Hugo and Tailwind CSS for a fast, responsive experience.

🌐 **[Live Site](https://vibezurich.github.io/VibeZurich/)** | 📖 **[Repository](https://github.com/vibezurich/VibeZurich)**

## Screenshots

![Landing Page Screenshot](./static/img/main_image.svg)  
*Hero section with animated text and call-to-action.*

## Features

- **Header with Animated Text**: Engaging intro with smooth animations.
- **About Section**: Details about the VibeZurich event.
- **Features Section**: 4-step process highlighting key aspects.
- **Registration Form**: Easy sign-up for participants.
- **Privacy & Thank You Pages**: Additional static pages for compliance and confirmation.
- **Responsive Design**: Optimized for all devices using Tailwind CSS.
- **Fast Builds**: Powered by Hugo for static site generation.

## Tech Stack

- **Hugo**: Static site generator for fast builds and SEO.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **Gulp**: Task runner for CSS processing.
- **Hosted on GitHub Pages**: Free and reliable hosting.

## Installation

### Prerequisites

- [Hugo](https://gohugo.io/getting-started/installing/) (version 0.58.0 or later)
- [Node.js](https://nodejs.org/) and npm
- [Gulp](https://gulpjs.com/) (install globally: `npm install -g gulp-cli`)

### Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/vibezurich/VibeZurich.git
   cd VibeZurich
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the development server**:
   ```bash
   npm run start
   ```

4. **Open your browser** and navigate to `http://localhost:1313`.

> **Note**: For a better development experience, edit `./tailwind.config.js` to disable `purge` or comment it out to access all Tailwind classes.

## Usage

### Configuration

- **Hugo Settings**: Edit `./config.toml` for site-wide configurations like title, base URL, and parameters.
- **Tailwind Customization**: Modify `./tailwind.config.js` for theme adjustments.
- **Netlify (if deploying there)**: Configure `./netlify.toml` for build settings.

### Content Management

- **Page Content**: All content is in `./content`. Sections are in `./content/sections/`.
- **Features**: Individual feature cards are in `./content/sections/features/`.
- **Templates**: Layouts are in `./layouts`. Start with `./layouts/_default/baseof.html` to understand the structure. Partials are in `./layouts/partials/sections`.
- **Images**: Replace placeholders in `./static/img` with your assets.

### Building CSS

Rebuild CSS anytime with:
```bash
gulp css
```
This generates `./static/css/page.css`. Note: `normalize.css` is not included in this build for regular pages.

## Deployment

The site is hosted on **GitHub Pages**. To deploy:

1. **Build the site**:
   ```bash
   npm run deploy
   ```

2. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Deploy updates"
   git push origin main
   ```

GitHub Actions (see `.github/workflows/hugo.yml`) will automatically build and deploy on pushes to the main branch.

For other platforms like Netlify, use the provided `./netlify.toml` configuration.

## Contributing

We welcome contributions! To get started:

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature/your-feature`.
3. Make your changes and test locally.
4. Submit a pull request with a clear description.

Please ensure your code follows the existing style and includes any necessary tests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
