# API. JavaScript Integration

You can integrate Pixboost into web app/site that that has direct access to the DOM, e.g. jQuery, Backbone. This  
solution won't work well with frameworks that using shadow DOM, e.g. React, AngularJs.

Some benefits of using library over directly editing HTML and adding `picture`/`img` tags:

* You can disable optimised images for the whole website or you can enable it conditionally by cookie
* Easy migration between domains
* One place to setup API key
* No need to manage mobile breakpoints in the code

The library is open source and hosted on [github](https://github.com/Pixboost/pixboost-js).

Table of Contents:

* Usage
  * [Installation](install.md)
  * [Responsive images](responsive-images.md)
  * [Non-responsive images](not-responsive-images.md)
  * [CSS Background images](css-background-images.md)
  * [Lazy Loading](lazy-loading.md)
  * [Replacing on Document Load](replacing-on-document-load.md)
  * [Custom Domain Name](custom-domain-name.md)
  * [Reloading](reloading.md)
  * [Disabling](disabling.md)
* [Browsers Support](browsers-support.md)

