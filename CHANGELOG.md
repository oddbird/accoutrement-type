Changelog
=========


3.2.0 - Unreleased
------------------
- NEW: Add `svgid` option to font maps
- NEW: Allow either string or number values
  for font-weights (e.g. `200` or `'200'` )
- NEW: Allow font-variants to define a sub-map
  of format/path pairs rather, than a single relative path -
  especially useful for defining data-uri embedded fonts.
- NEW: Format data-uri `src` values correctly


3.1.0 - 09/28/17
----------------

- NEW: `add-font` mixin makes font-config organization simpler


3.0.1 - 09/13/17
----------------

- Update docs.


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
