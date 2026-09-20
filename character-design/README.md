# Character Design 角色资产设计

通用角色与人物资产图设计技能:把想法变成稳定、可复用的角色资产——角色 DNA、身高比例锁、三视图一致性、服装状态、道具锚点与 AI 图像/视频提示词流程。

这个 skill 适合做:

- 人物资产图 / 角色设定图 / 角色卡 (character sheet)
- 三视图转面 (W0 front / side / back turnaround) 与一致性维护
- 身高比例锁、面部锚点、常驻道具锁定
- 服装状态阶梯 (wardrobe ladder)、表情系统与姿态设计
- 群像 / 角色关系矩阵、类型化选角包
- 多镜头 / 多段视频中的角色一致性 (identity anchors) 与视频可用性质检

## 工作流

```
角色目的 -> 角色DNA -> 身高/比例锁 -> 面部与常驻道具锁定
-> W0 正/侧/背三视图 -> 服装状态阶梯 -> 表情与动作姿态
-> 最终角色设定图 -> 视频试镜 / 可用性质检
```

核心原则:让角色有记忆点、稳定、可拍摄,而不是只追求好看。

## 目录结构

- `SKILL.md` — 轻量运行时入口,默认先读这个。
- `SECTIONS/` — 12 个专题章节(角色 DNA 七字诀、一致性维护、关系设计、表情姿态、负面清单、提示词模板、中国传统角色、人物原型库、完整流程、参考图哲学、群像设计、多智能体协作),按需加载。
- `references/` — 深度参考资料(骨相/面部结构、前置化角色资产、完整手册、真人短剧选角资产、短剧角色生产系统),仅在对应专项需求时打开。
- `agents/openai.yaml` — agent 接入配置。

## 安装

在本仓库根目录执行:

```bash
mkdir -p ~/.codex/skills
cp -R character-design ~/.codex/skills/
```

Claude 风格技能目录:

```bash
mkdir -p ~/.claude/skills
cp -R character-design ~/.claude/skills/
```

## 使用示例

```text
使用 $character-design,帮我给一个奇幻世界的快递员设计生产级角色资产包:身份锚点、身高比例锁、面部锚点、服装状态、标志性道具几何、表情、动作姿态和视频可用性检查。
```

```text
使用 $character-design,基于这张参考图重设计角色,保留原有体型、身高、嘴型、发型、服装类别和腰部道具;先做比例锁,再出最终设定图。
```

## 来源与许可

本技能来自 [khanhhuyenngo985-sys/character-scene-design-skills](https://github.com/khanhhuyenngo985-sys/character-scene-design-skills)(MIT License),集成时按本仓库结构补充了 `metadata` 路由字段。
