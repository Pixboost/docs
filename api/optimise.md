# Optimise

API endpoint - `/api/2/img/[IMAGE-URL]/optimise`

## Description

**Optimise** - optimises images using lossy compression automatically.

## Parameters

**dppx** \(optional\) - Number of dots per pixel defines the ratio between device and CSS pixels. The query parameter is a hint that enables extra optimisations for high density screens. The format is a float number in the same format as window.devicePixelRatio.

### Examples

* `dppx=2` - sending a hint to the API that screen has DPI=2

| Parameters    |                                                       Image                                                        | 
|:--------------|:------------------------------------------------------------------------------------------------------------------:|
| Original      |      ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/asis?auth=MTA0ODU5NDA0NQ__)       |
| No parameters |    ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/optimise?auth=MTA0ODU5NDA0NQ__)     |
| dppx=2        | ![](https://pixboost.com/api/2/img/http://www.midday.coffee/assets/cup.jpeg/optimise?dppx=2&auth=MTA0ODU5NDA0NQ__) |

###### You can see URL of the examples by "right-click -> Copy Image address"
