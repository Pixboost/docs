# As is

API endpoint - `/api/2/img/[IMAGE-URL]/asis`

## Description

**Asis** - does not perform any transformations. Respond with the original image without any modifications. Would be useful to leverage CDN.

## Parameters

No parameters required.

### Examples

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| ![](http://www.midday.coffee/assets/cup.jpeg) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ\_\_) |

### Sandbox

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| [www.midday.coffee/assets/cup.jpeg](www.midday.coffee/assets/cup.jpeg) | [http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=200x100&auth=MTA0ODU5NDA0NQ\_\_](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__)\_ |

