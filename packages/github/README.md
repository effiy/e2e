---
title: "@e2e-dev/github"
tags: [e2e, github, reporter, ci, pull-request]
category: packages
created: "2024-01-01"
updated: "2026-10-20"
source: external
type: index
status: stable
lifecycle: active
---

# 💡 概述

The GitHub reporter for [`e2e`](https://www.npmjs.com/package/e2e).
From GitHub Actions, every run becomes one pull request comment, edited in
place on reruns, and the same text lands in the job summary.

---

## 🚀 快速开始

```bash
npm install --save-dev @e2e-dev/github
```

```ts title="e2e.config.ts"
import type { E2EConfig } from 'e2e';
import { web } from '@e2e-dev/web';
import { github } from '@e2e-dev/github';

export default {
  targets: [{ engine: web(), app: { url: 'http://localhost:3000' } }],
  reporters: ['list', github()],
} satisfies E2EConfig;
```

The job needs `permissions: pull-requests: write` and the step that runs
`e2e` needs `GITHUB_TOKEN: ${{ github.token }}` in its `env`. Matrix replicas
of one job pass a `key` so their comments stay apart. When the reporter cannot
post (another CI, a push, a fork's read-only token) it says why in one summary
row and never changes the run's exit code.

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

- [GitHub integration docs](https://e2e.tester.army/docs/github)

## License

Apache-2.0