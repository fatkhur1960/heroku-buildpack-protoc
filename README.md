# heroku-buildpack-protoc

Install Protocol Buffer compiler `protoc` and some compiler plugins.

## How to use
Add a URL of this buildpack to your `.buildpacks` file. This buildpack just installs a `protoc` command.

This buildpack requires `pear` to install PHP plugin. So your `.buildpacks` should be like this;

```
https://github.com/heroku/heroku-buildpack-php
https://github.com/tayama0324/heroku-buildpack-protoc
...
```

See also: [Using Multiple Buildpack for an App](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app)

## Plugins
PHP code generation by [stanley-cheung/Protobuf-PHP](https://github.com/stanley-cheung/Protobuf-PHP) is available.
Specify `--php_out` option to `protoc`.

## LICENSE
MIT Licnense unless otherwise specified.
