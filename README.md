# DevEx V2: From Scripts to Intelligent Systems

A Jekyll-based presentation for the Atlassian DevEx Meetup exploring the impact of ML and Large Language Models on DevOps and Developer Experience.

## Quick Start

### Local Development

1. **Install dependencies:**
   ```bash
   bundle install
   ```

2. **Run the site locally:**
   ```bash
   bundle exec jekyll serve
   ```

3. **View the presentation:**
   Open `http://localhost:4000` in your browser

### GitHub Pages Deployment

This site is configured to automatically deploy to GitHub Pages when you push to the `develop` branch.

1. **Enable GitHub Pages:**
   - Go to your repository settings
   - Navigate to "Pages"
   - Set source to "GitHub Actions"

2. **Push to deploy:**
   ```bash
   git add .
   git commit -m "Deploy presentation"
   git push origin develop
   ```

## How to Use

### Slide Structure
- Each slide is a separate Markdown file in `_slides/`
- Slides are automatically linked with navigation
- Progress bar shows presentation progress

### Customization

#### Adding New Slides
1. Create a new file in `_slides/` (e.g., `slide-09.md`)
2. Add the front matter:
   ```yaml
   ---
   layout: slide
   title: "Your Slide Title"
   slide_number: 9
   prev_slide: "/slide-08"
   next_slide: "/slide-10"
   ---
   ```
3. Update the previous slide's `next_slide` field
4. Update `_data/slides.yml` with the new slide info
