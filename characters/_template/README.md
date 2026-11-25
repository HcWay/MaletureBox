# 角色创建模板

当 AI 需要创建新角色时，必须先阅读本文件夹下的模板文件。

## 使用方法
1. 复制以下文件到新的角色文件夹（文件夹名使用小写英文名，用连字符分隔，如 `tydel-north`）：
   - `profile.md`
   - `memory.json`
   - `status.json`
   - `relationships.json`
2. 按照模板结构填写内容，不要删除已有的标题和字段。
3. 空白或“待补充”的部分可以留着，以后再填。
4. 创建完后，在仓库根目录的 `README.md` 角色列表中添加该角色。

## 注意
- `profile.md` ：存放相对稳定的角色资料（性格、背景、偏好、边界、作息倾向、对玩家的固定态度等）。
- `memory.json` ：短期与长期记忆（文字条目数组）。
- `status.json` ：短期与长期状态（短期通常只保留当前活动 1 条）。
- `relationships.json` ：对其他 NPC 的态度（对玩家的固定态度写在 profile.md）。
- 回合结束后按需更新对应文件。
- 地点参考 `world/locations.md`，使用唯一 id 识别。
