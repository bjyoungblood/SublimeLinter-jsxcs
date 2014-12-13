SublimeLinter-jsxcs
=========================

[![Build Status](https://travis-ci.org/SublimeLinter/SublimeLinter-jsxcs.svg?branch=master)](https://travis-ci.org/SublimeLinter/SublimeLinter-jsxcs)

This linter plugin for [SublimeLinter](http://sublimelinter.readthedocs.org) provides an interface to [jsxcs](https://github.com/orktes/node-jsxcs). It will be used with files that have “JSX” syntax.

![SublimeLinter-jsxcs](demo.gif "SublimeLinter-jsxcs plugin demo")

## Installation
SublimeLinter 3 must be installed in order to use this plugin. If SublimeLinter 3 is not installed, please follow the instructions [here](http://sublimelinter.readthedocs.org/en/latest/installation.html).

### Linter installation
Before using this plugin, you must ensure that `jsxcs` is installed on your system. To install `jsxcs`, do the following:

1. Install [Node.js](http://nodejs.org) (and [npm](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager) on Linux).

1. Install `jsxcs` by typing the following in a terminal:
   ```
   npm install -g jsxcs
   ```

1. If you are using `nvm` and `zsh`, ensure that the line to load `nvm` is in `.zshenv` and not `.zshrc`.

1. If you are using `zsh` and `oh-my-zsh`, do not load the `nvm` plugin for `oh-my-zsh`.

**Note:** This plugin requires `jsxcs` 0.2.1 or later.

### Linter configuration
In order for `jsxcs` to be executed by SublimeLinter, you must ensure that its path is available to SublimeLinter. Before going any further, please read and follow the steps in [“Finding a linter executable”](http://sublimelinter.readthedocs.org/en/latest/troubleshooting.html#finding-a-linter-executable) through “Validating your PATH” in the documentation.

Once `jsxcs` is installed and configured, you can proceed to install the SublimeLinter-jsxcs plugin if it is not yet installed.

### Plugin installation
Please use [Package Control](https://sublime.wbond.net/installation) to install the linter plugin. This will ensure that the plugin will be updated when new versions are available. If you want to install from source so you can modify the source code, you probably know what you are doing so we won’t cover that here.

To install via Package Control, do the following:

1. Within Sublime Text, bring up the [Command Palette](http://docs.sublimetext.info/en/sublime-text-3/extensibility/command_palette.html) and type `install`. Among the commands you should see `Package Control: Install Package`. If that command is not highlighted, use the keyboard or mouse to select it. There will be a pause of a few seconds while Package Control fetches the list of available plugins.

1. When the plugin list appears, type `jsxcs`. Among the entries you should see `SublimeLinter-jsxcs`. If that entry is not highlighted, use the keyboard or mouse to select it.

## Settings
For general information on how SublimeLinter works with settings, please see [Settings](http://sublimelinter.readthedocs.org/en/latest/settings.html). For information on generic linter settings, please see [Linter Settings](http://sublimelinter.readthedocs.org/en/latest/linter_settings.html).

Since this plugin is executing `jsxcs` on your system, you may use `.jscsrc` files to configure its behavior. See the [jscs documentation](https://github.com/mdevils/node-jscs#configuration) for more information.

**Note**: Whereas `jsxcs` only looks in the linted file’s directory for a `.jscsrc` file, this linter plugin extends that behavior by searching the file hierarchy up to the root directory and then in the user’s home directory.

## Contributing
If you would like to contribute enhancements or fixes, please do the following:

1. Fork the plugin repository.
1. Hack on a separate topic branch created from the latest `master`.
1. Commit and push the topic branch.
1. Make a pull request.
1. Be patient.  ;-)

Please note that modications should follow these coding guidelines:

- Indent is 4 spaces.
- Code should pass flake8 and pep257 linters.
- Vertical whitespace helps readability, don’t be afraid to use it.

Thank you for helping out!
