# Architecture

## Runtime model
- WordPress plugin entrypoint: `wp-content/plugins/sparxstar-data-gap/sparxstar-data-gap.php`
- Front-end renderer: `assets/js/neural-map.js` using self-hosted Three.js
- Style layer: `assets/css/neural-map.css`

## Design constraints
- No runtime dependency on third-party map APIs.
- Deterministic rendering from embedded data.
- Shortcode-driven embedding for WordPress pages/posts.

## Boundaries
- PHP layer: asset registration + shortcode output.
- JS layer: visualization and interaction logic.
- CI/release workflows: build, package, tag-driven release publishing.
