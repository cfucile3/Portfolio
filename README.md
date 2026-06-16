# Portfolio — Aerospace Engineering

Custom Jekyll portfolio site for GitHub Pages.

## Setup

### 1. Personalize `_config.yml`
Replace the placeholder values:
```yaml
title: "Your Name"
author:
  name: "Your Name"
  email: "your.email@gatech.edu"
  linkedin: "https://linkedin.com/in/yourprofile"
  github: "https://github.com/yourusername"
```

### 2. Update `index.html`
- Edit your name in the `.hero-name` heading (two places — HTML and display)
- Update the bio paragraph
- Adjust skill tags to match your actual tools

### 3. Add your assets
Place images and GIFs in the correct folders:
```
images/
  para_mach.png
  para_validation.png
  nozz_mach.png
  nozz_pressure.png
  vert_pressure.png
  vert_kinetic.png
  groundtrack.png
  drag_polar.png
  turbine_setup.png
gifs/
  l2_motion.gif
  robot_motion.gif
papers/
  stockholm_turbine.pdf
```

### 4. Deploy to GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to **GitHub Actions**
4. Push to `main` — the workflow deploys automatically

### Local development
```bash
bundle install
bundle exec jekyll serve
# Visit http://localhost:4000
```

## File structure
```
_config.yml          # Site settings
_layouts/
  default.html       # Base layout, nav, styles, footer
index.html           # Home page with animated hero
research.html        # CFD research page
projects.html        # All projects page
Gemfile              # Ruby dependencies
.github/workflows/
  deploy.yml         # Auto-deploy to GitHub Pages
```
