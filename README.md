<a href="https://spectre-org.github.io/spectre-css">
  <img src="https://spectre-org.github.io/spectre-docs/img/spectre-logo.svg" width="72" height="72">
</a>

## Spectre CSS

[![Reviewed by Hound](https://img.shields.io/badge/Reviewed_by-Hound-8E64B0.svg)](https://houndci.com)

> This version of Spectre CSS has been forked from the [original repo](https://github.com/picturepan2/spectre); see the [organisation readme](https://github.com/spectre-org) for rationale.

Spectre is a lightweight, responsive and modern CSS framework.

- Lightweight (~10KB gzipped) starting point for your projects
- Flexbox-based, responsive and mobile-friendly layout
- Elegantly designed and developed elements and components

Spectre is a side project based on years of CSS development work on a large web service project.

Spectre only includes modern base styles, responsive layout system, CSS components and utilities, and it can be modified for your project using standard build tools.

### Usage (Sivujetti-Spectre CSS)

Add these before or after `sivujetti-spectre.min.css`:

```css
:root {
  --spectre-font-size: 0.8rem;
  --spectre-primary-color: #5755d9;
  --spectre-dark-color: #303742;
  --spectre-light-color: #fff;
  --spectre-primary-color-dark: #4b48d6; /* darken(--spectre-primary-color, 3%), you can use http://scg.ar-ch.org/ for this */
  --spectre-primary-color-light: #6361dc; /* lighten(--spectre-primary-color, 3%) */
  --spectre-secondary-color: #efeffb; /* lighten(--spectre-primary-color, 37.5%) */
  --spectre-secondary-color-dark: #e3e3f8; /* darken(--spectre-secondary-color, 3%) */
  --spectre-secondary-color-light: #fbfbfe; /* lighten(--spectre-primary-color, 3%) */
  --spectre-link-color: #5755d9; /* --spectre-primary-color */
  --spectre-link-color-dark: #302ecd; /* darken(--spectre-link-color, 10%) */
  --spectre-link-color-light: #807fe2; /* lighten(--spectre-link-color, 10%) */
  --spectre-base-font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", Roboto;
  --spectre-body-font-color: #3b4351; /* lighten(--spectre-dark-color, 5%) */
  --spectre-primary-shadow-color: #5755d933; /* rgba(0.2) */
  --spectre-gray-color: #bcc3ce; /* lighten(--spectre-dark-color, 55%) */
  --spectre-gray-color-dark: #66748b; /* darken(--spectre-gray-color, 30%) */
  --spectre-gray-color-light: #f7f8f9; /* lighten(--spectre-gray-color, 20%) */
  --spectre-border-color: #dadee4; /* lighten($dark-color, 65%) */
  --spectre-border-color-dark: #bdc4ce; /* darken(--spectre-border-color, 10%) */
  --spectre-border-color-light: #f2f3f5; /* lighten(--spectre-border-color, 8%) */
  --spectre-bg-color: #f7f8f9; /* lighten(--spectre-dark-color, 75%) */
  --spectre-bg-color-dark: #eef0f2; /* darken(--spectre-bg-color, 3%) */
}
```

## Documentation

New documentation is available at:

- [spectre-org.github.io/spectre-docs](https://spectre-org.github.io/spectre-docs)

Getting started:

- [Installation](https://spectre-org.github.io/spectre-docs/docs/introduction/installation.html)
- [Build](https://spectre-org.github.io/spectre-docs/docs/introduction/build.html)

Content:

- [Elements](https://spectre-org.github.io/spectre-docs/docs/elements/index.html)
- [Layout](https://spectre-org.github.io/spectre-docs/docs/layout/index.html)
- [Components](https://spectre-org.github.io/spectre-docs/docs/components/index.html)
- [Experimentals](https://spectre-org.github.io/spectre-docs/docs/experimentals/index.html)
- [Utilities](https://spectre-org.github.io/spectre-docs/docs/utilities/index.html)

Related content:

- [Original Spectre.css issues](https://github.com/picturepan2/spectre/issues)
- [Original Spectre.css docs](https://picturepan2.github.io/spectre/)
- [Spectre.css on Twitter](https://twitter.com/spectrecss)

## Contributing

Clone this repo locally with:

```bash
git clone https://github.com/spectre-org/spectre-css.git
```

Spectre uses [Gulp](http://gulpjs.com/) to compile CSS:

```bash
# compile SCSS to CSS and minify files
gulp build    

# watch file changes and re-compile
gulp watch    
```

To work with Spectre CSS source files live in another project, you can use NPM link.

In the Spectre CSS repo, create the global reference:

```bash
npm link
```

In your project repo, create the link:

```bash
npm link @spectre-org/spectre-css
```

The existing `node_modules/@spectre-org/spectre-css` folder will be replaced with a symlink to the local repository, and any changes there will be reflected immediately in your project.
