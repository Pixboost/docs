# API. URL-based integration

To make integration easier we provide a lightweight API that you can directly use from HTML code.

## URL pattern for API call

All endpoints follow the same pattern

`https://pixboost.com/api/2/img/[IMAGE_URL|IMAGES_SOURCE_ALIAS_WITH_PATH]/[OPERATION]?[OPERATION_PARAMS]&auth=[API_KEY]`

| Item                                      | Description                                                               |
|:------------------------------------------|:--------------------------------------------------------------------------|
| **\[IMAGE\_URL\]**                        | The URL of the original image you would like to process through Pixboost. |
| **\[IMAGES\_SOURCE\_ALIAS\_WITH\_PATH\]** | An alias of an images source with relative path to the image.             |
| **\[OPERATION\]**                         | Pixboost function call                                                    |
| **\[OPERATION\_PARAMS\]**                 | Operation parameters for a function call you are using                    |
| **\[API\_KEY\]**                          | A unique [API key](../setup/manage-api-keys.md)                           |

### Example using **&lt;img&gt;** tag

Before:

`<img src="http://www.midday.coffee/assets/cup.jpeg" alt="Midday Coffee">`

After:

`<img src="http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200x100&auth=MTg4MjMxMzM3MA__" alt="Midday Coffee">`

### Example using **&lt;picture&gt;** tag

Before:

```markup
<picture>
    <source srcset="http://www.midday.coffee/assets/cup.jpeg" 
        media="(min-width: 769px)">
    <source srcset="http://www.midday.coffee/assets/cup.jpeg" 
        media="(max-width: 768px)">
    <source srcset="http://www.midday.coffee/assets/cup.jpeg" 
        media="(max-width: 576px)">
    <img src="http://www.midday.coffee/assets/cup.jpeg">
</picture>
```

After:

```markup
<picture>
    <source srcset="https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/optimise?auth=API_KEY" 
        media="(min-width: 769px)">
    <source srcset="https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=300&auth=API_KEY" 
        media="(max-width: 768px)">
    <source srcset="https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=100x100&auth=API_KEY" 
        media="(max-width: 576px)">
    <img src="http://www.midday.coffee/assets/cup.jpeg">
</picture>
```

We support all transformation required for the typical website.

![](../.gitbook/assets/operations-diagram-aboutpage.png)

Read more on operations:

## [Resize](resize.md)

## [Fit](fit.md)

## [Optimise](optimise.md)

## [As is](as-is.md)

You can explore API sandbox here: [https://pixboost.com/docs/api/](https://pixboost.com/docs/api/)

