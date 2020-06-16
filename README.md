# Stremio Static Add-on Example

This repository is an example of static add-ons for Stremio.

## Testing locally

When testing locally, you can use a local server, but it's really important that you set the cache times to very low values (or 0) so that caching does not interfere with your development. Enabling CORS is also needed.

For example, with `http-server` from npm:

```
PORT=8081 http-server dist --cors -c-1
```

## Using with GitHub Pages

You can test this example add-on by adding the GitHub Pages URL:

`https://stremio.github.io/stremio-static-addon-example/manifest.json`

as the [Add-on Repository URL](https://github.com/Stremio/stremio-static-addon-example/blob/master/README.md#dont-know-where-to-add-the-add-on-repository-url)


## Using with Now.sh

[Now.sh](https://zeit.co/now) is a simple to use (and free) website publishing utility.

- Install `now.sh`:

```
npm i -g now
```

- Clone Repository:

```
git clone --recursive http://github.com/Stremio/stremio-static-addon-example
cd stremio-static-addon-example
```

- Publish with `now.sh`:

```
$ now
```

- `now.sh` will typically print a message similar to:

```
> https://stremio-static-addon-example-ijshgdlgoe.now.sh [in clipboard] [3s]
> Deployment complete!
```

In which case, we'll use `https://stremio-static-addon-example-ijshgdlgoe.now.sh/manifest.json` as the [Add-on Repository URL](https://github.com/Stremio/stremio-static-addon-example/blob/master/README.md#dont-know-where-to-add-the-add-on-repository-url) to load our add-on in Stremio


## Using with Express

We've made a separate repository demonstrating how to use these static files with a Node.js Express Server. The example also shows how to make a locally hosted add-on accessible remotely with the help of the `localtunnel` module.

This example add-on can be found at [stremio-express-static-addon](https://github.com/Stremio/stremio-express-static-addon).


### Don't know where to add the Add-on Repository URL?

![add-on-repository-url](https://user-images.githubusercontent.com/1777923/43146711-65a33ccc-8f6a-11e8-978e-4c69640e63e3.png)
