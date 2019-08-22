# Responsive images

The library provides `Picture` component that will render different size images for different visual breakpoints.

Below is a simple example:

```javascript
    //This is a reusable configuration
    const pixboostConfig = {
        apiKey: 'MTg4MjMxMzM3MA__',
        domain: 'pixboost.com',
        breakpoints: {
            lg: {media: '(min-width: 990px)'},
            md: {media: '(min-width: 640px)'},
            sm: {}
        }
    };

    class YourComponent extends Component {
        render() {
            return (
                <Picture alt={"gadgets"} breakpoints={
                    {
                        lg: {
                            //Will optimise image by default
                            src: 'https://cdn.pixabay.com/photo/2015/01/21/14/14/apple-606761_960_720.jpg'
                        },
                        md: {
                            src: 'https://cdn.pixabay.com/photo/2015/02/02/15/28/bar-621033_960_720.jpg',
                            op: 'fit?size=300x300'
                        },
                        sm: {
                            //We can hide image for certain breakpoints
                            hide: true
                        }
                    }
                } config={pixboostConfig}/>
            )
        }
    }
```

Properties \(mandatory properties marked with \*\):

| Property | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| breakpoints\* | Object |  | Object that sets an option for each visual breakpoint. You can use only breakpoints that you specified in the configuration property |
| breakpoints.src\* | String |  | URL of the original image |
| breakpoints.op | String | optimise | Operation to perform. By default is optimise. |
| breakpoints.hide | Boolean | false | If true then will hide image on the breakpoint. |
| config\* | Object |  | Configuration |
| alt | String |  | alt text for an image |
| lazy | Boolean | true | If true, then will enable lazy loading for the picture. |

