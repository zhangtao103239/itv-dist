# i电视 分发仓库

本仓库仅用于分发 **i电视（iTV）** Android 安装包与自更新清单，**不含源码**。

## 下载

- 最新版本见 [Releases](../../releases)
- 两个渠道：
  - `vX.Y.Z` — 主分支（Android 5.0+）
  - `vX.Y.Z-legacy` — legacy 分支（Android 4.4 老设备）

## 自更新清单

| 渠道 | 清单文件 | 适用 |
|------|----------|------|
| master | `update-master.json` | 主分支 App |
| legacy | `update-legacy.json` | legacy 分支 App |

清单格式：

```json
{
  "versionCode": 1166,
  "versionName": "1.19.1",
  "url": "https://github.com/zhangtao103239/itv-dist/releases/download/v1.19.1/itv-1.19.1.apk",
  "notes": "更新说明"
}
```

App 通过 `https://raw.githubusercontent.com/zhangtao103239/itv-dist/main/update-*.json` 读取清单，国内建议走 ghproxy 类镜像。
