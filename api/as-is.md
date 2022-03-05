# As is

API endpoint - `/api/2/img/[IMAGE-URL]/asis`

## Description

**Asis** - does not perform any transformations. Respond with the original image without any modifications. Would be useful to leverage CDN.

## Parameters

No parameters required.

### Examples

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__) |

### Sandbox

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| [www.midday.coffee/assets/cup.jpeg](https://github.com/Pixboost/docs/tree/8f93cdfa3e5fdb7584ce488ef51153268bef537f/api/www.midday.coffee/assets/cup.jpeg) | [http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=200x100&auth=MTA0ODU5NDA0NQ\_\_](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__)\_ |

