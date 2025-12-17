# Install smlpkg

This action installs smlpkg in a GitHub Actions runner (Linux and macOS).
The package manager is installed in `$HOME/.local`, which means it will be on
the `$PATH` of a standard setup.

## Inputs

`version`

The full version to install as a string (e.g. `'0.1.5'`), or the
string `'latest'`.

## Example usages

```yaml
      - uses: diku-dk/install-smlpkg@v1
        with:
          version: '0.1.5'
```

```yaml
      - uses: diku-dk/install-smlpkg@v1
```

```yaml
      - uses: diku-dk/install-smlpkg@v1
        with:
          version: 'latest'
```
