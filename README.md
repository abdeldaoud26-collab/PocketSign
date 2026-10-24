# PocketSign personal iPhone build

This build packages the independent PocketSign customization of SideStore and the small Pocket Hello test app. It does not submit a contribution to the upstream SideStore maintainers.

The source archive preserves the original upstream snapshot, its license, dependency revisions, integrity manifest, and build symlinks. The workflow validates the snapshot and package tests, then uses Xcode 26.4 on GitHub's standard macOS runner to build actual iPhone binaries.

Download the `PocketSign-iPhone` artifact from a successful Actions run. It contains `PocketSign.ipa`, `PocketHello.ipa`, and SHA-256 checksums. Both apps still need signing with your Apple account before installation. No Apple credentials, certificates, or device pairing files belong in this repository or workflow.

Status: PocketSign 0.1.0 and Pocket Hello compiled successfully with the iPhoneOS 26.4 SDK in [build 1](https://github.com/abdeldaoud26-collab/PocketSign/actions/runs/40129152792). Source and packaging tests passed, and the downloaded IPAs passed device-platform, identity, permission, bundled-test, and SHA-256 checks. Both support iOS 15 or later. Apple-account signing and on-device testing remain necessary.
