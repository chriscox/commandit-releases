# CommandIt

**An AI-powered command palette for developers.**

[![Latest version](https://img.shields.io/endpoint?url=https%3A%2F%2Fcommandit.ai%2Fbadges.json&query=%24.version.message&label=version&color=green)](https://github.com/chriscox/commandit-releases/releases/latest)
[![macOS](https://img.shields.io/endpoint?url=https%3A%2F%2Fcommandit.ai%2Fbadges.json&query=%24.macOS.message&label=macOS&color=blue)](#system-requirements)
[![Downloads](https://img.shields.io/github/downloads/chriscox/commandit-releases/total?color=brightgreen)](https://github.com/chriscox/commandit-releases/releases)
[![License](https://img.shields.io/badge/license-MIT-lightgrey)](LICENSE)

CommandIt lives one keystroke away. Hit `⌃Space`, search your snippets, fill in arguments, and paste straight into whatever app you're working in. It runs entirely on your Mac — your snippets stay local in SQLite, search is instant, and AI features are available on-device or via your own API key.

> 🌐 Visit **[commandit.ai](https://commandit.ai)** for the full feature tour, screenshots, and documentation.

---

## Download

➡️ **[Download the latest release](https://github.com/chriscox/commandit-releases/releases/latest)**

The DMG is **signed with a Developer ID certificate and notarized by Apple**, so macOS Gatekeeper will accept it on first launch — no right-click workarounds required.

## Install

1. Download `CommandIt-<version>.dmg` from the [latest release](https://github.com/chriscox/commandit-releases/releases/latest).
2. Open the DMG.
3. Drag **CommandIt** into your **Applications** folder.
4. Launch it from Applications (or Spotlight).
5. Follow the in-app onboarding to grant Accessibility permission (required for paste-into-any-app) and pick your global hotkey.

## System Requirements

- **macOS 15 (Sequoia) or later**
- **Apple Silicon recommended** (M1 or newer) — required if you want to use the on-device AI model. The core app, iCloud sync, and BYOK cloud AI (Claude / OpenAI) work on Intel Macs running macOS 15+.
- ~150 MB disk space (more if you opt in to downloading the on-device AI model)

## Auto-Updates

Once installed, CommandIt updates itself automatically via [Sparkle](https://sparkle-project.org). You don't normally need to come back here — the app will notify you when a new version is available and install it with one click. This page exists for first-time downloads, manual reinstalls, and people who prefer to grab the DMG directly.

## Verifying the Download

If you'd like to verify the DMG before installing, you can confirm the signature and notarization yourself:

```bash
# Confirm the bundle is signed by the expected Developer ID
codesign --verify --deep --strict --verbose=2 /Applications/CommandIt.app

# Confirm Gatekeeper accepts the bundle (notarization is checked here)
spctl -a -t exec -vv /Applications/CommandIt.app
```

You should see `accepted` and `source=Notarized Developer ID`.

## Links

- 🌐 **Website:** [commandit.ai](https://commandit.ai)
- 📚 **Help & Documentation:** [commandit.ai/help](https://commandit.ai/help)
- 💬 **Support:** [commandit.ai](https://commandit.ai)

## License

The contents of **this repository** (README, metadata, release artifact listings) are released under the [MIT License](LICENSE).

The CommandIt application itself is a separate product distributed under its own end-user license, shown to you on first launch and available on [commandit.ai](https://commandit.ai).
