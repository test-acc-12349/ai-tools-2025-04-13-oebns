# AI Tools Directory 🤖

> The ultimate directory of AI tools and resources for enhancing productivity and creativity.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization](#customization)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources](#resources)
- [Support](#support)

## Overview

AI Tools Directory is a curated collection of artificial intelligence tools and resources, presented in a clean, responsive 3-column grid layout. The directory showcases various AI tools including writers, SEO tools, chrome extensions, and more.

## Features

- 📱 Responsive 3-column grid layout
- 🏷️ Category filtering system
- 🔍 Search functionality
- 🎯 Featured items section
- 💫 Smooth animations
- 🎨 Customizable styling
- 📊 SEO optimized

## Demo

Visit the live demo: [https://ai-tools-directory.com](https://ai-tools-directory.com)

## Getting Started

### Prerequisites

- Node.js (v14.0.0 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── src/
│   ├── components/
│   │   ├── Header.js
│   │   ├── DirectoryGrid.js
│   │   ├── CategoryFilter.js
│   │   └── SearchBar.js
│   ├── data/
│   │   └── directory-items.js
│   ├── styles/
│   │   └── main.css
│   └── pages/
│       └── index.js
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization

### Adding Directory Items

Edit `src/data/directory-items.js`:

```javascript
export const directoryItems = [
  {
    id: "ai-writer",
    title: "AI Writer",
    description: "Advanced AI writing assistant",
    category: ["ai", "new"],
    image: "/images/ai-writer.png",
    url: "https://aiwriter.com"
  },
  // Add more items here
];
```

### Modifying Categories

Edit the category array in `src/data/categories.js`:

```javascript
export const categories = [
  "ai",
  "new",
  "sale"
];
```

### Updating Hero Section

Modify the hero section in `src/components/Header.js`:

```javascript
<div className="hero">
  <h1>AI Tools Directory</h1>
  <p>Your custom description here</p>
</div>
```

### Customizing Colors

Edit `src/styles/main.css`:

```css
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
  --background-color: #f5f6fa;
  --text-color: #2c3e50;
}
```

## Deployment

### Vercel Deployment

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

### Netlify Deployment

1. Connect your GitHub repository to Netlify
2. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
3. Click "Deploy"

## Custom Domain Setup

1. Purchase domain from your preferred registrar
2. Add domain in deployment platform:
   ```
   Domain: yourdomain.com
   ```
3. Configure DNS settings:
   ```
   A Record: @ -> Your-Platform-IP
   CNAME: www -> yourdomain.netlify.app
   ```
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. **Build Failures**
   ```bash
   npm run build --verbose
   ```

2. **Styling Issues**
   - Clear browser cache
   - Check CSS specificity
   - Verify media queries

3. **Image Loading**
   - Confirm image paths
   - Check file permissions
   - Verify image formats

## Resources

- [Documentation](https://docs.ai-tools-directory.com)
- [API Reference](https://api.ai-tools-directory.com)
- [Style Guide](https://style.ai-tools-directory.com)
- [Contributing Guidelines](CONTRIBUTING.md)

## Support

- 📧 Email: support@ai-tools-directory.com
- 💬 Discord: [Join our community](https://discord.gg/ai-tools)
- 🐦 Twitter: [@AIToolsDir](https://twitter.com/AIToolsDir)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [Your Name]