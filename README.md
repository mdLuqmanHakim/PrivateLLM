# PrivateLLM

An on-device AI chatbot with a live knowledge graph brain. All models run locally via WebGPU — no API keys, no internet required after the first model download.

## Requirements

- Node.js 18+
- npm
- A device with a GPU (for WebGPU inference)

## Quick start (dev)

```bash
npm install
npm start
```

## Build installers

```bash
# All platforms (run on each OS for best results)
npm run build

# Specific platform
npm run build:mac    # → dist/Odysseus-1.0.0.dmg
npm run build:win    # → dist/Odysseus Setup 1.0.0.exe
npm run build:linux  # → dist/Odysseus-1.0.0.AppImage
```

Output goes to the `dist/` folder.

## Notes

- First run requires internet to download the selected model (~0.8–2.2 GB depending on choice)
- Models are cached by the browser engine after first download
- WebGPU is required — works on Chrome/Electron on devices with a GPU
- macOS arm64 (Apple Silicon) and x64 both supported
# PrivateLLM
