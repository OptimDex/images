# Image Assets Repository

This repository is a simple static asset store for images used by other projects. It's intended to host image files (PNG, JPG, WebP, SVG, etc.) and provide clear guidance on organization, naming, usage, and contribution.

**Purpose:**
- Store and serve static image assets centrally for projects that reference them by path or URL.

**Contents:**
- Image files organized in folders. Each folder should represent a logical grouping (e.g., `icons/`, `logos/`, `photos/`, `sprites/`).

**Usage:**
- Reference images by their repository path or by the static URL served by your hosting (for example, a CDN or GitHub Pages). Example path: `images/logos/company-logo.png`.

**Naming Conventions:**
- Use lowercase letters, hyphens for separators (`company-logo.png`).
- Include size or scale when relevant (`icon-16x16.png`, `hero-1920w.jpg`).
- Prefer semantic names over numeric ones when meaningful (`user-avatar-default.png`).

**Recommended Formats & Optimization:**
- Use SVG for vector graphics (icons, logos) when possible.
- Use WebP for photographic images when browser support and hosting allow it; provide a JPEG/PNG fallback if needed.
- Keep file sizes minimal: compress images and remove unnecessary metadata.
- For responsive images, provide multiple widths and use `srcset` on the frontend.

**Example file:**
- `ragnarok/ragnarok-origin-310×196.png` — example raster image included in the `ragnarok/` folder. The filename includes the original dimensions to make intended display size obvious (`310×196`).

**Branch & direct access:**
- All images in this repository are stored on the `main` branch.
- You can access any file directly using the raw GitHub URL pattern:

	`https://raw.githubusercontent.com/<owner>/<repo>/<branch>/path/to/image.png`

	For example, the example file above can be accessed as:

	`https://raw.githubusercontent.com/OptimDex/images/main/ragnarok/ragnarok-origin-310×196.png`

	Markdown embed example:

	`![ragnarok example](https://raw.githubusercontent.com/OptimDex/images/main/ragnarok/ragnarok-origin-310×196.png)`

**Contributing:**
- Add new images to an appropriately named folder.
- Update this README if you add a new top-level category.
- Images should be checked for size and format — optimized and proven necessary.
- Open a pull request with the image files and a short description of purpose and usage.

**License:**
- Check individual image sources for license requirements. By default, files in this repo inherit the repository `LICENSE` unless otherwise noted in the file or folder.

If you'd like, I can also add a short script to generate `srcset` entries or a small validation action to check image sizes on PRs.

**Last Update:** 2025-12-17

**Version:** v0.1
