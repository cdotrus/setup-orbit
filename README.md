# `setup-orbit` action

[![Test](https://github.com/cdotrus/setup-orbit/actions/workflows/test.yml/badge.svg?branch=trunk)](https://github.com/cdotrus/setup-orbit/actions/workflows/test.yml)

This GitHub Action will install a release of the orbit package manager for you.

## Usage

### Examples

In most cases all you will need is the following in your workflow.

```yaml
- uses: cdotrus/setup-orbit@v0.1.0
```

If you want a specific version of `orbit` you can specify this by passing the
`orbit-version` input.

```yaml
- uses: cdotrus/setup-orbit@v0.1.0
  with:
    orbit-version: '0.12.0'
```

### Inputs

| Name           | Required | Description                                  | Type   | Default               |
| -------------- | -------- | -------------------------------------------- | ------ | --------------------- |
| `orbit-version`| no       | A valid semver specification.                | string | null                  |

By default, the latest version of `orbit` will be installed.