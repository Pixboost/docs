# Managing API Keys

**API Key** is a unique string that is used to secure your API access. Every API Key is globally unique and exists only in your account.

Once you [added at least one image source](adding-image-source.md) you will see the dashboard that will have "API Keys" section

![](../.gitbook/assets/api-keys-list.png)

You will already have one active API Key that you can start using straight away.

You'll need to pass an API Key in a query parameter called "**auth**" in the transformation URL. For example:

[https://pixboost.com/api/2/img/pixabay.com/logo.png/resize?size=200&\*\*auth=MTg4MjMxMzM3MA\](https://pixboost.com/api/2/img/pixabay.com/logo.png/resize?size=200&**auth=MTg4MjMxMzM3MA\)\_\*\*\_

You are able to delete and/or create new API Keys from the dashboard. You can use any API Key with any image source.

There is a soft limit on number of keys. You can have only 10 active keys. But don't hesitate to reach us on customer.service@pixboost.com if you need more than 10.

## Why you might need to have more than one API Key?

The most useful case is when you have more than one website/application that is using Pixboost.

**For example:**

Let's say you have two web sites: _**foo.com**_ and _**bar.com**_.

You have added both of them to the image sources.

Let's imagine that someone started using your transformed images from _**bar.com**_. We hope it would never happen though.

In case to prevent that you would need to create a new API key and start using it on _**bar.com**_. Once that done you can delete old API key.

If _**foo.com**_ is also using the old API key then you would need to change it there as well. But, if you use different API Keys in the first place then you won't need to change both of your websites.

