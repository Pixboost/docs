# Not responsive images

You can use library with `<img>` tag as well. Below is an example of image that will be replaced with optimised  
version:

```markup
<img data-op="resize?size=x600" data-src="https://yoursite.com/doggy.png" data-pb-image/>
```

To process all images:

```javascript
    window.Pixboost.image({apiKey: 'API_KEY'})
```

