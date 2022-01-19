<h1 align="center">fivem-ts-boilerplate</h1>

<p align="center">
  <i>:fire: A Typescript Boilerplate for FiveM :video_game:</i>
  <br>
  <br>
  <a href="https://github.com/v0idp/fivem-ts-boilerplate/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT">
  </a>
</p>

This project is based on the basic boilerplate by [d0p3t](https://github.com/d0p3t) for creating a FiveM resource using Typescript. I made some improvements and updates to the packages to keep it up-to-date. It includes webpack config files, linting (ESlint + prettier) and a directory structure to get you started. I also included [native-wrappers-client](https://github.com/AvarianKnight/native-wrappers-client/tree/master/examples/typescript/src) to increase development time. Original repository can be found here: [d0p3t/fivem-ts-boilerplate](https://github.com/d0p3t/fivem-ts-boilerplate)

## Usage
1. Clone repository into your `resources/[local]` folder.
2. `yarn install` the dependencies.
3. Start development.

### Development
Use `yarn run watch` to watch files during development.

### Production
Build your production ready code with `yarn run build`.

This will build the client and server script with the `--mode production` flag.

### Automatic Builds (Optional)
The `fxmanifest.lua` is not setup to automatically build upon first FXServer start. If you'd like to setup automatic builds you must remove the comments on the following lines in your `fxmanifest.lua`.

```lua
dependency 'yarn'
dependency 'webpack'

webpack_config 'webpack.config.js'
```

## License
This product is MIT licensed. Please make sure you give credit and include this license in your product.
