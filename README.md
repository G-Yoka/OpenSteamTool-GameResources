# GameResources

## 涓枃
杩欐槸涓€涓嫭绔嬬殑娓告垙璧勬簮浠撳簱锛岀敤浜庣粰 OpenSteamTool Manager 鎻愪緵鍙笅杞姐€佸彲鏍￠獙銆佸彲瀹夎鐨勬父鎴忚祫婧愬寘銆傚畠涓嶅睘浜?OpenSteamTool 鏍稿績椤圭洰鏈韩銆?
### 缁撴瀯

- `manifest.json`锛氳祫婧愮储寮曪紝鐢辩鐞嗗櫒璇诲彇銆?- `packages/`锛歚manifest.json` 寮曠敤鐨?ZIP 璧勬簮銆?
### 瑙勫垯

- 姣忎釜璧勬簮鍖呴兘蹇呴』鍦?`manifest.json` 涓彁渚?SHA-256銆?- 绠＄悊鍣ㄤ細鍦ㄥ畨瑁呭墠鏍￠獙 SHA-256銆?- 寤鸿浣跨敤 `main` 鍒嗘敮浣滀负鍥哄畾鍙戝竷鍏ュ彛銆?
## English
This is a separate game resource repository used by OpenSteamTool Manager to provide downloadable, verifiable, and installable game resource packages. It does not belong to the OpenSteamTool core project itself.

### Structure

- `manifest.json`: resource index consumed by the manager.
- `packages/`: ZIP assets referenced by `manifest.json`.

### Rules

- Each package must include a SHA-256 hash in `manifest.json`.
- The manager verifies the SHA-256 before installing.
- The `main` branch is recommended as the fixed release entry.
