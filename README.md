# Electron - TODO APP

**Compile Vue app using electron and electron-packager with OS-specific bundles.**

**Install ElectronJS and Electron Packager**

```bash
# Go to repo and install ElectronJs
npm install electron --save-dev [--save-exact]

# install electron-packager
npm install electron-packager --save-dev
```

**Instructions**

1. Build your vue app for production.
2. Copy the files in the dist folder to the electron main directroy. 
3. Run the following command to compile the code and build installable apps. 
###### NOTE: To create a Windows app using mac os, you will need to have wine installed.

```bash
# Running electron-packager from the command line 
electron-packager . todo --platform=all --overwrite --arch=x64 --icon=/img/logo.icns --prune=true --out=release-builds
```

## Resources for Electron and Electron Packager APIs 

- [electronjs.org/docs](https://electronjs.org/docs) - all of Electron's documentation
- [github.com/electron-userland/electron-packager](https://github.com/electron-userland/electron-packager/blob/master/docs/api.md) - Electron Packager API