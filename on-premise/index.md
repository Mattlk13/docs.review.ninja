---
layout: default
title: On Premise
---
<h1>On Premise</h1>

<h1 id="installation">Installation</h1>

We use salt provisioning to get you installed and ready to go as hassle-free as possible.  

Set up the environment
----------------------

Prerequisites:

  * NodeJS
  * MongoDB
  * Linux or Mac OSX

Basic steps:

  1. Install Node
  2. Install MongoDB
  3. Create MongoDB user
  4. Create MongoDB database 
  4. Install ReviewNinja
 
Clone this repository:

	git clone https://github.com/reviewninja/review.ninja.git

The app is located in `/home/review.ninja`.  

	cd ~/review.ninja

Install npm and bower dependencies:

	npm install
	bower install

To configure the application, copy the `.env.example` file to `.env`:

	cp .env.example venv

You need to [register the application on
GitHub](https://github.com/settings/applications/new). The callback is
http://localhost:5000/auth/github/callback.  Fill out the name and homepage 
as you wish.

Set the `GITHUB_CLIENT` and `GITHUB_SECRET` environment variables accordingly in the `.env` file.

The following environment variables are mandatory: 

  * `MONGODB`
  * `GITHUB_CLIENT`
  * `GITHUB_SECRET` 

The `MONGODB` default in the `.env.example` file is correct unless you have an alternative configuration.

Once that is done you can start the application with:

	npm app.js
	

Contribute to this repo
-----------------------

Any feedback or contributions on customizations are very welcome.

If you like any other provisioning provider better and can contribute your
script, feel free to open an issue and we are happy to create a repository for
it.

<h1 id="variables">Environment Variables</h1>

The following are the environment variables you have to configure to run a
private instance:

> **Pro Tip:** there is an example of these files in the root directory of the
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
