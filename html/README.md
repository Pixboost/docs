# Using in HTML

In this section we'll look at how to use Pixboost in the HTML markup and
what are some of the best practices.

We will use [Pixboost API](../api) for optimising and resizing image for different types of screens.

## Simple image

Let's start from the simple image that will always display the same on any devices:

```html
<img 
    src="https://pixboost.com/api/2/img/middaycoffeeimages/coffee.jpeg/optimise?auth=NDEzMTQ0NTY2Ng__"
    
    width="1333"
    height="2000"

    alt="coffee machine is filling in a cup"

    fetchpriority="high"

    loading="eager"
/>
```

Let's go through the attributes:

`src` - we use [optimise](../api/optimise.md) endpoint with [http alias](../setup/source-images/http.md). The original image [can be found here](http://www.midday.coffee/assets/coffee.jpeg). TODO: size comparison

`width` and `height` - these are the sizes of the original image and a browser can use them to calculate aspect ratio and prepare enough space on the page to render it. If we don't specify them then we can see the content "jumping" around the page before the image loaded which is harmful for the User Experience. It's also will contribute to Cumulative Layout Shift metric that is tracked as part of [Web Vitals](https://web.dev/vitals/) set of metrics

`alt` - alt attribute is a description of the image and important for accessibility, so screen readers can let the user know what's on the image. Also, a browser shows the description if it couldn't load the image for some reason.

`fetchpriority` is a relatively new addition which is still experimental and not supported in all browsers. It's extremely useful for hero banners and images that you'd need to load first or can be loaded later. The attribute values can be: `high`, `low` or `auto` (default.)

`loading` attribute 

