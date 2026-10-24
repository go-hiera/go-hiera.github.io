<p align="center"><img src="https://raw.githubusercontent.com/go-hiera/brand/main/social/go-hiera.png" alt="go-hiera/go-hiera.github.io" width="720"></p>

# go-hiera.github.io

The organization's institutional landing page, served at
<https://go-hiera.github.io> and built with [Hugo](https://gohugo.io). It is a
single page (custom `layouts/index.html`, capability cards driven by
`[[params.phases]]` in `hugo.toml`) for [go-hiera](https://github.com/go-hiera) —
a pure-Go (CGO=0) reimplementation of Puppet's Hiera 5 hierarchical data-lookup
engine.

Documentation lives in a separate repository,
[go-hiera/docs](https://github.com/go-hiera/docs), served at
<https://go-hiera.github.io/docs/>. This page links there.

`.github/workflows/deploy-pages.yml` builds the landing with Hugo and deploys it
to GitHub Pages on every push to `main`.

## Local preview

```bash
hugo server      # http://localhost:1313
```

## The design is not here

It comes from the shared Hugo module
[`go-fleettools/landingkit`](https://github.com/go-fleettools/landingkit),
pinned in `go.mod` (Renovate bumps it); `kit.go` keeps `go mod tidy` from
deleting that requirement. `[params.brand]` in `hugo.toml` is read from the logo by
`landingkit brand`. A file under `layouts/partials/` with the name of one of the
kit's would silently override it.
