# Proxy middleware standard (do not read this)

This is not finished

## Manifest

Unlike the previous aero-only middleware, files will be included through routes in the manifest.json. Additionally the optional Lib/get.ts from that time will still exist, but the assets must be routed as well. The [cosmetic metadata](https://developer.chrome.com/docs/extensions/reference/manifest) from chrome extensions will be nearly the same. Providing this metadata will help middleware frontents like [mine](https://hedge.soundar.eu.org/s/ZKz3GJV65#Storefront).

## Packaging

Middleware will be packaged with tar.gz.

## Shadow middleware

APIs will be provided in each ctx, that lets you create "fake middleware". Although this might seem strange, it has its uses. This lets you register your own middleware runtimes ontop of the minimal standard. This will have all the properties of a real middleware. The main reason why this exists is because of "middleware bridges", which are ports of alternative middleware systems to this lightweight standard. For example, I am building [one for PHP-Proxy](https://hedge.soundar.eu.org/s/o1WQpIBc3#).
