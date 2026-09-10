# Ningshi

**Version 0.3.9**

Ningshi (凝时) is a KernelSU module. It helps you scroll less and keeps apps from running in the background.

## Features

- **Kill at launch.** App code is stopped before it runs.
- **Rules.** Always-on, lock-screen block, time windows, duration limit + cooldown; per-app and shared-pool groups.
- **WebUI.** Configure everything in the browser.

## Usage

Each app (or group) can combine four rules:

- **Always on** — block it all the time.
- **Lock screen** — block while the screen is off.
- **Time windows** — block within chosen hours (or allow only within them).
- **Duration** — allow a limited usage time; once used up, it resets the next day, or blocks for a **cooldown** period and then resets automatically.

The **+5 / +20** buttons grant a temporary **extension** (capped daily) for when you really need the app.

## Requirements

- KernelSU, arm64 device
- Kernel with kprobe enabled and the `binder_transaction` symbol in `/proc/kallsyms`

**For full documentation, build instructions, screenshots, and source code, see the main repository:**
[https://github.com/yuciss/ningshi]
