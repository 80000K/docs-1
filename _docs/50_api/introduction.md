---
title: API Introduction
menu: Introduction
category: api
category_order: 9
order: 1
permalink: /api
---

There are a few ways to interact with our API. We have the stats API for basic stats and the business API for changing users, websites and other settings.

## Stats API

Use this if you want to retrieve aggregated stats from your website. Basically the stats you see in your dashboard (for now only page views, later we add referrals and others).

Some websites are set to public while others are set to private. You can manage this in your website settings. If your website is set to public you can get the JSON data without any credentials.

You can set the JSON format by adding `.json` to the URL of Simple Analytics. For example for our website it will be [`https://simpleanalytics.io/simpleanalytics.io.json`](https://simpleanalytics.io/simpleanalytics.io.json). You can add *start* and *end* dates to the URL as well like [`https://simpleanalytics.io/simpleanalytics.io.json?start=2019-01-01&end=2019-01-31`](https://simpleanalytics.io/simpleanalytics.io.json?start=2019-01-01&end=2019-01-31).

If you have your website set to private you can still export this data. You need to authenticate yourself. [See here how to authenticate](/api/authenticate).

### Get data for specific pages

With the stats API you can also retrieve data for a specific page of your website. By adding the path to the URL Simple Analytics returns the data for that path. For example if you want to know how many visits you got on `simpleanalytics.io/contact`, you can get the JSON with this URL: [`https://simpleanalytics.io/simpleanalytics.io/contact.json`](https://simpleanalytics.io/simpleanalytics.io/contact.json))

## Business API

Use this if you want to administer your account.

With this API you can for example add websites to your dashboard. This API is only available on request because we want to know what the use case for the API will be. Just drop us a line via [our contact page](https://simpleanalytics.io/contact?ref={{ site.hostname }}).

### Custom endpoints

For bigger customers we make custom endpoints. If you are in the need of a custom endpoint, [let us know](https://simpleanalytics.io/contact?ref={{ site.hostname }}).
