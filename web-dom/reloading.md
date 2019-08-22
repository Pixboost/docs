# Reloading

If you are fetching content using AJAX then you might want to run `picture()` and `image()` once requests finished.  
You can do this manually using `window.Pixboost.picture()` and `window.Pixboost.image()` call or you can trigger  
`pbUpdate` event:

```javascript
    var pbUpdateEvent = document.createEvent("Event");
    pbUpdateEvent.initEvent("pbUpdate", false, true);
    document.dispatchEvent(pbUpdateEvent);
```

## Custom reload events

The library supports native DOM events and JQuery. You can specify a list of events separated  
by the comma in `data-events` or `data-jquery-events` attributes. For example,

```text
    <script type="text/javascript" src="https://pixboost.com/libs/pixboost.js" 
            id="pb-script" 
            data-api-key="API_KEY"
            data-events="contentloaded"></script>
```

Then to trigger update:

```text
    var contentLoadedEvent = document.createEvent("Event");
    contentLoadedEvent.initEvent("contentloaded", false, true);
    document.dispatchEvent(contentLoadedEvent);
```

And with JQuery:

```text
    <script type="text/javascript" src="https://pixboost.com/libs/pixboost.js" 
            id="pb-script" 
            data-api-key="API_KEY"
            data-jquery-events="contentloaded"></script>
```

Then to trigger update:

```text
    $(document).trigger("contentloaded");
```

