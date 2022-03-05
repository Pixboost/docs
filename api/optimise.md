# Optimise

API endpoint - `/api/2/img/[IMAGE-URL]/optimise`

## Description

**Optimise** - optimises images using lossy compression automatically.

## Parameters

No parameters required.

### Examples

| Original | After |
| :---: | :---: |
| ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/optimise?&auth=MTA0ODU5NDA0NQ__) |

In the example above an image becomes at least 20% lighter

### Sandbox

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| [www.midday.coffee/assets/cup.jpeg](https://github.com/Pixboost/docs/tree/8f93cdfa3e5fdb7584ce488ef51153268bef537f/api/www.midday.coffee/assets/cup.jpeg) | [http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/optimise?&auth=MTA0ODU5NDA0NQ\_\_](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/optimise?&auth=MTA0ODU5NDA0NQ__) |

