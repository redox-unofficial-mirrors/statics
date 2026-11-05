# Redox static build assets

This repository mirrors selected assets originally served by `static.redox-os.org` so that Redox builds can retrieve them from GitHub. It is an unofficial mirror for build inputs.

See [Releases](https://github.com/redox-unofficial-mirrors/statics/releases) for available snapshots. For reproducible builds, use a specific release tag for the host and target and verify each archive against its pinned SHA-256.

## Initial toolchain set

Host `x86_64-unknown-linux-gnu`, target `x86_64-unknown-redox`. The original paths are relative to `https://static.redox-os.org/toolchain/x86_64-unknown-linux-gnu/x86_64-unknown-redox/`.

| File | Bytes | SHA-256 |
| --- | ---: | --- |
| `clang-install.tar.gz` | 184151121 | `fcf965f0a08fabb060a8fe8b96372ed95f3d8bff7c087b613a439a1cda003115` |
| `gcc-install.tar.gz` | 98465573 | `4bb5d1691d727546dc5064da794d798e9157cb85be8d463ebf7545bc01d9c362` |
| `rust-install.tar.gz` | 175167112 | `ecfe0e260cc7544b0e29ec4f217eacd0e6802248cf70e2fb689ce87808bfa2bb` |

This private mirror is for internal build use. The archived bytes and included notices are preserved. GCC and its runtime components, LLVM/Clang and Rust retain their respective upstream and bundled third-party terms. Verify the applicable notices and corresponding source before sharing the archives outside the current private access scope.
