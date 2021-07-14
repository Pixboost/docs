# Automated Workflows

Workflows help you to automate certain tasks while managing your images using Pixboost service. Workflows consist of API endpoints that you could use from your applications. Currently, Pixboost supports the following endpoints:

* [Cache Invalidation](cache-invalidation.md)
* [Warmup](warmup.md)

To call a workflow API, you will need to create an API secret first. Please, read about creating and managing API secrets [here](api-secrets.md).

Example of the workflow could be a CDN cache invalidation when a source image updated. You can find a reference implementation of such a scenario [here](https://github.com/Pixboost/aws-s3-invalidate-cdn)

![](../.gitbook/assets/cache-invalidation-ref-implementation.svg)

## Pricing

There is a limitation in number of calls that you allowed to do that depends on the selected plan. Please, refer to the [pricing page](../billing.md) to see the exact numbers.

