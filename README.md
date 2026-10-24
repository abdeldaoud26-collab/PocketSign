# PocketSign personal iPhone build

This build packages the independent PocketSign customization of SideStore and the small Pocket Hello test app. It does not submit a contribution to the upstream SideStore maintainers.

The source archive preserves the original upstream snapshot, its license, dependency revisions, integrity manifest, and build symlinks. The workflow validates the snapshot and package tests, then uses Xcode 26.4 on GitHub's standard macOS runner to build actual iPhone binaries.

Download the `PocketSign-iPhone` artifact from a successful Actions run. It contains `PocketSign.ipa`, `PocketHello.ipa`, and SHA-256 checksums. Both apps still need signing with your Apple account before installation. No Apple credentials, certificates, or device pairing files belong in this repository or workflow.

Status: build prepared; compilation and on-device testing have not yet been completed.
