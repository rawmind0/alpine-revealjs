[![](https://images.microbadger.com/badges/image/rawmind/alpine-revealjs.svg)](https://microbadger.com/images/rawmind/alpine-revealjs "Get your own image badge on microbadger.com")

alpine-revealjs
===============

This image is [reveal.js][reveal.js] base. It comes from [alpine-nginx][alpine-nginx].

## Build

```
docker build -t rawmind/alpine-revealjs:<version> .
```

## Versions

- `3.6.0-1` [(Dockerfile)](https://github.com/rawmind0/alpine-revealjs/blob/3.6.0-1/Dockerfile)

## Usage

This image runs [reveal.js][reveal.js] web server at port 8080.

```
docker run -td -p 8080:8080 rawmind/alpine-revealjs:<version>
```

### Default Configuration

You get access to default [reveal.js][reveal.js] demo 

### Custom Configuration

- Use this image as base at your dockerfile `FROM rawmind/alpine-revealjs:<version>`. 
- Add your slides under `/opt/nginx/www/reveal.js/slides` folder.
- Overwrite default index file with your own `/opt/nginx/www/reveal.js/index.html` .

[alpine-nginx]: https://github.com/rawmind0/alpine-nginx/
[reveal.js]: https://github.com/hakimel/reveal.js
