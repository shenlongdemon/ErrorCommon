## Debug

run node with command:


with debugger
```
$ node --inspect-brk index.js
``` 
without debugger
```
$ node index.js
``` 



with configuration
```
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Attach",
            "type": "node",
            "request": "attach",
            "port": 9229,
            "address": "localhost",
            "restart": false,
            "sourceMaps": false,
            "outDir": null,
            "localRoot": "${workspaceRoot}",
            "remoteRoot": null
        }
    ]
}
```


## Running Locally

Make sure you have [Node.js](http://nodejs.org/) and the [Heroku CLI](https://cli.heroku.com/) installed.

```sh
$ git clone git@github.com:heroku/node-js-getting-started.git # or clone your own fork
$ cd node-js-getting-started
$ npm install
$ npm start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku open
```
or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Documentation

For more information about using Node.js on Heroku, see these Dev Center articles:

- [Getting Started with Node.js on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- [Heroku Node.js Support](https://devcenter.heroku.com/articles/nodejs-support)
- [Node.js on Heroku](https://devcenter.heroku.com/categories/nodejs)
- [Best Practices for Node.js Development](https://devcenter.heroku.com/articles/node-best-practices)
- [Using WebSockets on Heroku with Node.js](https://devcenter.heroku.com/articles/node-websockets)


The first, because of missing node_modules so you must run below command 
```
npm install
```




Error 

Error: EACCES: permission denied, access '/usr/local/lib/node_modules/react-native-cli'
```
sudo chown -R $(whoami) /usr/local/lib/node_modules/react-native-cli
```


Error: Building and installing the app on the device (cd android && ./gradlew installDebug)...
Could not install the app on the device, read the error above for details.
Make sure you have an Android emulator running or a device connected and have
set up your Android development environment:

```
chmod 755 android/gradlew
```

Error: bundling failed: "TransformError: /Users/ntlong/ShareLocSL/ShareLocSL/index.android.js: Cannot find module 'AccessibilityInfo' (While processing preset: \"/Users/ntlong/ShareLocSL/ShareLocSL/node_modules/react-native/Libraries/react-native/react-native-implementation.js\")"

```
Remove build folder in android/app
npm install -g react-native-git-upgrade
```






Open Shake menu
```
adb shell input keyevent 82
```

Update npm lastest version 
```
npm install npm@latest -g
```

Remove npm, uninstall npm
```
npm ls -gp --depth=0 | awk -F/ '/node_modules/ && !/\/npm$/ {print $NF}' | xargs npm -g rm
```

Install npm
```
brew install node
brew install watchman
```


Remove node, uninstall node
```
sudo rm -rf  /usr/local/lib/node_modules/npm/
brew uninstall node
brew doctor
brew prune
```

