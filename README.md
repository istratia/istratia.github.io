# Glen Rock Historical & Preservation Society Website

This repository contains the source code for the Glen Rock Historical & Preservation Society (GRHPS) website. The site is built using Jekyll and is hosted on GitHub Pages.

## Technology Stack

- **Static Site Generator**: Jekyll
- **CSS Framework**: Tailwind CSS
- **Deployment**: GitHub Pages

## Project Structure

```
.
├── _config.yml          # Jekyll configuration
├── _layouts/           # Layout templates
├── _includes/          # Reusable components
├── _posts/            # Blog posts
├── _gallery/          # Gallery collection
├── _resources/        # Resources collection
├── _events/           # Events collection
├── _projects/         # Projects collection
└── assets/           # Static assets
```

## Development Setup

1. Install Ruby and Jekyll
```bash
gem install bundler jekyll
```

2. Install dependencies
```bash
bundle install
```

3. Run the development server
```bash
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`

## Required Images

The following images need to be placed in the `/assets/images/` directory:

1. `glen-rock-hero.jpg` - Hero section background image
2. `heritage-trail.jpg` - Image for Heritage Trail section
3. `photo-gallery.jpg` - Image for Photo Gallery section
4. `road2liberty.jpg` - Image for Road2Liberty section
5. `veteran-banners.jpg` - Image for Veteran Banners section

Image requirements:
- Format: JPG/JPEG
- Aspect ratio: 16:9 for featured resources
- Resolution: Minimum 1200x675 pixels recommended
- File size: Optimize for web (< 500KB per image)

## Contributing

1. Create a new branch for your feature
2. Make your changes
3. Submit a pull request

## License

Copyright © Glen Rock Historical & Preservation Society. All rights reserved.