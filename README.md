# rust-analyzer-no-server

A VSCode extension derived from [rust-analyzer](https://github.com/rust-lang/rust-analyzer), but without the bundled binary. This extension tracks the latest version of the original extension.

## Why this extension exists

The original rust-analyzer extension comes with pre-built binaries, which limits its availability to specific platforms when published to the extension registry. This creates challenges for VSCodium users on alternative architectures (such as RISC-V and Loong64) where pre-built binaries are not available.

This extension solves that problem by providing a version of rust-analyzer that works across all platforms(i.e. no architecture requirement), as it doesn't include any pre-built binaries.

> While the `rust-analyzer` repository do provide a no-server variant in its releases, it is currently not available in the extension registry. For more context, you can refer to the discussion in https://github.com/rust-lang/rust-analyzer/issues/18578.

## How to use

1. Build and install rust-analyzer on your system
2. Install this extension
3. If the extension cannot locate your rust-analyzer binary, you may need to manually specify its path using the `rust-analyzer.server.path` setting in your `settings.json`
