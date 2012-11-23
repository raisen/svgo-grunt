## SVGO Grunt v0.0.1

[SVGO](https://github.com/svg/svgo/) task for the [Grunt](https://github.com/gruntjs/grunt) build tool.

## How to use

In your `grunt``ed-project directory:

```sh
$ npm install svgo-grunt
```

In your `grunt.js` gruntfile, something like this:

```javascript
module.exports = function(grunt) {

    grunt.initConfig({
        svgo: {
            optimize: {
                files: '*.svg'
            }
        }
    });

    grunt.loadNpmTasks('svgo-grunt');

    grunt.registerTask('default', 'svgo');

};
```