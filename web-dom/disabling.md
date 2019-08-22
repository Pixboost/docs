# Disabling

You can globally disable URL transformations using `data-disabled` attribute.

```markup
    <script type="text/javascript" src="https://pixboost.com/libs/pixboost.js" 
        id="pb-script" 
        data-api-key="API_KEY"
        data-disabled></script>
```

## Enabling by cookie

Sometimes you would want to enable optimized images only if cookie presents. This is useful  
if you are using Optimizely or other AB testing services, so you can turn on optimization for a small amount  
of your customers in the beginning and increase it through time.

```markup
    <script type="text/javascript" src="https://pixboost.com/libs/pixboost.js" 
        id="pb-script" 
        data-api-key="API_KEY"
        data-cookie-enable="optimized-images"></script>
```

Value of the cookie must be set to `true`.

