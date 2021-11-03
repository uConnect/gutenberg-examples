# Gutenberg Examples

<p align="center"><img src="https://user-images.githubusercontent.com/1039236/47116000-fd775000-d27d-11e8-9c46-761a90cb30a2.gif" alt="Demo"></p>


Examples for extending
[Gutenberg](https://github.com/WordPress/gutenberg)
with plugins which create blocks.

See also:
[Gutenberg developer documentation](https://wordpress.org/gutenberg/handbook/)

## Development

This project uses the [`@wordpress/env`](https://developer.wordpress.org/block-editor/reference-guides/packages/packages-env/) package to provide a local development environment. Before you can use the development environment, you must install [Docker](https://docs.docker.com/get-docker/).

Once Docker is installed, clone this project and enter the working directory:

```
git clone git@github.com:uConnect/gutenberg-examples.git
cd gutenberg-examples
```

Then, install the project dependencies:

```
npm install
```

Once installed, start the local WordPress instance with one of two commands:

1. `npm run env:start` - Starts the instance normally.
2. `npm run env:start:debug` - Starts the instance with debugging enabled.

The WordPress instance will be available at http://localhost:8888/. You can login with the username and password "admin" and the password "password" at http://localhost:8888/wp-login.php. The plugin should be automatically activated.

To stop this local WordPress instance later run:

```
npm run env:stop
```

The block examples should be built and ready to use, however you can rebuild all of the ESNext examples by running `npm run build` from the project root.


For each of the examples that include an esnext example the following commands are required to build the plugins:

To install the node packages
```
npm install
```

To build a development version, change to the local directory of the block you are working on, and run `npm start` to watch for changes and automatically rebuild as you develop.
```
cd 05-recipe-card-esnext/
npm start
```


To build the production version of the plugin
```
npm run build
```

<br/><br/><p align="center"><img src="https://s.w.org/style/images/codeispoetry.png?1" alt="Code is Poetry." /></p>
