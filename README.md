# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Requirements

- Node.js version 18.0 or above (which can be checked by running `node -v`). You can use [nvm](https://github.com/nvm-sh/nvm) for managing multiple Node versions on a single machine installed.
    - When installing Node.js, you are recommended to check all checkboxes related to dependencies.

For more information, please refer to the [official documentation](https://docusaurus.io/docs/installation).

## Install the dependencies

```bash
npm install
```

### Run Local Development

```bash
npm start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

## Build for Production

```bash
npm build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.
