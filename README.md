Accoutrement-Type
=================

Sass typography [Accoutrement][accoutrement]
by [OddBird][oddbird].
Gather all your fonts into a single map,
access them by name,
and easily import the webfonts.
Also includes helpers for accessibility
and pseudo-elements.

[accoutrement]: http://oddbird.net/accoutrement/
[oddbird]: http://oddbird.net/


Quick Start
-----------

```bash
npm install accoutrement-type
```

Import the library:

```scss
@import 'path/to/accoutrement-type/type';
```

Configure your font settings:

```scss
$font-formats: 'woff' 'ttf'; // Define what webfont formats need importing
$font-path: '../fonts/'; // Set the a path to your fonts directory

$fonts: (
  'heading': ( // give your font a semantic name for reference
    'name': 'maven', // optionally set a different font name
    'stack': ('helvetica', 'arial', sans-serif), // define the stack
    'normal': 'maven/maven_pro_regular-webfont', // point to any webfont files
    'bold': 'maven/maven_pro_bold-webfont',
  ),

  'body': (
    'name': 'exo',
    'stack': ('helvetica', 'arial', sans-serif),
    'normal': false, // set variant paths to false when using font CDNs...
    'italic': false, // ...if you still want to document available styles
    'bold': false,
    'bold' 'italic': false,
  ),

  'alias': 'body', // create aliases when useful
);
```

Import one font at a time with `font-face()`
or all your webfonts ar once with `import-webfonts()`:

```scss
// Import one font by configuration key, with custom formats
@include font-face('body', 'otf' 'svg');

// Import all defined fonts, using the same formats
@include import-webfonts;
```

And set your font-family anywhere,
using the semantic names you set earlier:

```scss
html {
  @include font-family('body');
}

h1, h2, h3 {
  @include font-family('heading');
}
```


Changelog
---------

### 2.1.0 — 2016.12.09

- Document `$font` properties
- Add `false` option for font-variants,
  to allow documentation without triggering imports
- Test remaining mixins:
  `font-face`, `import-webfonts`, and `_import-font-face`


