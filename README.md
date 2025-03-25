# Articola Tools' JSON linter

[![image size](https://ghcr-badge.egpl.dev/articola-tools/json-linter/size?color=dodgerblue)](https://ghcr-badge.egpl.dev/articola-tools/json-linter/size?color=dodgerblue)

This repo contains Dockerfile with preconfigured [JSON linter](https://github.com/prantlf/jsonlint).

## Usage

Use `ghcr.io/articola-tools/json-linter` Docker image with `-v ./:/linter_workdir/repo`
parameter, where `./` - is a path to a folder with files you want to lint.
By default, linter outputs correct JSON to stdout. For validation only, use `--check`
parameter.

Example command to use this linter -
`docker run --rm -v ./:/linter_workdir/repo ghcr.io/articola-tools/json-linter --check`

