<div align="center">

# asdf-actionlint [![Build](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/build.yml/badge.svg)](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/build.yml) [![Lint](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml/badge.svg)](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml)


[actionlint](https://github.com/rhysd/actionlint/blob/main/docs/README.md) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

# Contents

- [asdf-actionlint ![Build](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/build.yml) [![Lint](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml/badge.svg)](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml)](#asdf-actionlint--)
- [Contents](#contents)
- [Build History](#build-history)
- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
- [License](#license)

# Build History

[![Build history](https://buildstats.info/github/chart/crazy-matt/asdf-actionlint?branch=main)](https://github.com/crazy-matt/asdf-actionlint/actions)

# Dependencies

- `bash`, `curl`, `tar`: generic POSIX utilities.
- ASDF_SKIP_VERIFY: skip verifying checksums.
- ASDF__OVERWRITE_ARCH: set this environment variable to force the plugin to use a specified processor architecture rather than the automatically detected value. Useful, for example, for allowing users on M1 Macs to install amd64 binaries when there's no arm64 binary available.

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
