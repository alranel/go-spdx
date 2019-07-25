# go-spdx

[![Go Report Card](https://goreportcard.com/badge/github.com/kyoh86/go-spdx)](https://goreportcard.com/report/github.com/kyoh86/go-spdx)
[![CircleCI](https://img.shields.io/circleci/project/github/kyoh86/go-spdx.svg)](https://circleci.com/gh/kyoh86/go-spdx)
[![Coverage Status](https://img.shields.io/codecov/c/github/kyoh86/go-spdx.svg)](https://codecov.io/gh/kyoh86/go-spdx)

The package parses SPDX license expression strings describing license terms.

> This a fork of the original https://github.com/kyoh86/go-spdx which I'm keeping because the original one seems not maintained actively (see my [pending Pull Request](https://github.com/kyoh86/go-spdx/pull/2))

## Install

```
go get github.com/kyoh86/go-spdx
```

## Usage

See [example](https://github.com/kyoh86/go-spdx/blob/master/cmd/go-spdx-example/main.go) or [test](https://github.com/kyoh86/go-spdx/blob/master/spdx/parser_test.go)

## Updating licenses

In order to update the licenses_asset.go file with the newest license list from SPDX, execute the following commands:

```
npm install spdx-license-list@latest
make licenses-asset
```

(You should also add a test to spdx/parser_test.go to make sure everything worked as expected.)

# LICENSE

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg)](http://www.opensource.org/licenses/MIT)

This is distributed under the [MIT License](http://www.opensource.org/licenses/MIT).
