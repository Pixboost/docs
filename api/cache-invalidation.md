# Cache Invalidation

API endpoint - `DELETE /api/2/img/[IMAGE-URL]?auth=[API_SECRET]`

## Description

Cache invalidation a service endpoint that allows you to invalidate images cached on CDN.

Calling example using curl:

```text
curl -X DELETE 'https://pixboost.com/api/2/img/http://www.midday.coffee/banner.jpeg?auth=ABCDEF'
```

## Parameters

API\_SECRET - [secret key](../workflows/api-secrets.md).

## Example

You can find reference example of using cache invalidation workflow with S3 bucket [here](https://github.com/Pixboost/aws-s3-invalidate-cdn).

## Limitations

Please, be aware that invalidations don't affect cached copies in web browser caches or caches operated by third-party Internet service providers.

In most cases, using versioning on file names is a better option.

