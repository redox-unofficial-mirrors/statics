# Redox static files and signed packages

Unofficial distribution of Redox build inputs and binary packages. Download
through https://redox-statics.pages.dev using the original request paths.
Cloudflare redirects to this repository's public Release attachments; it does
not store the binary files.

## Packages

The distribution retains the complete official package collection and applies
verified locally maintained x86_64 build overrides. Official-derived packages
are verified before re-signing; their installed files, permissions and links
are preserved. These are signatures from this distribution, not official Redox
signatures. The private signing key is never distributed.

All architectures use the same public key at
https://redox-statics.pages.dev/pkg/id_ed25519.pub.toml. Its file SHA-256 is:

```text
0c581ffbf05585a41ebe1a0fc94f83283b47382fd4f79a4138d9f6641e8b4ec0
```

Fresh builds and newly generated images use this source. Existing installed
systems are not automatically migrated to a different trust key; preserve your
data and rebuild the image when changing from an older package source.

## Release layout

Package snapshots cover x86_64, aarch64, i586 and riscv64gc. The x86_64 snapshot
has main and lib-prefixed parts to stay below GitHub's 1000-attachment limit.
Original attachment names are retained. Each snapshot is verified before the
redirects switch to it; active snapshots are not replaced file by file.
Releases remain mutable, and obsolete snapshots are removed after acceptance
and active-reference checks.

Toolchain archives, firmware and config.sub retain their existing paths.
See the Release descriptions and supplied source/license material for provenance
and redistribution terms. All software retains its applicable upstream license.
