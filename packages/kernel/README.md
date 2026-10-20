---
title: "@e2e-dev/kernel"
tags: [e2e, kernel, hosted, browsers, chromium, testing]
category: packages
created: "2024-01-01"
updated: "2026-10-20"
source: external
type: index
status: stable
lifecycle: active
---

# 💡 概述

[Kernel](https://kernel.sh) hosted browsers for [`e2e`](https://www.npmjs.com/package/e2e):
`web({ browser: kernel() })` runs a web target in Kernel's hosted Chromium.

---

## 🚀 快速开始

### Install

```bash
npm install --save-dev @e2e-dev/kernel @onkernel/sdk
```

### Usage

```ts title="e2e.config.ts"
import type { E2EConfig } from 'e2e';
import { web } from '@e2e-dev/web';
import { kernel } from '@e2e-dev/kernel';

export default {
  targets: [{ engine: web({ browser: kernel({ stealth: true }), viewport: null }), app: { url: 'https://staging.example.com' } }],
  workers: 4,
} satisfies E2EConfig;
```

`KERNEL_API_KEY` comes from the run's environment. `kernel(options)` takes
Kernel's create-browser body as is (`stealth`, `headless`, `timeout_seconds`,
`profile`, `proxy_id`, `viewport`, `tags`, ...) plus the lease `scope`:
`worker` (default) is one browser per worker slot for the run, `attempt` a
fresh browser per test attempt. Every browser is tagged with the run, target,
and slot, `timeout_seconds` defaults to 600 so Kernel deletes a browser a dead
worker never released, and each lease logs its live view URL when Kernel
gives one. On a headed browser, an attempt that records video (`--video`, or
a test's `video` option) gets a Kernel replay of the browser's screen as its
`video/replay.mp4`; a headless browser and `replay: false` get the page
screencast.

---

## ⚡ 功能

「待补充」

---

## ⚙️ 技术栈

「待补充」

---

## 📊 指标

「待补充」

---

## 🏛️ 设计

「待补充」

---

## 📁 目录

「待补充」

---

## 🔗 资源

- [Kernel](https://kernel.sh)
- [Integration docs](https://e2e.tester.army/docs/integrations/kernel)

## License

Apache-2.0