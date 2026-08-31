# Academic & Professional Portfolio

A modern, responsive Jekyll-based portfolio website showcasing academic research, publications, talks, teaching experience, and professional projects.

## 📋 Overview

This portfolio site is built with Jekyll and hosted on GitHub Pages. It features:

- **Publications** - Display academic papers and research work
- **Talks & Presentations** - Showcase conference talks and seminars
- **Teaching** - Document teaching experience and courses
- **Blog Posts** - Share insights and regular content
- **Portfolio Projects** - Highlight key professional work
- **CV/Resume** - Professional experience and qualifications
- **Responsive Design** - Mobile-friendly interface
- **Docker Support** - Containerized local development

## 🚀 Quick Start

### Option 1: Local Installation (Recommended)

**Prerequisites:**

- Ruby 2.7+
- Bundler
- Git

**Setup:**

```bash
# Clone the repository
git clone https://github.com/madhavr35/madhavr35.github.io.git
cd madhavr35.github.io

# Install dependencies
bundle install

# Start the Jekyll development server
bundle exec jekyll serve

# Visit http://localhost:4000
```

### Option 2: Docker Setup

**Prerequisites:**

- Docker
- Docker Compose

```bash
# Build and run the container
docker-compose up

# Visit http://localhost:4000
```

## 📁 Directory Structure

```plaintext
.
├── _posts/              # Blog posts (YYYY-MM-DD-title.md)
├── _publications/       # Academic papers
├── _talks/              # Conference talks and presentations
├── _teaching/           # Teaching experience and courses
├── _portfolio/          # Portfolio projects and case studies
├── _pages/              # Static pages (about, CV, archive, etc.)
├── _layouts/            # Jekyll template layouts
├── _includes/           # Reusable template components
├── _sass/               # SCSS stylesheets
├── _data/               # Data files (navigation, authors, CV)
├── assets/              # Static files (CSS, JS, images)
├── files/               # downloadable files
├── images/              # Image assets
├── _config.yml          # Main Jekyll configuration
└── Gemfile              # Ruby dependencies
```

## ✏️ Adding Content

### Blog Posts

Create a new file in `_posts/` with format: `YYYY-MM-DD-post-title.md`

```markdown
---
title: "Post Title"
date: 2024-01-15
permalink: /posts/2024/01/post-title/
categories: [technology, development]
tags: [jekyll, github-pages]
excerpt: "Brief description of your post"
---

Your post content here...
```

### Publications

Create a file in `_publications/` with format: `YYYY-MM-DD-paper-title.md`

```markdown
---
title: "Paper Title"
collection: publications
permalink: /publication/2024-01-15-paper-title
date: 2024-01-15
venue: "Conference Name"
citation: 'Author, Year. "Title." Venue.'
---

Paper abstract and details...
```

### Talks

Create a file in `_talks/` with format: `YYYY-MM-DD-talk-title.md`

```markdown
---
title: "Talk Title"
collection: talks
type: "Talk"
permalink: /talks/2024-01-15-talk-title
date: 2024-01-15
location: "Conference, City"
---

Talk description and details...
```

### Teaching

Create a file in `_teaching/` with format: `YYYY-season-course-name.md`

```markdown
---
title: "Course Name"
collection: teaching
type: "Course"
permalink: /teaching/2024-spring-course-name
date: 2024-01-15
location: "Institution"
---

Course description, materials, and details...
```

### Portfolio Projects

Create a file in `_portfolio/` with format: `project-name.md` or `.html`

```markdown
---
title: "Project Name"
excerpt: "Short project description"
header:
  image: /images/project-image.png
  teaser: /images/project-teaser.png
---

Project details, methodology, and results...
```

## ⚙️ Configuration

Edit `_config.yml` to customize:

- **Site Title & Description** - Main site metadata
- **Author Information** - Your name, bio, social profiles
- **Navigation** - Edit `_data/navigation.yml` for menu items
- **Theme Settings** - Colors, fonts, and layout options
- **URL & Baseurl** - For GitHub Pages deployment

### Key Configuration Files

- `_config.yml` - Main configuration
- `_config_docker.yml` - Docker-specific overrides
- `_data/navigation.yml` - Menu structure
- `_data/authors.yml` - Author profiles
- `_data/cv.json` - CV data (if using structured format)

## 🔧 Development

### Build the site (without serving)

```bash
bundle exec jekyll build
```

### Watch for changes

```bash
bundle exec jekyll serve --livereload
```

### Run linting/checks

```bash
# Check for errors
bundle exec jekyll doctor
```

## 🚢 Deployment

### Automatic (GitHub Pages)

The site automatically deploys when you push to the `main` or `master` branch (if using GitHub Pages with Jekyll).

**Requirements:**

- Repository name: `USERNAME.github.io`
- GitHub Pages enabled in repository settings
- Branch set to publish from: `main` or `master`

### Manual Build & Deploy

```bash
# Build the site
bundle exec jekyll build

# The static site is in the _site/ directory
# Deploy to your hosting platform
```

## 📝 Common Tasks

**Update Navigation Menu:**
Edit `_data/navigation.yml`

**Add Social Links:**
Edit `_data/authors.yml`

**Change Site Colors/Fonts:**
Modify `_sass/_themes.scss` and `_sass/_variables.scss`

**Add Custom CSS:**
Create/edit `assets/css/main.scss`

**Update CV:**
Edit `_pages/cv.md` or `_data/cv.json`

## 🛠️ Built With

- **Jekyll** - Static site generator
- **SASS/SCSS** - Stylesheets
- **Minimal Mistakes** - Jekyll theme (customized)
- **GitHub Pages** - Hosting
- **Docker** - Containerization

## 📦 Dependencies

See [Gemfile](Gemfile) for complete Ruby dependencies.

Key gems:

- `jekyll` - Static site generator
- `jekyll-paginate-v2` - Pagination
- `jekyll-gist` - GitHub Gist embedding
- `jemoji` - Emoji support

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

Found a bug or have suggestions? Please open an issue or submit a pull request.

## 📧 Contact

Connect with me:

- 📍 [GitHub](https://github.com/madhavr35)
- 📚 [Portfolio](https://madhavr35.github.io)
- 📝 Check `_data/authors.yml` for additional social links

---

**Last Updated:** 2026
**Maintained by:** Madhav Ramesh
