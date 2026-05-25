# GameResources

# 资源仓库 / Resource Repository

这是一个独立的游戏资源仓库，用于给 OpenSteamTool Manager 提供可下载、可校验、可安装的游戏资源包。它不属于 OpenSteamTool 核心项目本身。

This is a separate game resource repository used by OpenSteamTool Manager to provide downloadable, verifiable, and installable game resource packages. It does not belong to the OpenSteamTool core project itself.

## 结构 / Structure

- `manifest.json`: 资源索引 / resource index consumed by the manager
- `packages/`: 被 `manifest.json` 引用的 ZIP 资源 / ZIP assets referenced by `manifest.json`

## 规则 / Rules

- 每个资源包都必须在 `manifest.json` 中提供 SHA-256。
- 管理器会在安装前校验 SHA-256。
- 建议使用 `main` 分支作为固定发布入口。

- Each package must include a SHA-256 hash in `manifest.json`.
- The manager verifies the SHA-256 before installing.
- The `main` branch is recommended as the fixed release entry.
