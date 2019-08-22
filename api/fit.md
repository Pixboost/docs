# Fit

API endpoint - `/api/2/img/[IMAGE-URL]/fit?size=[NEW-SIZE]`

## Description

**Fit** - resizes image, crops it to the size and optimises it using lossy compression. If you need to resize image with preserved aspect ratio then use [resize operation](https://help.pixboost.com/api/resize.html).

## Parameters

**size** - new size \(in pixels\) of the image in the format `WIDTHxHEIGHT`.

You have to specify both dimensions \[width\] and \[height\].

### Example

size =`200x100 (scaling by the smaller side which is height, cropping sides, center positioning)`

| Options | Original | After |
| :--- | :---: | :---: |
| size=200x100 | ![](http://www.midday.coffee/assets/cup.jpeg) | ![](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=200x100&auth=MTg4MjMxMzM3MA__) |

### Sandbox

| Original Image | Image after Pixboost transformation |
| :--- | :--- |
| [www.midday.coffee/assets/cup.jpeg](https://github.com/dmitrypokidov/pixboost/tree/c6f1ddd25e878d9100600d2df063f6910794593f/www.midday.coffee/assets/cup.jpeg) | [http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=200x100&auth=MTg4MjMxMzM3MA\_](http://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=200x100&auth=MTg4MjMxMzM3MA__)\_ |

