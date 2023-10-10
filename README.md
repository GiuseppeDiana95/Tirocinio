#Plugin intercept Mirador event
Il plugin è stato implementato come un componente React integrato nell'applicazione Mirador. Lo scopo dello sviluppo del plugin è quello di monitorare e registrare eventi specifici da parte di un utente all'interno dell'applicazione. Una volta intercettato l’evento, tutte le informazioni relative a quest’ultimo vengono inviate ad un server Restful locale tramite richieste HTTP.

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
