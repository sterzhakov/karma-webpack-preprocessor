> Preprocessor to compile Webpack files on the fly.

## How to install?

```
npm install karma-webpack-preprocessor --save-dev
```

## Configuration

```javascript
// karma.conf.js
module.exports = function(config) {
  config.set({

    // ...

    files: [
      './app/**/*.spec.js',
    ],

    preprocessors: {
      ['./app/**/*.spec.js']: ['webpack'],
    },

    webpackPreprocessor: {
      configPath: './config/webpack'
    },

    /// ...

  })
}

```
