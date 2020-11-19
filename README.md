[![Build Status](https://github.com/axetroy/changelog/workflows/ci/badge.svg)](https://github.com/axetroy/changelog/actions)
[![Go Report Card](https://goreportcard.com/badge/github.com/axetroy/changelog)](https://goreportcard.com/report/github.com/axetroy/changelog)
![Latest Version](https://img.shields.io/github/v/release/axetroy/changelog.svg)
![License](https://img.shields.io/github/license/axetroy/changelog.svg)
![Repo Size](https://img.shields.io/github/repo-size/axetroy/changelog.svg)

## changelog

A cli to generate changelog

> The project is in development

feature:
- [x] Cross-platform support
- [ ] Template Support
- [ ] Custom template
- [ ] Conventional Commits Parser

### Usage

```bash
# Automatically generate a change log from the current to the latest tag
$ changelog
# Generate 1.2.0 changelog
$ changelog v1.2.0
# Generate changelog from v1.2.0~v2.0.0
$ changelog v1.2.0 v2.0.0
# Generate changelog and write to CHANGELOG>md
$ changelog > CHANGELOG.md
```

### Installation

If you are using Linux/macOS. you can install it with the following command:

```shell
# install latest version
curl -fsSL https://raw.githubusercontent.com/axetroy/changelog/master/install.sh | bash
# or install specified version
curl -fsSL https://raw.githubusercontent.com/axetroy/changelog/master/install.sh | bash -s v1.3.0
# or install from gobinaries.com
curl -sf https://gobinaries.com/axetroy/changelog@v1.3.0 | sh
```

Or

Download the executable file for your platform at [release page](https://github.com/axetroy/changelog/releases)

Then set the environment variable.

eg, the executable file is in the `~/bin` directory.

```bash
# ~/.bash_profile
export PATH="$PATH:$HOME/bin"
```

then, try it out.

```bash
changelog --help
```

Finally, to use Deno correctly, you also need to set environment variables

```bash
# ~/.bash_profile
export PATH="$PATH:$HOME/.deno/bin"
```

### Build from source code

Make sure you have `Golang@v1.15.x` installed.

```shell
$ git clone https://github.com/axetroy/changelog.git $GOPATH/src/github.com/axetroy/changelog
$ cd $GOPATH/src/github.com/axetroy/changelog
$ make build
```

### Test

```bash
$ make test
```

### License

The [MIT License](LICENSE)
