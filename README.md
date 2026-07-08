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
