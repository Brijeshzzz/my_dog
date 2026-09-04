# Agent Instructions

## Project Shape

- This is a dependency-free static HTML research site; there is no build tool, package manager, or test suite.
- `index.html` is the homepage. Research articles use zero-padded numeric filenames such as `001.html` and `002.html`.
- GitHub Pages deploys the repository root directly through `.github/workflows/deploy.yml`.

## Theme And Content

- Preserve the deliberate late-1990s documentation aesthetic: dark `#1A1A1A` background, off-white body text, white headings, blue links, gray rules and borders, centered fixed-width content, and simple HTML elements.
- Keep the site JavaScript-free and avoid external libraries, trackers, advertisements, cookies, and unnecessary modern framework or build additions.
- Keep typography and spacing consistent with the existing pages unless a change explicitly requests a visual redesign. Existing pages use Verdana-family sans-serif text, 18px body text, and generous line height.
- Research content should remain direct and technical. Preserve the author's informal voice where it is part of an article rather than rewriting it into marketing copy.

## Editing Conventions

- Prefer small, local edits to the existing inline styles and HTML. The shared CSS is duplicated in the three pages, so theme changes must be kept synchronized across `index.html`, `001.html`, and `002.html` when applicable.
- Use relative paths for assets under `images/`. Preserve unusual existing filenames, including colons, unless a rename is explicitly required.
- Before adding an image link, confirm the asset exists. Be aware that `images/watch.jpg` is currently referenced but absent.
- Preserve the existing numeric article naming scheme and update homepage links when adding or renaming articles.
- Check anchors and links after edits; the homepage currently includes a `#contact` link without a matching section, so do not introduce additional dangling targets.
- Preserve the site's legacy markup intentionally, but keep any new markup valid and add missing structural elements only when the task calls for cleanup.

## Validation

- Validate changed HTML by opening the relevant file in a browser or using an available HTML checker; test both a desktop-sized and narrow viewport when layout changes are involved.
- Confirm every changed relative asset path exists and every new internal link has a destination.
- Review the rendered result for horizontal overflow on narrow screens before changing the established fixed-width layout.