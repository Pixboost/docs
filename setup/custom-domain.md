# Custom Domain Name

By default, API is accessible on pixboost.com domain, but you can easily use your own.

It just 3 simple steps:

* Create a new DNS record for the subdomain. For instance, to use _**static.foo.com**_ 

  domain you will need the following DNS record:

| Type | Subdomain | Canonical Name |
| :--- | :--- | :--- |
| CNAME | static | pixboost.com. |

DNS changes can take some time to apply. You can test DNS change by loading subdomain in the browser. Enter static.foo.com in the location bar and you should see pixboost website.

* Write us an email on **customer.service@pixboost.com**, so we could issue a SSL certificate for a new domain.
* You can start accessing API on _**static.foo.com**_ instead of _**pixboost.com.**_ Once SSL certificate and DNS change is done

