# Resize

API endpoint - `/api/2/img/[IMAGE-URL]/resize?size=[NEW-SIZE]`

## Description

**Resize** - resizes image with preserving aspect ratio and optimizes it using lossy compression. If you need the exact size then use fit operation.

## Parameters

**size** \(**required**\) - new size (in pixels) of the image in the format `WIDTH and xHEIGHT`.

**dppx** \(optional\) - Number of dots per pixel defines the ratio between device and CSS pixels. The query parameter is a hint that enables extra optimisations for high density screens. The format is a float number in the same format as window.devicePixelRatio.


You can specify only one dimension and the second will be calculated according to the image's aspect ratio.

### Examples

* `size=200` - resize to 200 px wide preserving aspect ratio
* `size=x80` - resize to 80 px high preserving aspect ratio
* `dppx=2` - sending a hint to the API that screen has DPI=2

| Parameters        |                                                           Image                                                           | 
|:------------------|:-------------------------------------------------------------------------------------------------------------------------:|
| Original          |          ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__)          |
| size=200          |  ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200&auth=MTA0ODU5NDA0NQ__)   |
| size=x80          |    ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=x80&auth=MTA0ODU5NDA0NQ__)     |
| size=200&dppx=2   | ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/resize?size=200&dppx=2&auth=MTA0ODU5NDA0NQ__) |

###### You can see URL of the examples by "right-click -> Copy Image address"