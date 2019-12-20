# Ara Framework - Static example

## Run Nova

The folder `nova` contains a nova generated with [Ara CLI](https://github.com/ara-framework/ara-cli) configured with no SSR.

Run webpack dev server:

```
yarn dev

```

The `client.js` can be consumed on http://localhost:<port>/client.js


## Run Host Application

In this example the host application is just a static file that contains the placeholder where the micro-frontend needs to be mounted.

```
<div data-hypernova-key="Example" data-hypernova-id="8f07d513-0c84-4b16-8058-08cf2a014d0d"></div>
<script type="application/json" data-hypernova-key="Example" data-hypernova-id="8f07d513-0c84-4b16-8058-08cf2a014d0d"><!--{"title":"Ara Framework"}--></script>
```

The `div` tag is where the component named `Example` will be mounted and the `script` tag contains the initial state to render it.

Run host application:

```
yarn serve
```

The application uses [http-server] to serve the `index.html` file behind of scenes.