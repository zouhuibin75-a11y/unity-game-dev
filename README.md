# Unity Game Development Skill

面向 AI 编程助手的 Unity 游戏开发 skill，覆盖从 JS/H5 Demo 或游戏设计文档出发，实现可运行的 Unity 最小玩法闭环、组织项目结构和完成交付验证。

本仓库保存 skill 的说明、参考文档、模板与初始化脚本。它本身不是可直接在 Unity Editor 中打开的游戏工程。

## 使用方式

1. 将本仓库放入所用 AI 助手的 skills 目录，并保留目录名 `unity-game-dev`。
2. 在助手中调用该 skill，并提供已有 JS/H5 Demo、设计文档及目标 Unity 项目路径。
3. 按 [SKILL.md](SKILL.md) 完成项目发现、最小玩法闭环实现与验证。

已有 Demo 时，skill 要求先读取原型，并复用原型的数据结构、关卡布局和计分规则。具体要求见 [发现清单](references/discovery-checklist.md)。

## 文件结构

```text
SKILL.md                             # skill 入口与工作流程
references/                          # 项目结构、编码、玩法、UI、平台与交付规范
assets/templates/                    # C# 与 link.xml 模板
scripts/init_unity_project_structure.py  # 创建 Assets/_Project 目录骨架
```

模板使用 `.cs.txt` / `.xml.txt` 扩展名。放入实际 Unity 工程时，需按 `SKILL.md` 的说明去掉末尾 `.txt` 并调整命名空间。

## 来源

从项目中的 `unity-game-dev-1.0.3_副本.zip` 整理，保留原始 skill 内容；移除了 `__MACOSX` 和来源平台 `.knot` 元数据。
