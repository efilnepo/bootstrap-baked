bootstrap-baked
===============

Build on top of generator-lessapp yeoman generator.

Modified Gruntfile to watch bootstrap less directory for changes

less: {
                files: ['/styles/{,*/}*.less', '/bower_components/bootstrap/less/{,*/}*.less'],
                tasks: ['less:server', 'autoprefixer']
            },

## How to use

mkdir project && cd $_
git clone git@github.com:efilnepo/bootstrap-baked.git
cd bootstrap-baked
nmp install
grunt --force //из-за тупой ошибки jshint
grunt serve

modify files and watch for changes
