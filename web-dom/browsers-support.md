# Browsers Support

The library supports all major browsers including Chrome, Firefox, Safari and Internet Explorer. Internet Explorer 9 requires polyfill for `<picture>` and `matchMedia` implementations. For picture support, we are recommending to use [picturefill](http://scottjehl.github.io/picturefill/) version 3. Pixboost-js has integration with it and will call `window.picturefill()` once replacements are done. For matchMedia, we highly recommend [matchMedia.js](https://github.com/paulirish/matchMedia.js).

Lazy loading is using [Intersection Observer](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API) feature that supports by all [major browsers](https://caniuse.com/#search=intersectionObserver) except for Safari. You can use polyfill, but make sure that you are doing thorough testing \(see more details in [lazy loading](lazy-loading.md) section\).

