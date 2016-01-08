Accoutrement-Fonts
==================

Webfont management tools.
Gather all your fonts into a single map,
access them by name,
and easily import the webfonts.


Quick Start
-----------

```bash
npm install accoutrement-fonts
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
    'normal': 'exo/exo2-regular-webfont',
    'italic': 'exo/exo2-italic-webfont',
    'bold': 'exo/exo2-bold-webfont',
    'bold' 'italic': 'exo/exo2-bolditalic-webfont',
  ),

  'alias': 'body', // create aliases when useful
);
```

Import a webfont,
or all your configured fonts with a mixin:

```scss
@include font-face('body'); // Import one font by configuration key
@include import-webfonts; // Import all defined fonts
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


About OddBird Accoutrement
--------------------------

[OddBird][oddbird]'s *Accourement* modules
are individual Sass toolkits
that work together to form
the central nervous system of a project.
They help to establish and access a projects configuration
in consistent and inter-connected ways.

[oddbird]: http://oddbird.net/
