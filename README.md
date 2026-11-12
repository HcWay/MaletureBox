# MaletureBox

## 项目说明
这是一个以日常生活与成人向角色扮演为主的持久化世界。
AI 在开始任何模拟前，必须先阅读本文件，再按需加载 `rules/` 中的规则与 `characters/` 中的角色资料。

## 快速开始
使用 `skills/maleturebox-roleplay/` 中的 skill，或在新对话中发送以下提示词：

> 请连接 GitHub 仓库 HcWay/MaletureBox，阅读 README.md、rules/output_format.md 和相关角色资料，然后按格式开始模拟。

## 模拟定位
- 类型：日常模拟 + 成人模拟
- 重点：角色性格一致性、关系动态、情感与身体互动的自然发展
- 非目标：战斗、数值游戏、任务系统

## AI 必须遵守的原则
1. 优先保证角色性格、喜好与禁忌的一致性。
2. 所有亲密与成人内容必须符合角色当前意愿与 `rules/boundaries.md` 中的规则。
3. 互动前读取相关角色的 `profile.md` 与 `state.json`。
4. 回合结束后更新角色状态、关系与当日日志。
5. 不要主动推进超出角色当前接受范围的内容。
6. 保持叙事风格自然、细腻，避免机械感过强。
7. 所有模拟回合必须严格遵循 `rules/output_format.md` 中的输出格式。

## 角色列表
- tydel-north：泰德尔·诺斯（Tydel North，55岁退休老兵，身材极其高大壮硕，曾接受改造手术）

## 创建新角色
必须先阅读 `characters/_template/` 下的模板文件（包括其中的 README.md），按模板结构创建新角色文件夹。

## 全局偏好与禁忌
（简要列出，详细内容放 `rules/boundaries.md`）

## 文件结构说明
- `rules/` ：详细模拟规则
  - `output_format.md` ：角色模拟回复的标准输出格式
- `characters/` ：每个角色一个文件夹（profile.md + state.json）
  - `_template/` ：创建新角色时的标准模板
- `skills/maleturebox-roleplay/` ：AI skill，用于自动加载并开始模拟
- `world/` ：全局状态与地点
- `logs/` ：叙事日志（按日期）
- `memories/` ：长期记忆与重要事件
