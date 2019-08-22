# Lazy Loading

Lazy loading will not load image until it becomes visible to a user. Pixboost.js supports lazy loading for both responsive and non-responsive images. To enable lazy load you need to add `data-lazy` attribute to `<div>` or `<img>` elements.

```markup
<div data-pb-picture
    data-lazy
    data-url="https://yoursite.com/doggy.png"
    data-lg="optimise"
    data-md="resize?size=300"
    data-sm="fit?size=100x100"/>
```

```markup
<img data-pb-image data-lazy data-op="resize?size=x600" data-src="https://yoursite.com/doggy.png"/>
```

Lazy loading in Pixboost.js implemented by using 3rd party library [lozad.js](https://github.com/ApoorvSaxena/lozad.js). In order to make it work, you'll need to use pixboost bundle \(see [Usage](lazy-loading.md#usage) section\) or add the library with polyfill for the [Intersection Observer](https://github.com/w3c/IntersectionObserver/) feature if you want to have support in all browsers:

```markup
    <script type="text/javascript" src="https://pixboost.com/libs/intersection-observer.min.js"></script>
    <script type="text/javascript" src="https://pixboost.com/libs/lozad.min.js"></script>
```

WARNING: In case of using polyfill make sure that you test your application in all browsers. We found some issues in IE \(before Edge\) and Safari with absolute positioning when using polyfill.

