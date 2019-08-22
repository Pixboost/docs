# Installation

The easiest way to start using the library is to include it on the page and turn on autoload:

```markup
<script 
  type="text/javascript" 
  src="https://pixboost.com/libs/pixboost.bundle.min.js"
  id="pb-script"
  data-api-key="<YOUR PIXBOOST API KEY>"
  data-autoload=""
></script>
```

pixboost.bundle.min.js script includes picturefill library that adds support of `<picture>` element to old browsers, lozad.js for lazy loading and matchMedia.js for supporting matchMedia\(\) call in IE9.

autoload option will run `picture()`, `image()` and `background()` functions \(see below\) on document load.

Alternatively, you can include all components separately:

```markup
<!--Responsive images-->
<script type="text/javascript" src="https://pixboost.com/libs/picturefill.min.js"></script>

<!-- Lazy loading-->
<script type="text/javascript" src="https://pixboost.com/libs/lozad.min.js"></script>

<!-- Match media-->
<script type="text/javascript" src="https://pixboost.com/libs/matchMedia.min.js"></script>

<script type="text/javascript" src="https://pixboost.com/libs/pixboost.min.js"></script>
```

Library provides three main functions:

* [picture\(\)](responsive-images.md) - to deal with responsive images.
* [image\(\)](not-responsive-images.md) - to optimise all images that are device agnostic.
* [background\(\)](css-background-images.md) - for images that using CSS background

