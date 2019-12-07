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
| size=200 | ![](http://www.midday.coffee/assets/cup.jpeg) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200&auth=MTA0ODU5NDA0NQ\_\_) |
| size=x80 | ![](http://www.midday.coffee/assets/cup.jpeg) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=x80&auth=MTA0ODU5NDA0NQ\_\_) |

### Sandbox

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| [www.midday.coffee/assets/cup.jpeg](www.midday.coffee/assets/cup.jpeg) | [http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200x100&auth=MTA0ODU5NDA0NQ\_\_](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200x100&auth=MTA0ODU5NDA0NQ\_\_) |

