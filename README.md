# grunt-mixtape-run-app

> A Grunt task to to run the server in the mixtape boilerplate

## Getting Started
This plugin requires Grunt `~0.4.1`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install -g nodemon
npm install grunt-mixtape-run-app --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-mixtape-run-app');
```

## The "runapp" task

### Overview
In your project's Gruntfile, add a section named `runapp` to the data object passed into `grunt.initConfig()`.

* `env: [String]` The NODE_ENV to pass to the server

#### Options
* `dieWithParent: [true|false]` Keeps the server running until the parent process exits (end of Grunt tasks).  Useful for e2e testing. 

### Usage Examples

```js
runapp: {
  development : {
    env: 'development'
  },

  debug : {
    env: 'debug'
  },

  production : {
    env: 'production'
  },

  test : {
    options: {
      dieWithParent: true
    },
    env: 'test'
  }
}
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_
