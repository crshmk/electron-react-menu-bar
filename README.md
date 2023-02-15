## Boilerplate for Electron Menu Bar App using React

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
Change the src path to the bundle in `dist/index.html` from `/main` to `./main`. (If you know how to configure this please let me know.)

- Build the app 
```bash
npm run build:app
```

### Features 

- React with hooks for state management
- [IPC](https://www.electronjs.org/docs/latest/tutorial/ipc) 
- [Template image](https://github.com/electron/electron/blob/main/docs/api/native-image.md#template-image) 

### Icons 

Use the [SF Symbols app](https://developer.apple.com/sf-symbols/) to create a template image for the menu bar

Use [these instructions](https://apple.stackexchange.com/a/402653) to create a .icns icon for the applications folder
