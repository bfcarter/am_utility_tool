###:cherry_blossom: Utility Tool Developed by Ashley Miller :cherry_blossom:

![AGirleyGeek Approved](https://img.shields.io/badge/AGirleyGeek-Approved-feafbc.svg)

###:cherry_blossom: Before You Install :cherry_blossom:

Before you install my **Utility Tool**, you will need an app that you developed with **NodeJS**.

###:cherry_blossom: Install :cherry_blossom:

To install my **Utility Tool**, in your CLI, change your current directory to your app's directory, and type `npm install am_utility_tool --save`. This will add **am_utility_tool** to your *package.json* file's list of dependencies and install it to your *node_modules* directory.

###:cherry_blossom: Debugging :cherry_blossom:

My **Utility Tool** lets you debug your app and display a success, an error, or a warn message in your CLI.

To use my **Utility Tool**, you will need to require **am_utility_tool** in the file you want to debug. You can do this by typing `const debug = require('am_utility_tool')` at the top of the file. Then you will need to call the debugSuccess, debugError, or debugWarn functions with an argument of a success, an error, or a warn message wherever you want to use them. For example, if you want to call the debugError function in one of your routes, your code may look like this:

```
res.status(500).json(err);
debug.debugError('The user was not successfully redirected to the long URL because of the following error: ' + err);
```

To turn debugging on, in your CLI, change your current directory to your app's directory if it's not already your current directory, and type `DEBUG=true` before you start your server.

Now if your route errors out, you will get an error message in your CLI that says, *The user was not successfully redirected to the long URL because of the following error: [error]*.

###:cherry_blossom: Version Bumping :cherry_blossom:

To bump your version, in your CLI, type
```
node vbumper.js -v [major, minor, or patch] -n [version number]
```

For example, if you want to bump the major version to 2, in your CLI, type
```
node vbumper.js -v major -n 2
```
