SilverStripe Salesforce Authentication Module
=============================================

This module provides an authenticator which uses the Salesforce OAuth
authentication service.

Installation
------------

* Create an OAuth enabled external application in the Salesforce control
  panel through the Create / Apps section.
* Set the Callback URL to `https://<your-site>/salesforce-auth/callback`,
  ensuring you use a HTTPS scheme.
* Configure the `SalesforceAuth` service, for example using the configuration
  file show below.

```yaml
Injector:
  SalesforceAuth:
    constructor:
      - '<client_id>'
      - '<client_secret>'
```
