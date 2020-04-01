# Electron Builder Template

This template is an example of how to build apps with electron-builder and publish them.

## Output formats

The output formats used are AppImage for Linux, portable .exe for Windows, and dmg for mac.

## Getting started

```
$ npm i
$ npm start
```

If google.com opens up then its working fine. Just change the icon in src/icon.png and build-resources/icon.png and you can point to
any other website by changing the url in main.js.

## Building.

### Linux and Windows builds:

** NOTE: You need docker for building windows .exe on linux. **

If you are on linux you can build for linux and windows by running:
```
$ npm run build-linux-and-windows
```

For just linux
```
$ ./node_modules/.bin/electron-builder -l
```

For just windows
```
$ ./node_modules/.bin/electron-builder -w
```

### Mac

To build dmg you need a mac, after the getting started steps run:
```
$ npm run build-mac
```

OR

```
$ ./node_modules/.bin/electron-builder -m
```


The output folder is /dist all the targets will be found there.