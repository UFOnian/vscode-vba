# VSCode VBA

[![Marketplace Version](https://vsmarketplacebadge.apphb.com/version/spences10.vba.svg)](https://marketplace.visualstudio.com/items?itemName=spences10.vba)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/spences10.vba.svg)](https://marketplace.visualstudio.com/items?itemName=spences10.vba)
[![Rating](https://vsmarketplacebadge.apphb.com/rating/spences10.vba.svg)](https://marketplace.visualstudio.com/items?itemName=spences10.vba)

<!-- TOC depthFrom:2 -->

- [Syntax Highlighting](#syntax-highlighting)
- [Snippets](#snippets)
  - [Basic code](#basic-code)
- [Installation](#installation)
- [Contributing](#contributing)
- [Contacts](#contacts)
- [Links](#links)
- [Handy links](#handy-links)

<!-- /TOC -->

## Syntax Highlighting

This package provides syntax highlighting and snippets of VBA.

Based off an import of the
[VBScript.tmLanguage](https://github.com/SublimeText/VBScript/blob/master/VBScript.tmLanguage)
file from the
[Sublime Text VBScript](https://github.com/SublimeText/VBScript)
repository.

## Snippets

### Basic code

- dim declarations
- if/else
- for/while
- sub/function with errHandler
- case

## Installation

Launch VS Code Quick Open (Ctrl+P), paste the following command, and
press enter.

```
ext install vba
```

## Contributing

Please fork this repository and contribute back using pull requests.

Any contributions, large or small, major features, bugfixes and
integration tests are welcomed and appreciated but will be thoroughly
reviewed and discussed.

## Contacts

You can contact me in the following ways:

- Mail : [spences10apps@gmail.com](mailto:spences10apps@gmail.com)
- Github : [spences10](https://github.com/spences10)

## Links

- [Source Code](https://github.com/spences10/vscode-vba)
- [Market](https://marketplace.visualstudio.com/items?itemName=spences10.VBA)

## Handy links

I struggled to find how to generate a token after not doing anything
with this project for well over a year:

To get to your token creation, go here:

- https://YOUR_USER_NAME.visualstudio.com/_details/security/tokens

**Create a token:**

- Name: vsce
- Organisation: All accessible organizations
- show all scopes, select:
  - Marketplace
  - Check Acquire and Manage

**Publish with CLI:**

```bash
# login
vsce login <publisher name>
vsce package
# myExtension.vsix generated
# bump version
# vsce publish major, minor or patch
vsce publish -p <add created token here>
```

If you get `ERROR Failed request: (401)` see here:

- https://github.com/Microsoft/vscode-vsce/issues/11

Some good documentation on publishing with the CLI:

- https://code.visualstudio.com/api/working-with-extensions/publishing-extension

## Version history

```
20200405 - Added basic If snippet, and changed all snippets to use tabs (for user customisation capability).
20200405 - Multi-line comment capability
20200405 - Added certain keywords e.g. Type, Enum, Implements, Optional, Friend, ... Also changed behavior of some keywords, e.g. "End","Function","Sub" instead of "End Function", "End Sub" etc..
20200405 - Removal of non-vba behavior.
```
