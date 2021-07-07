# Kindly-Beta
# All links and common extension information is in the ./public/manifest.json file
# manifest follows format described at https://developer.chrome.com/docs/extensions/mv3/manifest/
# Kindly API URL is in ./src/config.ts 

# Kindly API Chrome Extension

Kindly API Chrome Extension written on TypeScript within Visual Studio Code.
Supported all generic Textarea inputs, and extensible interface for the not-ordinary forms. Adapters for Twitter, Instagram, Facebook and Gmail already included.

## Prerequisites

* [node + npm](https://nodejs.org/) (Current Version)

## Option

* [Visual Studio Code](https://code.visualstudio.com/)

## Includes the following

* [TypeScript](https://github.com/microsoft/TypeScript)
* [Webpack](https://github.com/webpack/webpack)
* [SweetAlert2](https://github.com/sweetalert2/sweetalert2)

## Project Structure

* ./src: TypeScript source files
* ./public: Static files
* ./dist/build: Chrome Extension directory (dev mode, mocked requests)
* ./dist/release-x.x.x.x: Chrome Extension directory (release mode)

## Setup

```
$ npm install
```

## Open as Visual Studio Code project

```
$ code .
```

## Config file

```
./src/config.ts
```

## Run / build

### Visual Studio Code

To run within VSCode, type `Ctrl + Shift + B`

### Terminal

#### Build in watch mode

Run in development mode (autocompiling and API requests mocker, full console log output)

```
$ npm run watch
```

#### Build preview release

Build current version in preview mode (poduction API, output only info messages)

```
$ npm run build
```

#### Build production release

Build in production mode (production API, minified code, no console output)

```
$ npm run release
```

## Load extension to chrome

On [chrome://extensions/](chrome://extensions/) turn on Development mode an load unpacked extension from `./dist/build` or `./dist/release-x.x.x.x` directory
