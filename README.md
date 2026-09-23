# Cline Chinese Desktop releases

Public release artifacts and the stable HTTPS updater feed for the Chinese desktop build of Cline. This is an independent localization build of upstream Cline Desktop.

## Update feed

`https://github.com/439033521-maker/cline-desktop-zh-cn/releases/latest/download/latest.json`

Each stable release contains `latest.json`, a Windows x64 NSIS installer, its Tauri updater `.sig` signature, and `SHA256SUMS.txt`. The manifest points to the versioned installer asset in the same release.

The updater public key is embedded in the client. The production private signing key is held locally and is never committed to this repository or included in an artifact.

## Installation identity

The Chinese installer uses the `Cline Chinese` NSIS identity, separate from the official English `Cline` installation. The Tauri/WebView identifier remains `bot.cline.app` to preserve the existing Chinese profile. Existing user data is not packaged in releases.

Upstream: https://github.com/cline/cline
