# YuqiEngine-Skills

宇奇引擎 AI 助手的技能仓库。应用启动/检查更新时拉取 `skills/manifest.json`，按 SHA256 校验并同步变更文件到本地技能目录。

## 结构

- `skills/manifest.json` — 技能索引（slug/version/文件 SHA256 清单）
- `skills/<slug>/` — 单个技能文件夹（SKILL.md 主文件 + 附属文档/脚本/本地化）

## 更新技能

修改 `skills/<slug>/` 内文件 → 更新 manifest.json 中对应 version 与文件 SHA256 → 推送。客户端下次检查即自动同步。
