<div align="center">

# asdf-actionlint [![Build](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/build.yml/badge.svg)](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/build.yml) [![Lint](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml/badge.svg)](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml)


[actionlint](https://github.com/rhysd/actionlint/blob/main/docs/README.md) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [Contents](#contents)
- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Dependencies

- `bash`, `curl`, `tar`: generic POSIX utilities.

# Install

Plugin:

```shell
asdf plugin add actionlint
# or
asdf plugin add actionlint https://github.com/crazy-matt/asdf-actionlint.git
```

actionlint:

```shell
# Show all installable versions
asdf list-all actionlint

# Install specific version
asdf install actionlint latest

# Set a version globally (on your ~/.tool-versions file)
asdf global actionlint latest

# Now actionlint commands are available
actionlint --version
```

Check [asdf](https://github.com/asdf-vm/asdf) readme for more instructions on how to
install & manage versions.

# Contributing

Contributions of any kind welcome! See the [contributing guide](contributing.md).

[Thanks goes to these contributors](https://github.com/crazy-matt/asdf-actionlint/graphs/contributors)!

# License

Licensed under the [Apache License 2.0](LICENSE)