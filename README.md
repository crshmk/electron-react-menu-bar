<img src="https://github.com/crshmk/electron-react-menu-bar/blob/master/app-image.png" width="300" />

## Boilerplate for macOS Electron Menu Bar App using React

No Typescript 

### Development

```bash
npm run dev
```

To turn on the dev tools and use a larger window, flip the `showDevTools` flag in `main/createWindow/config`. You can also leave this on to debug a prod build.

### Production Builds 
- Bundle the renderer
```bash
npm run build:renderer
```
- Change the src path to the bundle in `dist/index.html` from `/main` to `./main`. (If you know how to configure this please let me know.)

- Build the app 
```bash
npm run build:app
```

### Features 

- React with hooks for state management
- [IPC](https://www.electronjs.org/docs/latest/tutorial/ipc) 
- Icons 

### Icons 

- Use the [SF Symbols app](https://developer.apple.com/sf-symbols/) to create a [template image](https://github.com/electron/electron/blob/main/docs/api/native-image.md#template-image) for the menu bar. Update the icons and `iconPath` in `main/createTray`.

- To [create](https://apple.stackexchange.com/a/402653) the .icns icon that will display in the applications folder, create a `.png` icon of size 1024 x 1024 px named `icon1024.png` and put it in the root folder. From the root, run `./create-app-icon.sh`.

