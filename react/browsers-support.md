# Browsers Support

The library supports all major browsers including Chrome, Firefox, Safari and Internet Explorer. Internet Explorer 9 requires polyfill for `<picture>` implementations. We are recommending to use [picturefill](http://scottjehl.github.io/picturefill/) version 3. You can include it from our CDN:

```markup
    <script src="https://pixboost.com/libs/picturefill.min.js" async></script>
```

Lazy loading is using [Intersection Observer](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API) feature that supports by all [major browsers](https://caniuse.com/#search=intersectionObserver) except Safari. You can use polyfill, but make sure that you are doing thorough testing as we found some problems with absolute positioned layouts.

