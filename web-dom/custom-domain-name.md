# Custom Domain Name

If you have [custom domain name](https://help.pixboost.com/setup/custom-domain.html) setup then you can pass domain to the script tag using `data-domain` attribute:

```markup
    <script type="text/javascript" src="https://pixboost.com/libs/pixboost.js" 
        id="pb-script" 
        data-api-key="API_KEY"
        data-domain="static.yoursite.com"
        data-autoload></script>
```

Or you can pass it to a picture\(\) call:

```javascript
  window.Pixboost.picture({apiKey: 'API_KEY', domain: 'static.yoursite.com'})
```

