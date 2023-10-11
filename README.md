## Mirador Plugin that intercept click, zoom and canvas change event
The plugin was implemented as a React component integrated into the Mirador application. The purpose of plugin development is to monitor and record specific events by a user within the application. Once the event is intercepted, all information relating to it is sent to a local Restful server via HTTP requests.
The plugin monitors three main types of events within Mirador:
- `handleClick:` The plugin detects clicks on specific elements within Mirador windows and records these interactions, including details of the clicked element.
- `handleZoom:` The plugin detects zoom events and records their details, including the element that was zoomed to.
- `windowAdded:` The plugin detects when a new window is added to Mirador and logs the details of the event by highlighting the new image information.

## Integrating Mirador

This repository is designed to show integrating Mirador 3 with modern frontend build systems.

### Dependencies

You will likely need to have at least the following dependencies available in your `package.json`.

 - `mirador`
 - `react`
 - `react-dom`
 - `mirador-image-tools` - A plugin just to test plugin integration

### Webpack

See `./webpack` for a basic webpack setup for Mirador 3 + a plugin.

```sh
npm run webpack
```

### Parcel

See `./parcel`, but essentially it is just an html file referencing the JavaScript.

```sh
npm run parcel
```
