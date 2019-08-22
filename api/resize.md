# Resize

API endpoint - `/api/2/img/[IMAGE-URL]/resize?size=[NEW-SIZE]`

## Description

**Resize** - resizes image with preserving aspect ratio and optimizes it using lossy compression. If you need the exact size then use fit operation.

## Parameters

**size** - new size \(in pixels\) of the image in the format `WIDTH and xHEIGHT`.

You can specify only one dimension and the second will be calculated according to aspect ratio of the image.

### Examples

| Options | Original | After |
| :--- | :---: | :---: |
| size=200 | ![](http://www.midday.coffee/assets/cup.jpeg) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200&auth=MTg4MjMxMzM3MA__) |
| size=x80 | ![](http://www.midday.coffee/assets/cup.jpeg) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=x80&auth=MTg4MjMxMzM3MA__) |

### Sandbox

Please, feel free to test this in your browser to see how it works.

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| [www.midday.coffee/assets/cup.jpeg](https://github.com/dmitrypokidov/pixboost/tree/c6f1ddd25e878d9100600d2df063f6910794593f/www.midday.coffee/assets/cup.jpeg) | [http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200x100&auth=MTg4MjMxMzM3MA\_\_](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200x100&auth=MTg4MjMxMzM3MA__) |

