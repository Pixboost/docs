# Cache Invalidation

API endpoint - `DELETE /api/2/img/[IMAGE-URL]?auth=[API_SECRET]`

## Description

This a service endpoint that allows you to invalidate images cached on CDN.

We recommend that you use invalidation sparingly and only as a last resort. For example, invalidation is useful when you must remove content for legal reasons or because of an accidental upload. Otherwise, we recommend that you use versioning whenever possible or wait until the content expires normally.

Calling example using curl:

```text
curl -X DELETE 'https://pixboost.com/api/2/img/http://www.midday.coffee/banner.jpeg?auth=ABCDEF'
```

## Limitations

Invalidation is intended for use in exceptional circumstances, not as part of your normal workflow. Importantly, invalidations don't affect cached copies in web browser caches or caches operated by third-party Internet service providers.

Invalidations are rate limited. You can submit at most one invalidation per minute.

## Parameters

API\_SECRET - secret key. This secret key is not public and _should not_ be shared.

