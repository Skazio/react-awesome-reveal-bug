# Bug

## Description of the bug

Linked to the issue [#147](https://github.com/morellodev/react-awesome-reveal/issues/147)

### Expected

The app runs and Slide-reveals the `Hello` text

### Actual

Failed after `npm install && npm start` with the following message :

```
Failed to compile.

./node_modules/react-awesome-reveal/dist/index.mjs
Can't import the named export 'Children' from non EcmaScript module (only default export is available)
```

## Environment

Here are the environment specs

### OS

`lsb_release -a` gives :

```
Distributor ID: Ubuntu
Description:    Ubuntu 20.04 LTS
Release:        20.04
```

### Node

`node --version` gives :

```
v16.17.0
```

### NPM

`npm --version` gives :

```
8.15.0
```

## Side Note

This does work correctly with `package.json` having:

```json
"dependencies": {
  "react": "17.0.2",
  "react-dom": "17.0.2",
  "@emotion/react": "11.10.6",
  "react-scripts": "4.0.3",
  "react-awesome-reveal": "4.0.1" <- Minor is 1 down
},
```
