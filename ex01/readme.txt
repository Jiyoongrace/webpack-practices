ex01: Bundling I: JS Module

0. Init. Project
$ npm init -y

1. Install Packages
$ npm i -D webpack webpack-cli express

----------------------------------------------------------------
* npx webpack --version
  System:
    OS: macOS 14.5
    CPU: (8) arm64 Apple M3
    Memory: 448.34 MB / 16.00 GB
  Binaries:
    Node: 20.15.0 - ~/.nvm/versions/node/v20.15.0/bin/node
    npm: 10.7.0 - ~/.nvm/versions/node/v20.15.0/bin/npm
  Browsers:
    Chrome: 126.0.6478.127
    Safari: 17.5
  Packages:
    webpack: ^5.92.1 => 5.92.1
    webpack-cli: ^5.1.4 => 5.1.4

----------------------------------------------------------------
* npx webpack ./src/index.js
asset main.js 157 bytes [emitted] [minimized] (name: main)
orphan modules 133 bytes [orphan] 1 module
./src/index.js + 1 modules 225 bytes [built] [code generated]

WARNING in configuration
The 'mode' option has not been set, webpack will fallback to 'production' for this value.
Set 'mode' option to 'development' or 'production' to enable defaults for each environment.
You can also set it to 'none' to disable any default behavior. Learn more: https://webpack.js.org/configuration/mode/

webpack 5.92.1 compiled with 1 warning in 134 ms
----------------------------------------------------------------

2. NPM Scripting

  "scripts": {
    "start": "node dev-server",
    "build": "npx webpack ./src/index.js -o ./public"
  }

3. Build(Bundling)
$ npm run build  

4. Test
$ npm start
