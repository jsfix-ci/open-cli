# open-cli [![Build Status](https://travis-ci.org/sindresorhus/open-cli.svg?branch=master)](https://travis-ci.org/sindresorhus/open-cli)

> Open stuff like URLs, files, executables. Cross-platform.


## Install

```
$ npm install --global open-cli
```


## Usage

```
$ open-cli --help

  Usage
    $ open-cli <file|url> [--wait] [--background] [-- <app> [args]]
    $ cat <file> | open-cli [--ext] [--wait] [--background] [-- <app> [args]]

  Options
    --wait         Wait for the app to exit
    --background   Do not bring the app to the foreground (macOS only)
    --ext          File extension for when stdin file type can't be detected

  Examples
    $ open-cli https://sindresorhus.com
    $ open-cli https://sindresorhus.com -- firefox
    $ open-cli https://sindresorhus.com -- 'google chrome' --incognito
    $ open-cli unicorn.png
    $ cat unicorn.png | open-cli
    $ echo '<h1>Unicorns!</h1>' | open-cli --ext=html
```

The [following file types](https://github.com/sindresorhus/file-type#supported-file-types) are automagically detected when using stdin mode.


## Related

- [open](https://github.com/sindresorhus/open) - API for this module


## License

MIT © [Sindre Sorhus](https://sindresorhus.com)
