<div align="center">

# asdf-actionlint [![Build](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/build.yml/badge.svg)](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/build.yml) [![Lint](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml/badge.svg)](https://github.com/crazy-matt/asdf-actionlint/actions/workflows/lint.yml)

[actionlint](https://github.com/rhysd/actionlint/blob/main/docs/README.md) plugin for the [asdf version manager](https://asdf-vm.com).

</div>

<details open="open">
<summary>Table of Contents</summary>

- [Build History](#build-history)
- [Dependencies](#dependencies)
- [Install](#install)
- [Contributing](#contributing)
  - [Tooling Requirements](#tooling-requirements)
    - [Task](#task)
- [License](#license)

</details>

# Build History

[![Build history](https://buildstats.info/github/chart/crazy-matt/asdf-actionlint?branch=main)](https://github.com/crazy-matt/asdf-actionlint/actions)

# Dependencies

- `bash`, `curl`, `tar`: generic POSIX utilities.
- `ASDF_SKIP_VERIFY`: set this environment variable to g u pskip verifying checksums.
- `ASDF_OVERWRITE_ARCH`: set this environment variable to force the plugin to use a specified processor architecture rather than the automatically detected value. Useful, for example, for allowing users on M1 Macs to install amd64 binaries when there's no arm64 binary available.

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

## Tooling Requirements

### Task

[Task](https://taskfile.dev/#/) is a great shell commands bootstrap solution (like `Make` but in Yaml) permitting you to make the same calls locally (for development phases) and within the CI/CD pipeline.

You want to get familiar with it? Read [this](https://tsh.io/blog/taskfile-and-gnu-make-for-automation/).

You can install it that way:

```bash
asdf plugin add task
# Will install the Task version refrenced in ./tool-versions
asdf install task $(asdf current task | tr -s ' ' | cut -d' ' -f2)
task --version
```

# License

Licensed under the [Apache License 2.0](LICENSE)
