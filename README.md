# N-Ops Documentation

<div align="center">
    <h3>Automate your DevOps with N-Ops</h3>
    <p>Comprehensive documentation for the N-Ops project, a powerful tool designed to streamline and enhance server operations.</p>

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Docusaurus](https://img.shields.io/badge/Built%20With-Docusaurus%203-green.svg)](https://docusaurus.io/)
[![React](https://img.shields.io/badge/React-19-61DAFB.svg)](https://react.dev/)
[![Discord](https://img.shields.io/discord/YOUR_DISCORD_ID?color=7289DA&label=Discord&logo=discord&logoColor=white)](https://discord.com/invite/PYqHVUGdwv)

</div>

## 📚 Live Documentation

Visit our official documentation site: [https://n-ops.nekonik.org](https://n-ops.nekonik.org)

## 🌟 About N-Ops

This repository contains the official documentation for N-Ops, built with [Docusaurus 3](https://docusaurus.io/).

N-Ops is a comprehensive DevOps automation platform designed for modern infrastructure management, offering:

### Key Features

- **Server Management**:

  - Complete control over server resources and operations
  - Automated provisioning and deprovisioning
  - Resource scaling and optimization
  - Centralized configuration management
  - Multi-cloud and on-premises support

- **Performance Monitoring**:

  - Real-time insights into system performance
  - Customizable dashboards and visualizations
  - Proactive alerting and notification systems
  - Historical performance data analysis
  - Resource utilization tracking

- **Task Automation**:

  - Streamlined workflows for common DevOps tasks
  - CI/CD pipeline integration
  - Scheduled maintenance operations
  - Batch processing capabilities
  - Event-driven automation

- **Secure Operations**:
  - Built-in security features for safe server management
  - Role-based access control
  - Audit logging and compliance reporting
  - Encrypted communications
  - Security policy enforcement

## 🚀 Quick Start

### Prerequisites

- **Node.js** (>= 18.0) - Ensure you have Node.js installed. You can download it from [nodejs.org](https://nodejs.org/) or use a version manager like [nvm](https://github.com/nvm-sh/nvm).
- **Package Manager** - npm (comes with Node.js) or yarn (`npm install -g yarn`).
- **Git** - For cloning the repository and version control.

### Installation

```bash
# Clone the repository
git clone https://github.com/Neko-Nik-Org/N-Ops-Docs.git

# Navigate to the project directory
cd N-Ops-Docs

# Install dependencies
npm install  # or yarn install

# Verify installation
npm run clear  # This clears Docusaurus cache and verifies the installation
```

### Local Development

```bash
# Start the development server
npm start
```

This command starts a local development server and opens your browser to `http://localhost:3000`. The development server features:

- Hot module replacement for instant feedback
- Real-time preview of documentation changes
- Built-in error reporting
- Automatic reloading for most configuration changes

### Testing Your Changes

Before submitting your contributions, test them thoroughly:

```bash
# Build the documentation
npm run build

# Serve the built documentation locally
npm run serve
```

This builds the documentation in production mode and serves it locally, allowing you to verify that everything works as expected in the production environment.

## 📂 Project Structure

```
N-Ops-Docs/
├── docs/                          # Documentation content
│   ├── intro.md                   # Introduction to N-Ops
│   ├── get-started.md             # Getting started guide
│   ├── backend/                   # Backend documentation
│   │   ├── overview.md            # Backend architecture overview
│   │   ├── api-routes.md          # API endpoint documentation
│   │   ├── models.md              # Data models and schemas
│   │   ├── security.md            # Security implementation details
│   │   └── ansible.md             # Ansible integration guide
│   ├── frontend/                  # Frontend documentation
│   │   ├── overview.md            # Frontend architecture overview
│   │   ├── components.md          # UI component documentation
│   │   ├── state-auth.md          # State management and authentication
│   │   ├── websockets.md          # Websocket implementation
│   │   └── env-setup.md           # Environment setup guide
│   ├── features/                  # Feature documentation
│   │   ├── command-center.md      # Command center interface
│   │   ├── secure-notes.md        # Secure notes feature
│   │   └── sql-runner.md          # SQL runner functionality
│   ├── deployment/                # Deployment guides
│   │   ├── local-dev.md           # Local development setup
│   │   ├── docker.md              # Docker deployment guide
│   │   └── production.md          # Production deployment guide
│   ├── guides/                    # User guides
│   │   ├── installation.md        # Installation instructions
│   │   ├── project-structure.md   # Project structure explanation
│   │   ├── what.md                # What is N-Ops
│   │   ├── why.md                 # Why use N-Ops
│   │   └── example.md             # Example use cases
│   ├── contribute/                # Contribution guidelines
│   │   ├── how.md                 # How to contribute
│   │   ├── roadmap.md             # Project roadmap
│   │   └── structure.md           # Contribution structure
│   ├── tutorial-basics/           # Basic tutorials
│   └── tutorial-extras/           # Advanced tutorials
├── src/                           # Custom React components
│   ├── components/                # Reusable UI components
│   │   └── HomepageFeatures/      # Homepage feature components
│   ├── css/                       # CSS styles
│   │   └── custom.css             # Custom CSS overrides
│   └── pages/                     # Static pages
│       ├── index.js               # Homepage
│       └── markdown-page.md       # Example markdown page
├── static/                        # Static assets
│   └── img/                       # Images and icons
├── docusaurus.config.js           # Docusaurus configuration
├── sidebars.js                    # Sidebar configuration
├── wrangler.jsonc                 # Cloudflare deployment config
├── babel.config.js                # Babel configuration
└── package.json                   # Project dependencies and scripts
```

## 📋 Available Scripts

| Script                       | Description                                                                  |
| ---------------------------- | ---------------------------------------------------------------------------- |
| `npm start`                  | Start the development server                                                 |
| `npm run build`              | Build the documentation for production                                       |
| `npm run serve`              | Serve the production build locally to test before deploying                  |
| `npm run deploy`             | Build and deploy the documentation to Cloudflare Pages                       |
| `npm run preview`            | Build and preview the documentation locally with Wrangler                    |
| `npm run clear`              | Clear the Docusaurus cache to resolve any caching issues                     |
| `npm run swizzle`            | Customize Docusaurus components; use with caution as it ejects the component |
| `npm run write-translations` | Extract translatable content                                                 |
| `npm run write-heading-ids`  | Generate heading IDs                                                         |

## 🚢 Deployment

This documentation is deployed on **Cloudflare Pages** using Wrangler. The deployment process is automated to ensure the latest documentation is always available.

### Deploy to Cloudflare

Before deploying, ensure you have the Cloudflare Wrangler CLI installed and configured:

```bash
# Install Wrangler CLI globally
npm install -g wrangler

# Authenticate with Cloudflare
wrangler login

# Deploy to Cloudflare Pages
npm run deploy
```

To preview the deployment locally before pushing to production:

```bash
# Preview deployment locally
npm run preview
```

### Continuous Deployment

The documentation site is automatically deployed when changes are pushed to the main branch. The CI/CD pipeline:

1. Builds the documentation site
2. Runs tests to ensure everything is working correctly
3. Deploys to Cloudflare Pages
4. Sends notifications upon successful or failed deployments

## 👥 Contributing

We welcome contributions to improve the N-Ops documentation! Whether you're fixing typos, adding new documentation, or improving existing content, your help is appreciated.

### Contribution Workflow

1. **Fork** the repository by clicking the "Fork" button at the top right of the repository page.
2. **Clone** your forked repository to your local machine:

   ```bash
   git clone https://github.com/your-username/N-Ops-Docs.git
   cd N-Ops-Docs
   ```

3. **Create** a new branch for your changes:

   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Make** your changes to the documentation.
5. **Test** your changes locally:

   ```bash
   npm start
   ```

6. **Commit** your changes with descriptive messages:

   ```bash
   git add .
   git commit -m 'Add comprehensive documentation for feature X'
   ```

7. **Push** your changes to your remote branch:

   ```bash
   git push origin feature/your-feature-name
   ```

8. **Create** a Pull Request (PR) on GitHub by navigating to your forked repository and clicking the "New Pull Request" button.
9. **Fill out** the PR template with details about your changes.
10. **Wait** for a maintainer to review your PR and address any feedback.

### Documentation Guidelines

- **Language**: Use clear, concise language. Avoid jargon when possible, and explain technical terms when they are introduced.
- **Structure**: Follow the existing document structure. Use headings to organize content hierarchically.
- **Code Examples**: Include practical code examples where applicable. Use syntax highlighting for code blocks.
- **Images**: Use screenshots and diagrams to illustrate complex concepts. Optimize images for web before adding them.
- **Links**: Use relative links for internal documentation. Check that all links work before submitting.
- **Testing**: Test your documentation changes locally to ensure they render correctly.
- **Sidebar**: Update the sidebar configuration (`sidebars.js`) if adding new sections or pages.

### Setting up Gitpod for Online Contribution

For quick contributions without setting up a local environment, you can use Gitpod:

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/Neko-Nik-Org/N-Ops-Docs)

Gitpod provides a fully configured development environment in your browser, with all dependencies pre-installed.

## ⚙️ Configuration

### Key Configuration Files

- `docusaurus.config.js`: Main Docusaurus configuration file. Controls the site's metadata, navigation, footer, and plugins.

```javascript
// Example configuration snippet
module.exports = {
  title: "N-Ops Documentation",
  tagline: "Automate your DevOps with N-Ops",
  url: "https://n-ops.nekonik.org",
  baseUrl: "/",
  // Additional configuration...
};
```

- `sidebars.js`: Defines the sidebar navigation structure. Modify this file to update the documentation's table of contents.

```javascript
// Example sidebar configuration
module.exports = {
  docs: [
    "intro",
    "get-started",
    {
      type: "category",
      label: "Backend",
      items: ["backend/overview", "backend/api-routes" /* ... */],
    },
    // Additional configuration...
  ],
};
```

- `wrangler.jsonc`: Cloudflare deployment configuration. This file configures how the site is deployed to Cloudflare Pages.

- `package.json`: Project dependencies and scripts. This file manages the project's dependencies and defines the npm scripts used for development and deployment.

### Customization Options

- **Theme**:

  - Modify `src/css/custom.css` for styling
  - This file contains the custom CSS rules that override the default Docusaurus theme
  - You can adjust colors, typography, spacing, and other visual elements

- **Homepage**:

  - Edit `src/pages/index.js`
  - This file defines the content and layout of the homepage
  - You can customize the hero section, feature highlights, and other homepage components

- **Components**:

  - Add custom React components in `src/components/`
  - This directory is where you can add reusable React components
  - Components can be used across multiple documentation pages

- **Plugins**:
  - Add or configure Docusaurus plugins in `docusaurus.config.js`
  - Plugins extend functionality like search, analytics, and more

## 🔧 Built With

- [Docusaurus 3](https://docusaurus.io/) - Modern documentation framework that makes creating beautiful, functional documentation sites easy
- [React 19](https://react.dev/) - UI library for building interactive user interfaces
- [Cloudflare Pages](https://pages.cloudflare.com/) - Fast, secure hosting platform with global CDN
- [Prism](https://prismjs.com/) - Syntax highlighting for code blocks
- [MDX](https://mdxjs.com/) - Markdown extension that allows embedding React components

## 📞 Support & Contact

- **Email**: [nikhil@nekonik.org](mailto:nikhil@nekonik.org)
- **Discord**: [Join our community](https://discord.com/invite/PYqHVUGdwv)
- **GitHub Issues**: [Report bugs or request features](https://github.com/Neko-Nik-Org/N-Ops-Docs/issues)
- **GitHub Discussions**: [Ask questions and share ideas](https://github.com/Neko-Nik-Org/N-Ops-Docs/discussions)

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

Copyright © 2024 Neko Nik. Built with [Docusaurus](https://docusaurus.io/).

## 🔄 Related Projects

- [N-Ops API](https://github.com/Neko-Nik-Org/N-Ops-API) - Backend API for the N-Ops platform
- [N-Ops Client](https://github.com/Neko-Nik-Org/N-Ops-Client) - Frontend client for N-Ops
- [N-Ops CLI](https://github.com/Neko-Nik-Org/N-Ops-CLI) - Command-line interface for N-Ops

---

<div align="center">
<p>⭐ <strong>Star this repository</strong> if you find it helpful! ⭐</p>
<p>
    <a href="https://n-ops.nekonik.org">Documentation</a> |
    <a href="https://github.com/Neko-Nik-Org/N-Ops-API">Main Project</a> |
    <a href="https://github.com/Neko-Nik-Org">GitHub Organization</a>
</p>
</div>
