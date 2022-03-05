# Resize

API endpoint - `/api/2/img/[IMAGE-URL]/resize?size=[NEW-SIZE]`

## Description

**Resize** - resizes image with preserving aspect ratio and optimizes it using lossy compression. If you need the exact size then use fit operation.

## Parameters

**size** - new size \(in pixels\) of the image in the format `WIDTH and xHEIGHT`.

You can specify only one dimension and the second will be calculated according to aspect ratio of the image.

### Examples

| Parameters | Original | After |
| :--- | :---: | :---: |
| size=200 | ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200&auth=MTA0ODU5NDA0NQ__) |
| size=x80 | ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=x80&auth=MTA0ODU5NDA0NQ__) |

### Sandbox

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| [www.midday.coffee/assets/cup.jpeg](https://github.com/Pixboost/docs/tree/a18a5ae66426629920df8220795d1a1ac414a5a0/api/www.midday.coffee/assets/cup.jpeg) | [http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200x100&auth=MTA0ODU5NDA0NQ\_\_](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200x100&auth=MTA0ODU5NDA0NQ__) |

