# OpenYSM

[简体中文](README.md) | **English** | [日本語](README.ja.md)

![OpenYSM logo](images/brand.png)

**Open-source alternative to Yes Steve Model (YSM), based on YSM 2.6.5 for Minecraft 1.20.1 Forge.**

This repository contains source code corresponding to the YSM 2.6.5 (April 2026) version, including the Minecraft 1.20.1 Forge implementation.

> **Development status:** Not production-ready. Decompiled or reconstructed naming may be inaccurate; rendering problems and other bugs may occur. Please report issues with screenshots and logs whenever possible.

## Why open source?

The project aims to support studying, modifying, and developing an open alternative to the newer YSM implementation. The project notes that tools already exist for decrypting affected YSM models, reducing the practical value of the relevant encryption mechanism.

## Differences and features

- Rewrites model loading and rendering in Java instead of depending on native code, improving portability to platforms such as macOS and alternative CPU architectures.
- Supports existing encrypted YSM models.
- Provides `/openysm cache dump` to export models obtained from servers for debugging.
- Implements Ogg Opus audio decoding, WebP/AVIF texture decoding, YSM-compatible client/server handshake, and model loading/rendering.

## Known unfinished work

- Submodel animation controllers
- SIMD rendering optimizations
- Correct handling of the default model during server handshakes
- Compatibility testing with older binary and unencrypted models
- YSGPHeader generation

These items are **not** presented as completed features.

## Licenses

The **source code** is distributed under the [MIT License](LICENSE). Bundled model assets have separate terms:

- Default model: **CC0**
- Wine Fox model: **CC BY-NC-SA 4.0** (attribution, noncommercial use, share-alike)

Check the applicable license before redistributing models.

## Contributing

Issues and contributions are welcome, particularly reproducible rendering issues and compatibility reports. This repository targets development and research use rather than a stable production release.
