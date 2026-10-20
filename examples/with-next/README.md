---
title: e2e with Next.js
tags: [e2e, nextjs, react, example, testing, web]
category: examples
created: "2024-01-01"
updated: "2026-10-20"
source: external
type: index
status: stable
lifecycle: active
---

# 💡 概述

A Next.js App Router greeting app with three locator tests and two agent tests.

![Next.js example app with the greeting "Hello, Ada!"](screenshot.png)

---

## 🚀 快速开始

Use Node 22.22.3+, 24.8+, or 26+. From this folder:

```bash
npm install
npm run test:e2e
```

The runner starts the app at `http://localhost:3100`.
It downloads Chromium on the first run if needed.

### Agent tests

Set a [Vercel AI Gateway](https://vercel.com/docs/ai-gateway) key:

```bash
AI_GATEWAY_API_KEY="your-key" npm run test:e2e
```

Without the key, the agent tests skip. Add `-- --no-cache` to use fresh
model calls. Results are in `.e2e/report.json`.

See [e2e.config.ts](e2e.config.ts) and [tests/](tests/) for the setup.
For your own app, follow the [Quickstart](https://e2e.tester.army/docs/quickstart).

---

## ⚡ 功能

「待补充」

---

## ⚙️ 技术栈

- Next.js 16.3 (App Router)
- React
- e2e 0.15.2
- @e2e-dev/web 0.11.1
- Node.js 22+

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

- [Quickstart](https://e2e.tester.army/docs/quickstart)

Last checked with e2e 0.15.2, @e2e-dev/web 0.11.1, Next.js 16.3, and Node 22.