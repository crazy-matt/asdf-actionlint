# Contributing

## Testing Locally

```shell
asdf plugin test <plugin-name> <plugin-url> [--asdf-tool-version <version>] [--asdf-plugin-gitref <git-ref>] [test-command*]

#
asdf plugin test actionlint https://github.com/crazy-matt/asdf-actionlint.git "actionlint --version"
```

Tests are automatically run in GitHub Actions on push and PR.

## Linting Locally

```shell
task lint
task format
```
