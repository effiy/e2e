---
title: "@e2e-dev/limrun"
tags: [e2e, limrun, hosted, mobile, testing, ios, android]
category: packages
created: "2024-01-01"
updated: "2026-10-20"
source: external
type: index
status: stable
lifecycle: active
---

# 💡 概述

Run `@e2e-dev/mobile` tests on Limrun iOS simulators and Android emulators.
Each worker gets a device, its build installed, and automatic cleanup.

---

## 🚀 快速开始

```ts
import { mobile } from '@e2e-dev/mobile';
import { limrun } from '@e2e-dev/limrun';

const engine = mobile({ platform: 'ios', device: limrun() });
```

Set `LIMRUN_API_KEY` in the run environment and install `@limrun/api`.
Android also requires `adb` on `PATH` for the driver's tunnel.

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

- [Integration guide](https://e2e.tester.army/docs/integrations/limrun)
- [App-flow example](../../examples/with-limrun)