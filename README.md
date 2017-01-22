# pctl - zsh plugin for proxy

[Overview](#overview) |
[Installation](#installation) |
[Configuration](#configuration) |
[License](#license)

[![license-badge]][license-link]
[![release-badge]][release-link]

## Overview

This is zsh plugin to toggle the environment variables of proxy.

[![screenshot]][demo-link]

## Installation

You can use zplug to install pctl.
Add the following to your `.zshrc`:

```zsh
zplug 'ytet5uy4/pctl'
```

## Configuration

Add the following to your `.zshrc`:

```zsh
export PROXY_ADDRESS=proxy.example.com PORT=8080
```

To keep the environment variables of proxy when using `sudo`,
append the following to `/etc/sudoers` via `sudo visudo`:

```zsh
Defaults env_keep += "http_proxy https_proxy"
```

## License

Copyright (c) 2015 ytet5uy4

Released under the MIT License, see **[LICENSE.md][license-link]**.

[screenshot]: https://raw.githubusercontent.com/wiki/ytet5uy4/pctl/screenshot.png
[release-badge]: https://img.shields.io/github/release/ytet5uy4/pctl.svg?style=flat-square
[license-badge]: https://img.shields.io/github/license/ytet5uy4/pctl.svg?style=flat-square

[demo-link]: //asciinema.org/a/59no1i98y61fvpdcq3n086r3h
[release-link]: //github.com/ytet5uy4/pctl/releases/latest
[license-link]: LICENSE.md
