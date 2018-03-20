alpine-revealjs
===============

This image is [reveal.js][reveal.js] base. It comes from [alpine-nginx][alpine-nginx].

## Build

```
docker build -t rawmind/alpine-revealjs:<version> .
```

## Versions

- `3.6.0-0` [(Dockerfile)](https://github.com/rawmind0/alpine-revealjs/blob/3.6.0-0/Dockerfile)

## Usage

This image runs [reveal.js][reveal.js] web server at port 8080.

```
docker run -td -p 8080:8080 rawmind/alpine-revealjs:<version>
```

### Default Configuration

You get access to default [reveal.js][reveal.js] demo 

### Custom Configuration

- Use this image `FROM rawmind/alpine-revealjs:<version>` at the top of your `Dockerfile`. 
- Overwrite default [reveal.js][reveal.js] `/opt/nginx/www/reveal.js/index.html` file with own.
- Add your slides under `/opt/nginx/www/reveal.js/slides` folder.

[alpine-nginx]: https://github.com/rawmind0/alpine-nginx/
[reveal.js]: https://github.com/hakimel/reveal.js
