# Nexus DataOps Control Center

An offline-first operations workspace for exploring data pipelines, run history, data contracts, lineage, connectors, incidents, and an asset catalog.

## Run it

- Fastest: double-click standalone.html.
- Source version: open index.html in a current Chromium, Edge, or Firefox browser.
- Windows shortcut: double-click Launch Nexus.bat.
- No install, server, account, API key, or internet connection is required.

The interface is a local simulation. Pipeline runs and connector checks use bundled sample records; they do not connect to external systems or execute real ETL jobs. Changes are saved in browser storage on the current device. Use Settings → Export JSON backup to keep a portable copy.

## What is included

- Operations overview with reliability signals, recent runs, and workflow activity.
- Pipeline inventory, pause/resume controls, workflow creation, and simulated run playback.
- Execution history with status filters, detail inspection, and CSV export.
- Data contracts, quality rules, and a local rule-evaluation action.
- Interactive lineage explorer, connector registry, incident triage, and searchable asset catalog.
- English and Simplified Chinese UI, local JSON backup/restore, and responsive layouts.
- A no-dependency source version plus a generated single-file standalone.html for easy sharing.

## Rebuild the single-file version

Install Node.js 18 or newer, then run: node scripts/build.mjs

The build embeds the CSS and JavaScript into standalone.html. It does not download packages or contact a service.

## Project layout

- index.html — source entry point
- standalone.html — self-contained browser build
- styles.css — application styling
- src/data.js — bundled sample workspace
- src/i18n.js — English and Simplified Chinese labels
- src/core.js — local persistence and simulation logic
- src/views.js — page rendering
- src/app.js — UI events and lifecycle cleanup
- scripts/build.mjs — single-file builder
- Launch Nexus.bat — Windows launch shortcut

## Nexus 数据运营中枢

这是一个离线优先的数据运营工作台，用于查看数据管道、运行记录、数据契约、血缘关系、连接器、告警和资产目录。

- 直接运行：双击 standalone.html。
- 源码入口：使用 Edge、Chrome 或 Firefox 打开 index.html。
- Windows 快捷方式：双击 Launch Nexus.bat。
- 无需安装、服务器、账号、密钥或网络连接。

页面中的管道运行和连接器检查都是本地模拟，不会连接外部系统，也不会执行真实 ETL。更改保存在当前浏览器的本地存储中；可在“设置”里导出 JSON 备份。
