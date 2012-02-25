About
=================
CocoaRestClient is a Mac OS X app for testing HTTP/Restful endpoints. 

I love curl, but sometimes I need my output XML or JSON pretty printed. I want to be able to save frequent PUT and POST bodies for later and copy and paste from responses easily. Think of this as curl with a light UI. 

The goal of this project is to build a lightweight native Cocoa app for testing and debugging HTTP Restful services.
This project was greatly inspired by the Java rest-client (http://code.google.com/p/rest-client/). 

Features
=================
* Make GET, PUT, POST, DELETE, HEAD calls
* Set request body to arbitrary content
* Set request headers
* Set HTTP basic & digest auth
* Auto-format (pretty print) XML and JSON responses
* Display response headers
* Quick save requests in a handy drawer
* Send multipart/form-data
* Upload files via multipart/form-data
* Enter POST/PUT input as raw input or key/value pairs
* Reports response latency
* Command-R reloads last request
* Lightweight: Real memory usage hovers around 40MB
* Automatic updates
* SSL Support
* Optionally follows HTTP redirects
* Go full screen in Lion
* Import and export requests

Screenshots
=================

![Screenshot 1](https://github.com/mmattozzi/cocoa-rest-client/raw/master/screenshots/cocoa-rest-client-1.jpg)

*Pretty print XML content. Quick save of request URLs, body, and headers in one convenient drawer.*

![Screenshot 2](https://github.com/mmattozzi/cocoa-rest-client/raw/master/screenshots/cocoa-rest-client-2.jpg)

*Pretty print JSON content. Set and save HTTP headers.*

![Screenshot 3](https://github.com/mmattozzi/cocoa-rest-client/raw/master/screenshots/cocoa-rest-client-3.jpg)

*Set HTTP Basic or Digest Auth. Displays HTTP response headers.*

Source and Contributions
=================
* Source code is now hosted on Github: http://github.com/mmattozzi/cocoa-rest-client
* If you would like to contribute, please fork and create a pull request on Github 
* Downloads and issues will still be kept up to date on Google Code. I will probably keep source up to date with each release.
* I don't plan on switching from Garbage Collection to ARC until I drop 10.6 support, as there seems to be some [limitations with ARC on 10.6](http://stackoverflow.com/questions/7696201/how-to-deploy-to-snow-leopard-with-arc-enabled)
* I am not turning on AutoLayout constraints in my xib files until I drop 10.6 support.

Credits
=================
* Contains json-framework/SBJSON library (http://code.google.com/p/json-framework/) embedded in it, source and all
* Mucho guidance from Open Kosmaczewski blog (http://kosmaczewski.net/2008/03/26/playing-with-http-libraries/)
* Multipart features contributed by Adam Venturella
* Sparkle automatic update framework (https://github.com/andymatuschak/Sparkle)