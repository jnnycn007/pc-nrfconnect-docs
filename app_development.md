---
---

# Everyday app development

After you [created a project for a new app](./create_new_app) or
[got the sources of an existing app](./get_an_existing_app_s_sources), you can start developing
your app.

## Install dependencies

Install the required Node.js dependencies with the `npm ci` command.

You need to do this at the beginning of the development process.
Later, this is required only if the dependencies change.

## Compiling

You can use the following commands for compiling your application:

* `npm run watch` (recommended) - This command compiles and packs all your code into `dist/bundle.js`.
  It also continuously checks the types. It then waits and watches your code. Whenever you save source files, it
  creates a new `dist/bundle.js`. You can stop it at any time with Ctrl-C.

* `npm run build:dev` - If you just want to compile and pack the code only once.

* `npm run build:prod` - If you want to create a `dist/bundle.js` package that is optimized for production use (for example, the bundle is minified).

## Running

Complete the following steps to run your application:

1. Start nRF Connect for Desktop. The launcher finds all apps in
`~/.nrfconnect-apps/local` and, using the `package.json` in your project, picks
up the `dist/bundle.js` that was built before.
1. Look for your app in the list with a “local” tag under its name.
1. Launch the app.

When you edit the source of the app and it is recompiled, press Ctrl-R (Windows or Linux) or Cmd-R
(macOS) in the running app window to reload it.

Chrome Developer Tools can be opened by pressing Ctrl-Alt-I (Windows or Linux) or
Cmd-Option-I (macOS).

## Testing

You can use the following commands for testing:

* `npm run check` - For running static checks like linting and type checking
* `npm test` - For unit tests

## Distributing development versions

To distribute your development version of an app to others, run
`npm pack`.

This command creates a file that you can send to others so that they can
[install that app locally](./local_app_installation). For example, for the `pc-nrfconnect-boilerplate` app, the file will be named `pc-nrfconnect-boilerplate-0.0.1.tgz`.
