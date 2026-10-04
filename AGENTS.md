# Agent instructions

## Releases are recipe-only

BellPad releases publish only the PadMint recipe (`BellPad-vX.Y.Z-padmint.json`, a copy of `padmint.json`) and its `SHA256SUMS`; players build the app themselves with PadMint. Bump `version.json` with each release.

Never publish, re-publish, or restore an IPA, APK, or macOS build, and do not add app download links: the app is compiled from the Animal Crossing decompilation. Publishing a ready-made app needs the maintainer's explicit approval first.

Every release artifact must pass `python3 ~/.codex/release-gate/release_gate.py <artifact>` on the maintainer's machine before it is published. A failure is a stop, not a note.
