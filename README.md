![triple image](http://cl.ly/image/3H2x3c2g1X0p/triple%20banner.png)

[REPL](http://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop) for Titanium. Features include:

* Full access to Titanium API
* Command history
* Multi-line statements
* Color-coded return values, by type

## Support

The following is the only configuration for which this has been tested so far:

* Mac OSX 10.9.4
* iOS 7.1 + simulator
* Titanium SDK 3.2.3+

Support for all of Appcelerator's supported platforms is planned. Windows OS support is planned as well.

## Install [![NPM version](https://badge.fury.io/js/triple.svg)](http://badge.fury.io/js/triple)

```bash
$ npm install -g triple
```

## Usage

```bash
$ triple
[creating app]
[loading app]
> alert('hello, world!');
```

## Testing [![Built with Grunt](https://cdn.gruntjs.com/builtwith.png)](http://gruntjs.com/)

```bash
# run jshint and unit tests
$ grunt

# create coverage report in ./coverage/index.html
$ grunt coverage
```

## Known Issues

### `this.Kroll`

Trying to inspect `this.Kroll` on iOS will cause a fatal error. This is due to the fact that `this.Kroll` is not a genuine Javascript object. It will be skipped if your inspect `this`, and it will crash the app if you try to inspect it directly.

## Credits

* Triskelion logo is a slight derivation from the original work of [Marco Kaiser](http://commons.wikimedia.org/wiki/User:Marco_Kaiser), which is licensed under [Creative Commons CC-BY-SA-2.5](http://creativecommons.org/licenses/by-sa/2.5/).
