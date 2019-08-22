# HTTP/2 Support

Pixboost automatically supports HTTP/2 protocol. If the [browser supports HTTP/2](https://caniuse.com/#search=http%2F2) protocol, we deliver it accordingly.

HTTP/2 was created to improve efficiency of the existed HTTP protocol by including several features:

* it is binary, instead of textual
* is fully multiplexed, instead of ordered and blocking
* can therefore use one connection for parallelism
* uses header compression to reduce overhead
* allows servers to “push” responses proactively into client caches

This all makes it easier to deliver fast and efficient website. More on HTTP/2 protocol please read it's [official page](https://http2.github.io/).

