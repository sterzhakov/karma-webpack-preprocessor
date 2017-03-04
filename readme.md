## How to install?

```
npm install karma-coffee-preprocessor --save-dev
```

## Configuration

```javascript
// karma.conf.js
module.exports = function(config) {
  config.set({

    // ...

    files: [
      '../app/**/*.karma.js',
    ],

    preprocessors: {
      ['../lib/**/*.karma.js']: ['webpack'],
    },

    webpackPreprocessor: {
      configPath: './config/webpack'
    },

    /// ...

  })
}

```

---

For more information on Karma see the [homepage](http://karma-runner.github.io/1.0/index.html)
.
