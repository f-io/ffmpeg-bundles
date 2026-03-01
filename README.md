# ffmpeg-bundles

Prebuilt FFmpeg / FFplay binary bundles intended for embedding into applications.

This repository provides minimal, platform-specific builds of FFplay that are designed to be:

- Self-contained
- Suitable for redistribution inside desktop applications
- Built in CI for reproducibility
- Versioned via GitHub Releases

## Target Platforms

- macOS arm64 (Apple Silicon)
- Windows x64

## Purpose

These bundles are **not** general-purpose FFmpeg distributions.
They are intended for controlled use within application environments where:

- No external runtime dependencies should be required
- A consistent FFmpeg/FFplay version is desired
- Reproducible builds matter

## Distribution Model

Binaries are distributed exclusively via GitHub Releases.

Each release contains platform-specific archives, for example:

- `ffplay-macos-arm64.zip`
- `ffplay-win-x64.zip`

Applications can fetch these assets during CI and embed them into their own distribution packages.

## License

FFmpeg is licensed under LGPL/GPL depending on build configuration.
See the corresponding FFmpeg release and build configuration for details.