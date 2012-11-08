
# todo

  Todo list component example

## Installation

 Install express for the server, and the component dependencies:

    $ npm install
    $ make

## Running the app

    $ node app

## Implementation

  All private client-side components are located in `./client`,
  while server related REST end-points are in `./server`. The `./index.html`
  file bootstraps the client-side, and `app.js` is a small Express server
  to power the backend.

  Each client-side component in `./client` defines its own dependencies,
  both "local" (in the `./client` dir), and remote from public components
  that devs have created. On `make` these are installed and the builder
  outputs `./build`. The tiny 1-line middleware in `./server/build` executes
  `make` on-demand each time `index.html` is requested, so you don't even
  have to know about the build

## License

  MIT