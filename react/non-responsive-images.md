# Non-responsive images

There is an `Image` component that you can use to render a standard image.

Example:

```javascript
    //This is a reusable configuration
    const pixboostConfig = {
        apiKey: 'MTg4MjMxMzM3MA__',
        domain: 'pixboost.com'
    };

    class YourComponent extends Component {
        render() {
            return (
                <Image src={'https://cdn.pixabay.com/photo/2016/05/10/15/29/bear-1383980_960_720.jpg'}
                       alt={'lazy bear'}
                       config={pixboostConfig}
                       op={'resize?size=200'}
                />
            )
        }
    }
```

Properties \(mandatory properties marked with \*\):

| Property | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| src\* | String |  | URL of the original image |
| config\* | Object |  | Configuration |
| alt | String |  | alt text for an image |
| lazy | Boolean | true | If true, then will enable lazy loading for the image. |

