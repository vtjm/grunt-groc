grunt-groc
================

A simple grunt task to generate a project's documentation using [Groc](http://nevir.github.com/groc/)

Groc depends on [Pygements](http://pygments.org/) to generate documentation. Follow the installation instructions [here](http://pygments.org/docs/installation/).

### Usage
Running `grunt groc:javascript` (or `grunt groc` since groc is a multitask) will generate documentation for the specified files.

```js
// Project configuration.
grunt.initConfig({
  groc: {
    javascript: [
      "tasks/*.js", "README.md"
    ],
    options: {
      "out": "doc/"
    }
  }
});
```

See [Groc's cli](http://nevir.github.com/groc/cli.html) for all available options