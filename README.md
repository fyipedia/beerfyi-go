# beerfyi

[![Go Reference](https://pkg.go.dev/badge/github.com/fyipedia/beerfyi-go.svg)](https://pkg.go.dev/github.com/fyipedia/beerfyi-go)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Beer style guide with BJCP styles, hops, malts, and yeast — API client for [beerfyi.com](https://beerfyi.com).

> **Try the interactive tools at [beerfyi.com](https://beerfyi.com)**

## Install

`go get github.com/fyipedia/beerfyi-go`

## Quick Start

```go
package main

import (
    "fmt"
    "fyipedia/beerfyi-go"
)

func main() {
    client := beerfyi.NewClient()
    result, err := client.Search("ipa")
    if err != nil {
        panic(err)
    }
    fmt.Println(result.Total, "results")
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install beerfyi` | [PyPI](https://pypi.org/project/beerfyi/) |
| **npm** | `npm install beerfyi` | [npm](https://www.npmjs.com/package/beerfyi) |
| **Go** | `go get github.com/fyipedia/beerfyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/beerfyi-go) |
| **Rust** | `cargo add beerfyi` | [crates.io](https://crates.io/crates/beerfyi) |
| **Ruby** | `gem install beerfyi` | [rubygems](https://rubygems.org/gems/beerfyi) |

## Embed Widget

Embed [BeerFYI](https://beerfyi.com) widgets on any website with [beerfyi-embed](https://widget.beerfyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/beerfyi-embed@1/dist/embed.min.js"></script>
<div data-beerfyi="entity" data-slug="ipa"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.beerfyi.com)

## Links

- [BeerFYI](https://beerfyi.com) — Main site
- [API Documentation](https://beerfyi.com/developers/)
- [OpenAPI Spec](https://beerfyi.com/api/openapi.json)
- [Glossary](https://beerfyi.com/glossary/)

## License

MIT
