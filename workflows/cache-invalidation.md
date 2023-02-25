# Cache Invalidation

API endpoint - `DELETE /api/2/img/[IMAGE-URL]?auth=[API_SECRET]`

## Description

Cache invalidation invalidates images cached on CDN and Pixboost 2nd level cache.

Example:

```bash
curl -X DELETE 'https://pixboost.com/api/2/img/http://www.midday.coffee/banner.jpeg?auth=ABCDEF'
```

## Parameters

API\_SECRET - [secret key](api-secrets.md).

## Response

200 - Image has been invalidated.

202 - Invalidation process began and will finish soon. Usually it will take up to the 5 minutes.

401 - Failed authorization. Image domain is not in the list of [images sources](../setup/source-images/domain.md)

## Example

You can find reference example of using cache invalidation workflow with S3 bucket [here](https://github.com/Pixboost/aws-s3-invalidate-cdn).

## Limitations

Please, be aware that invalidations don't affect cached copies in web browser caches or caches operated by third-party Internet service providers.

In most cases, using versioning on file names is a better option.

