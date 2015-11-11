---
layout: post
title:  "How the internet works"
date:   2015-11-10 19:00:00
categories: networks internet learning
---

##Networking


Understanding the 'series of tubes' that make up the internet is an important aspect of becoming a web developer. 

## The internet is not a cloud, it is a global series of interconnected networks

Servers connect to networks via fiber optics, satellite, or even via cell phones. All of the networks work together using **TCP/IP** (Transmission Control Protocol / Internet Protocol). 

TCP/IP provides standardized rules for how data should be transmitted, routed, and received. 

Web application development 'stands on the shoulders of giants.' Web devs largely deal with **HTTP** or Hyper Transfer Protocol.

##HTTP Verbs

The most popular HTTP/1.1 request methods are `GET`, `POST`, `PUT`, `DELETE`, although there are also methods for `TRACE`, `OPTIONS`, `CONNECT`, and `HEAD`. 

Most web applications use `GET` and `POST` to update and create content values. 

`GET` - Retrieves content from an existing resource.

`POST` - Submits a request to an existing resource and updates an existing resource.

As a web developer it is also important to be familiar with `PUT` and `DELETE`.

`PUT` - Creates a new resource defined at the specified Uniform Resource Identifier (URI). The most common form of URI is the Uniform Resource Locator or URL.

`DELETE` - Removes the resource specified at the URI.

###HTTP Status Codes
HTTP uses a collection of three-digit codes to easily parse what has happened to a request.

**5XX** - Server error

**4XX** - Couldn't complete request, but there wasn't an error

**3XX** - Further action needs to be taken by the user in order to fill request

**2XX** - Request was successfully recieved, understood, and accepted

**1XX** - Getting what you want, keep going
##Sending requests in terminal
###cURL
cURL is a terminal program that can send requests and recieve responses. 

A sample `GET` request:
	
	curl -X GET 'http://www.google.com'

The `GET` request shown in <http://www.explainshell.com>:
![](http://i.cubeupload.com/fbRhrZ.png)
	
	
##Postman
In the Galvanize Full Stack Program we are using [Postman](https://www.getpostman.com/) to help us work with APIs. It allows you to quickly send, save, and test requests.

A sample `GET` request:

	GET  HTTP/1.1
	Host: www.google.com
	Cache-Control: no-cache
A sample response:

	alternate-protocol → 443:quic,p=1
	cache-control → private, max-age=0
	content-encoding → gzip
	content-type → text/html; charset=UTF-8
	date → Wed, 11 Nov 2015 23:34:00 GMT
	expires → -1
	server → gws
	status → 200
	x-frame-options → SAMEORIGIN
	x-xss-protection → 1; mode=block