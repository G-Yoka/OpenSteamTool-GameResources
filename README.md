# GameResources

这是一个独立的游戏资源仓库，用于给 OpenSteamTool Manager 提供可下载、可校验、可安装的游戏资源包。

### 结构

- `manifest.json`：资源索引，由管理器读取。
- `packages/`：`manifest.json` 引用的 ZIP 资源。

### 规则

- 每个资源包都必须在 `manifest.json` 中提供 SHA-256。
- 管理器会在安装前校验 SHA-256。
