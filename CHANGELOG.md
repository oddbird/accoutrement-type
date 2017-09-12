Changelog
=========


3.0.0 - 09/12/17
----------------

- BREAKING: Use proper `::` syntax for pseudo-elements
- BREAKING: Set `pointer-events: none` on hidden text


2.1.0 — 12/09/16
----------------

- Document `$font` properties
- Add `false` option for font-variants,
  to allow documentation without triggering imports
- Test remaining mixins:
  `font-face`, `import-webfonts`, and `_import-font-face`


2.0.0 - 02/22/16
----------------

- NEW: `is-hidden()` mixin for screen-reader accessible, hidden text
- NEW: Add pseudo-element helper mixins:
  `before()`, `after()`, and `wrap-content()`
- BUGFIX: Add quotes to font url
- BREAKING: re-write font-helpers
