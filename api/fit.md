# Fit

API endpoint - `/api/2/img/[IMAGE-URL]/fit?size=[NEW-SIZE]`

## Description

**Fit** - resizes, crops, and optimises source image. This operation does not respect original aspect ratio. 
If you need to preserve aspect ratio then use [resize operation](./resize.md).

## Parameters

**size** \(**required**\) - new size \(in pixels\) of the image in the format `WIDTHxHEIGHT`.  You have to specify **both** dimensions width and height.

**dppx** \(optional\) - Number of dots per pixel defines the ratio between device and CSS pixels. The query parameter is a hint that enables extra optimisations for high density screens. The format is a float number in the same format as window.devicePixelRatio.

**trim-border**\(optional\) - Will remove the edges of the image with the same color, if the option specified.

### Examples

* `size=200x100` - scaling by the smaller side which is height, cropping sides, center positioning
* `dppx=2` - sending a hint to the API that screen has DPI=2

| Parameters               |                                                                         Image                                                                          | 
|:-------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------:|
| Original                 |                        ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__)                         |
| size=200x100             |                  ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=200x100&auth=MTA0ODU5NDA0NQ__)                   |
| size=200x100&dppx=2      |               ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/fit?size=200x100&dppx=2&auth=MTA0ODU5NDA0NQ__)               |
| Original                 |             ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cups/keep-calm-2816357__340.jpg/asis?auth=MTA0ODU5NDA0NQ__)             |
| size=200x200&trim-border | ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cups/keep-calm-2816357__340.jpg/fit?size=200x200&trim-border&auth=MTA0ODU5NDA0NQ__) |
| size=200x200             |       ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cups/keep-calm-2816357__340.jpg/fit?size=200x200&auth=MTA0ODU5NDA0NQ__)       |

###### You can see URL of the examples by "right-click -> Copy Image address"