# Supported Image Formats

Pixboost transforms and delivers PNG and JPEG images through CDN to the end user. This allowed provide highly optimized images for website needs.

We deliver default WebP format for Chrome and Opera browsers. And optimized PNG and JPEG images for other web browsers.

## WebP Format

### About

WebP is a method of **lossy** and **lossless** **compression** that can be used on a large variety of photographic, translucent and graphical images. WebP typically achieves an average of 30% more compression than JPEG and JPEG 2000, without loss of image quality.

### How it works

There is no need to setup this feature or do any coding to start using it. We decided to make it a **default option**, therefore it is already turned on automatically.

1. Browsers are sending special header called  **“Accept”** that tells server which formats it supports.
2. If browser supports WebP format then the header will have **“image/webp”** value.
3. When Pixboost sees this value will transform image to a new format. 

### How to avoid using WebP

If you would like to avoid using WebP transformation, please use [as-is option](https://help.pixboost.com/api/as-is.html).

### Browsers support

WebP lossy support:

* Google Chrome \(desktop\) 17+
* Google Chrome for Android version 25+
* Opera 11.10+
* Native web browser, Android 4.0+ \(ICS\)

WebP lossy, lossless & alpha support:

* Google Chrome \(desktop\) 23+
* Google Chrome for Android version 25+
* Opera 12.10+
* Native web browser, Android 4.2+ \(JB-MR1\)
* Pale Moon 26+

WebP Animation support:

* Google Chrome \(desktop and Android\) 32+
* Opera 19+

