# Portfolio — Aerospace Engineering

Custom Jekyll portfolio site for GitHub Pages. Editorial style: serif headlines
(Fraunces), clean sans body (Inter), warm off-white background with deep slate
blue and denim accents — no dark mode, no tech-bro cyan.

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
- Edit your name in the `.hero-name` heading
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
**Easiest way — no terminal needed:**
1. Create a new repo on GitHub named `yourusername.github.io`
2. Click **Add file → Upload files**, drag in everything from this folder
3. Commit changes
4. Go to **Settings → Pages → Source** and select **GitHub Actions**
5. Add your images via **Add file → Upload files** again — type the folder path
   (e.g. `images/para_mach.png`) into the filename box to auto-create folders

Your site goes live at `https://yourusername.github.io` within a couple of minutes.
Check progress under the **Actions** tab.

### Local development (optional, if you have Ruby installed)
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
index.html            # Home page — text-led hero, no photo
research.html        # CFD research page
projects.html         # All projects page
Gemfile               # Ruby dependencies
.github/workflows/
  deploy.yml          # Auto-deploy to GitHub Pages
```

## Design notes
- **Fonts:** Fraunces (serif, headlines) + Inter (sans, body)
- **Palette:** slate blue `#2C3A4D`, blue-gray `#5B6B7F`, denim accent `#4A6585`,
  warm off-white `#F7F5F0`
- No animation, no dark theme — calm and editorial, matching the aerospace
  engineer portfolios that inspired it (Katie Heinemann, Davis Ryan, etc.)
