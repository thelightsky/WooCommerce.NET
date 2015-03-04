﻿WooCommerce.NET
======================

A Brief Intro
-------------------

WooCommerce.NET is a .NET library for calling WooCommerce REST API v2 in Windows 8.1 APP, Windows Phone 8.1 APP, Windows Desktop APP and ASP.NET Web application.

[Visit WooCommerce](http://www.woothemes.com/woocommerce/)
[Visit WooCommerce REST API](http://woothemes.github.io/woocommerce-rest-api-docs/)

If you have any question or would like to contribute code, please email to xiaofaye@msn.com.

Usage
-------------------

```cs
RestAPI rest = new RestAPI("http://www.yourstore.co.nz/wc-api/v2/", "<WooCommerce Key>", "<WooCommerce Secret");
WCObject wc = new WCObject(rest);
var products = await wc.GetProducts();
```

Version History
-------------------
* v0.2.1 Minor update (4/03/2015)
  1. Fix HMAC-SHA256 bug.
* v0.2.0 Minor update
  1. Add support for Windows Desktop application and Web application.
* v0.1.1 Minor update
  1. Use the same way to trim json string.
  2. Implement Customer Download call.
  3. Implement Order Refund call.
* v0.1 First working version
  1. Implement only GET method for most REST API calls.
  2. Supports WooCommerce REST API version 2.