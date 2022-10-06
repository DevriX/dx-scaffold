# DevriX Scaffold CLI

This is a CLI tool to scaffold a new plugin based on the DevriX plugin boilerplate.
## Installation


```bash
composer global require devrix/scaffold
```

> Note: Make sure to place the `~/.composer/vendor/bin` directory (or the equivalent directory for your OS) in your PATH so the `dx-scaffold` executable can be located by your system.

```bash
export PATH="$PATH:$HOME/.config/composer/vendor/bin"
```

## Usage

After installing the composer package `cd` to the `wp-content/plugins` directory.

Then run the following command to start the interactive CLI:

```bash
dx-scaffold plugin new
```

You can predefine the plugin attributes by specifying them as arguments:

- `name=""` - The name of the plugin.
- `slug=""` - The slug of the plugin.
- `class=""` - The main class of the plugin.
- `namespace=""` - The namespace of the plugin.
- `abbr=""` - The abbreviation to use for global variables.

Example usage:
```bash
dx-scaffold name="DevriX" slug="devrix" class="Devrix" namespace="DX" abbr="DX" 
```

You can also skip parts of the interactive CLI by specifying a `--skip` flag.

- `--skip-clone` - Skips the git clone step.
- `--skip-rename` - Skips the renaming/search-replace step.
- `--skip-npm` - Skips `npm install` and `npm run prod`.


## License
MIT [DevriX](https://devrix.com)