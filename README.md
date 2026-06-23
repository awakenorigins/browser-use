# browser-use — Full-featured browser automation with session support

> Automates real browser interactions — form filling, screenshots, data extraction, and multi-tab workflows. Supports headless Chromium, real Chrome with your login sessions, and cloud browsers.

[![OpenClaw Skill](https://img.shields.io/badge/OpenClaw-Skill-blueviolet)](https://github.com/NachaFromMars)

## Overview
browser-use is a browser automation skill that controls a browser via structured commands. It supports three modes: headless Chromium for fast isolated runs, real Chrome with profile support for authenticated sessions, and a remote cloud browser. Use `state` to get a numbered list of clickable elements, then interact by index — no CSS selectors needed. Multi-tab and download support are included.

## Features
- **chromium** — headless, fast, isolated
- **chromium --headed** — visible Chromium window
- **real** — real Chrome binary; `--profile "Name"` copies your login sessions and cookies
- **remote** — cloud-hosted browser with proxy support
- Index-based interaction: no fragile CSS selectors
- Multi-tab management, `eval` for JS execution, file download

## Usage / Quick Start
```bash
# Check prerequisites
browser-use doctor

# Core workflow
browser-use open https://example.com
browser-use state                  # get numbered clickable elements
browser-use click 5                # click element #5
browser-use input 3 "search text"  # fill input #3
browser-use screenshot             # capture current page
```

## Trigger Keywords (OpenClaw)
navigate website, fill form, take screenshot, extract from web page, browser automation

## Related Skills
- [agent-browser](https://github.com/NachaFromMars/agent-browser) — lightweight Rust-based browser CLI for simpler use cases

---
Part of the [NachaFromMars](https://github.com/NachaFromMars) OpenClaw skill ecosystem.
