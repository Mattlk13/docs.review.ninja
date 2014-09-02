---
layout: default
title: ReviewNinja Environment Variables
---

Environment Variables
=====================

The following are the environment variables you have to configure to run a
private instance:

> *Pro Tip:* there is an example of these files in the root directory of the
> application called `.env.example` it contains preset variables suitable for
> development use.

`HOST`: Defaults to "review.ninja".

`PORT`: The local port to bind to. Defaults to 5000.

`PROTOCOL`: Valid options are "http" or "https". Defaults to "https".

`HOST_PORT`: This only needs to be set if it is a custom host port.  For
example, http and https are used but not on port 80 and 443.

`GITHUB_CLIENT`: Required. From your registered application in GitHub.

`GITHUB_SECRET`: Required. From your registered application in GitHub.

`GITHUB_PROTOCOL`: Valid options are "http" or "https". Defaults to "https".

`GITHUB_HOST`: Defaults to "github.com". 

> *Warning:* If this variable is set, it is assumed that GitHub Enterprise is
> used.

`GITHUB_API_HOST`: Defaults to "api.github.com".

`MONGODB`: Mandatory. This has to be in form of a mongodb url, e.g. `mongodb://<user>:<password>@<host>:<port>/<dbname>`.

`GACODE`: Optional. If this is not set, Google Analytics will not be recorded.

SMTP
----

> If `SMTP_HOST` is set, then all `SMTP_*` variables must be set. If
> `SMTP_HOST` is not set, then the systems's sendmail will be used.
 
 * `SMTP_HOST`: Host on which the SMTP Server runs on.
 * `SMTP_PORT`: Port on which the SMTP Server runs on.
 * `SMTP_SSL`: Use ssl or not, values are "true" or "false". Defaults to "true".
 * `SMTP_USER`: User on the SMTP Server.
 * `SMTP_PASS`: Password for the `SMTP_USER`.
