# Creator – Awakening the Right Hand of Desktop Apps

**Creator** is an open-source Chromium browser, but it is far more than that.  
It introduces a brand-new launch mode called **Chromium Host Mode**, which turns any compiled 64-bit desktop application (WinForm, MFC, WPF, etc.) into a **real Chromium browser instance**.

> Compilation is no longer the end of capability – it is the starting point of the Web + AI ecosystem.

[![GitHub release](https://img.shields.io/github/v/release/AIGCEra/Creator)](https://github.com/AIGCEra/Creator/releases/tag/FirstRelease)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

---

## 🚀 Core Idea

Traditional desktop applications, once compiled, have their functional boundaries fixed (the **left hand**).  
But every application hides a Web world composed of hundreds of standard HTML elements (the **right hand**), which has long been asleep.

**Creator awakens this right hand**, granting any `.exe` at runtime:

- Full Chromium multiprocess architecture (browser process + Renderer/GPU/Utility)
- Chrome Tab Groups
- Chrome DevTools Protocol (CDP)
- Chrome extension ecosystem
- Support for all LLM / AI Agent toolchains

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| **Non‑invasive** | No source code modification, no code injection – just launch via Loader |
| **Instant browserification** | Turns `appName.exe` into a Chromium browser process |
| **Full CDP support** | Any CDP‑compatible tool (Puppeteer, Playwright, OpenClaw, etc.) can control the app |
| **Native ↔ Web hybrid** | Mix WinForm controls, WPF, MFC CView with HTML elements inside the same tab |
| **Window Nucleus** | At runtime, “move out” any child window and re‑layout it to enable capability emergence |
| **Native AI Agent interface** | Agents just point their `executablePath` to the Loader and control the desktop app like a browser |

---

## 📦 Download & Installation

- Source code: [https://github.com/AIGCEra/Creator](https://github.com/AIGCEra/Creator)
- First release: [https://github.com/AIGCEra/Creator/releases/tag/FirstRelease](https://github.com/AIGCEra/Creator/releases/tag/FirstRelease)

After installation, the Loader is located at:
