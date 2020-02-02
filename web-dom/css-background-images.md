# CSS Background images

[Background images](https://css-tricks.com/almanac/properties/b/background-image/) are often used for hero banners or in cases where you need to put content on top of an image.

Below is a simple example of a hero banner:

```markup
<style>
    .hero {
        height: 600px;
        background-image: url("https://yoursite.com/hero.jpg");
        background-size: cover;
    }
</style>

<div class="hero" >
    <div class="content">This text is displayed on top of the image.</div>
</div>
```

In this example, we created hero banner and using "background-image" CSS rule to setup an URL for the image.

Using this library, you can optimise this image and also make it responsive. The syntax is exactly the same as for [responsive images](responsive-images.md), but instead of using `data-pb-picture` attribute you should use `data-pb-background`:

```markup
<style>
    .hero {
        height: 600px;
        background-size: cover;
    }
</style>

<div class="hero" 
    data-pb-background=""
    data-url="https://yoursite.com/hero.jpg"
    data-lg="optimise"
    data-md="resize?size=990"
    data-sm="resize?size=640">
</div>

    <div class="content">This text is displayed on top of the image.</div>
</div>
```

The snippet above renders 3 different sizes for different devices. We don't need `background-image` CSS rule anymore as it created by the library.

You can kick off optimisation by calling `background()` function or use [autoload](replacing-on-document-load.md):

```text
window.Pixboost.background({apiKey: 'API_KEY'})
```

Lazy loading is supported for background images as well.

