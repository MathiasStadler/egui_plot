# project path to explore this

## check sccache is started - start in separate terminal and look :-)
<!-- keep the format -->
-- **SCCACHE_LOG=debug SCCACHE_START_SERVER=1 SCCACHE_NO_DAEMON=1 sccache**
<!-- keep the format -->
- **sccache  --show-stats**
- sccache  --stats-format=text --show-stats
<!-- keep the format -->
## rust version
<!-- keep the format -->
```bash <!-- markdownlint-disable-line code-block-style -->
rustc -vV
rustc 1.89.0 (29483883e 2025-08-04)
binary: rustc
commit-hash: 29483883eed69d5fb4db01964cdf2af4d86e9cb2
commit-date: 2025-08-04
host: x86_64-unknown-linux-gnu
release: 1.89.0
LLVM version: 20.1.7
```
<!-- keep the format -->
## Is there a list of all cfg features?  [![alt text][1]](https://stackoverflow.com/questions/41742046/is-there-a-list-of-all-cfg-features#41743950>)
<!-- keep the format -->
## See what targets Rust supports [![alt text][1]](https://stackoverflow.com/questions/49453571/how-can-i-set-default-build-target-for-cargo)

rustc --print target-list

rustup target  list |wc -l => 99

rustup target  list --help
List installed and available targets

rustc --print target-list | wc -l => 290
Usage:
    <!-- markdownlint-disable MD033 -->
    --print <INFO>[=<FILE>]
    <!-- markdownlint-enable MD033 -->
    Compiler information to print on stdout (or to a file)
    INFO may be one of
    all-target-specs-json
    calling-conventions
    cfg|check-cfg
    code-models
    crate-name
    crate-root-lint-levels
    deployment-target
    file-names
    host-tuple
    link-args
    native-static-libs
    relocation-models
    split-debuginfo
    stack-protector-strategies
    supported-crate-types
    sysroot
    target-cpus
    target-features
    target-libdir
    target-list
    target-spec-json
    tls-models

rustup target  list

## active toolchain
<!-- keep the format -->
- **rustup show |sed -n '/active toolchain/,/^$/p'**
<!-- keep the format -->
## cargo-chef prepare recipe.json
<!-- keep the format -->
cargo chef prepare --recipe-path recipe.json
<!-- keep the format -->
## cargo cook the binary
<!-- keep the format -->
cargo chef cook --recipe-path recipe.json
<!-- keep the format -->

<!-- keep the format -->
<!-- make folder and download the link sign vai curl -->
<!-- mkdir -p img && curl --create-dirs --output-dir img -O  "https://raw.githubusercontent.com/MathiasStadler/link_symbol_svg/refs/heads/main/link_symbol.svg"-->
<!-- Link sign - Don't Found a better way :-( - You know a better method? - **send me a email** -->
<!-- keep the format -->

<!-- keep the format -->
>[!NOTE]
>Symbol to mark web external links [![alt text][1]](./README.md)
<!-- make folder and download the link sign vai curl -->
<!-- mkdir -p img && curl --create-dirs --output-dir img -O  "https://raw.githubusercontent.com/MathiasStadler/link_symbol_svg/refs/heads/main/link_symbol.svg"-->
<!-- Link sign - Don't Found a better way :-( - You know a better method? - send me a email -->
[1]: ./img/link_symbol.svg
<!-- keep the format -->
