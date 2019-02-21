# Icotar
## Colorful Icon Avatars
Icotar generates simple, playful avatars for your app or website. Based on the lovable avatars from Yik Yak, each avatar consists of a colorful background and a recognizable symbol. All colors and icons are hand-picked from [Material Design](https://material.io/).

Setting up Icotars is easy with a simple and free HTTP API that you can use without an account!

### How to Use Icotar
Icotar images may be requested just like a normal image. Our HTTP-API is based on the system built by the fine folks of Gravatar.

#### Base Request
The most basic image request URL looks like this:
```
https://icotar.com/avatar/:hash
```
Where `:hash` is replaced with anything you like. But **don't** use any sensitive or personal data here! For example, here is a base URL:
```
https://icotar.com/avatar/craig
```
![craig](https://icotar.com/avatar/craig "Craig")

#### File Types
All avatars are served as SVG files by default. If you require a **file-type extension** then you can add an optional `.svg` extension to that URL:
```
https://icotar.com/avatar/craig.svg
```
Icotar also supports PNG files:
```
https://icotar.com/avatar/craig.png
```

#### Size
By default, PNG images are presented at 80px by 80px if no size parameter is supplied. You may request a specific image size, which will be dynamically delivered from Icotar by using the `s=` or `size=` parameter and passing a single pizel dimension (since Icotars are square):
```
https://icotar.com/avatar/craig.png?s=200
```
![craig](https://icotar.com/avatar/craig?s=20 "Craig")
![craig](https://icotar.com/avatar/craig?s=80 "Craig")
![craig](https://icotar.com/avatar/craig?s=200 "Craig")

You may request images anywhere from **1px up to 1024px**.

#### Secure Requests
All URL requests should start with HTTPS.

##### Made with ❤️ by [Six Overground](http://sixoverground.com)