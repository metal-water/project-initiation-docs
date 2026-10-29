# 项目立项报告与决议 Skill

根据游戏研发项目材料和用户模板，编写或修订中文立项报告与立项决议。两份文稿共用项目事实，支持原稿修改、指定参考材料改写、日期计划、预算人数标黄及玩法配图。

## 使用

将本仓库放入 Codex 的 skills 目录，文件夹名为 `project-initiation-docs`。调用示例：

```text
请用 $project-initiation-docs，根据这个项目的材料和模板生成立项报告与立项决议。
主体：[公司全称]
材料：[文件夹或链接]
周期：[准确区间、按原材料，或授权拆分阶段]
预算和人员人数：[标黄留空、仅标黄，或已确认数据]
```

已配置GitHub访问权限时，也可用Git安装：

```powershell
git clone https://github.com/metal-water/project-initiation-docs.git "$env:USERPROFILE\.codex\skills\project-initiation-docs"
```

目标目录已存在时，先检查现有版本，避免覆盖自定义修改。

## 内容

- [Skill入口](SKILL.md)：新写、旧稿修订、指定参考改写三种模式。
- [框架与模板](references/frameworks.md)：报告八章框架、决议结构及两份Word参考。
- [可复用Prompt](references/prompts.md)：8组常用任务提示。
- [字段与周期](references/fields-and-timeline.md)：标黄与留空、授权时间安排、预算跨期和下游数据清理。
- [材料与图片](references/materials-and-images.md)：本地材料、嵌套线上文档、PPT权限和游戏截图。
- [中文行文与humanizer](references/writing-and-humanizer.md)：正式自然的文稿风格。
- [用户原话](references/conversation-evidence.md)：15个相关对话、39条去重输入和来源索引。
- [项目实例](references/project-cases.md)：历史要求的变化与例外。

模板中的公司、项目和日期均为原始示例。新任务采用当前用户指令，不默认复用历史项目的年份、金额或审批事实。

## 版本与验证

当前版本为1.0.0，整理于2026年10月28日。已完成技能结构、UTF-8、内部引用、模板副本哈希和五类场景推演检查。实际生成的Word仍需逐页检查版面。

## 第三方内容

集成 [blader/humanizer](https://github.com/blader/humanizer) 3.1.0，随包保留[原文](references/humanizer-upstream.md)和[MIT许可](references/humanizer-LICENSE.txt)。该许可对应humanizer，不自动扩展到本仓库的内部模板和对话材料。
