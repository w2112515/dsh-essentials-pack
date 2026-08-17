# DSH 分类星数榜首（DSH Category Star Leaders）

**面向 [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness)（DSH）的整合方案，可通过 [DSH 插件市场](https://github.com/w2112515/dsh-plugin-marketplace)安装：市场目录每个分类中 star 数最高的收录条目。**

**English documentation: [README.md](README.md)**

## 选取规则

纯机械规则，不含编辑判断：

1. 取市场目录收录的全部条目（静态校验通过、未归档）。
2. 按市场分类分组（主题、记忆、界面、工具、模型接入、用量、技能、安全、消息渠道）。
3. 取每个分类中 GitHub star 数最高的一条。

数据来源：**2026-08-17** 目录快照（3543 条收录）。star 数随时间变化；下表是快照时刻的事实，每行链接到仓库页面可查看当前数值。

收录仅陈述目录事实（"快照日期时 X 分类 star 数最高"）。**不构成评价、背书或推荐。**

## 内容

| 分类 | 插件 | Stars（快照） | 安装方式（目录事实） |
| --- | --- | --- | --- |
| 技能 | [liustack/modlens](https://github.com/liustack/modlens) | 2486 | 一键安装 |
| 界面 | [omdsh-dev/DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) | 1720 | 需脚本审阅（`prepare`） |
| 记忆 | [sandbaseai/sandbase-harness](https://github.com/sandbaseai/sandbase-harness) | 608 | 手动 |
| 工具 | [superdesigndev/treg](https://github.com/superdesigndev/treg) | 428 | 一键安装 |
| 主题 | [kingOfSoySauce/dsh-liang-skin](https://github.com/kingOfSoySauce/dsh-liang-skin) | 66 | 一键安装 |
| 用量 | [Han-1413141/dsh-cost-meter](https://github.com/Han-1413141/dsh-cost-meter) | 57 | 一键安装 |
| 消息渠道 | [tencent-connect/dsh-qqbot](https://github.com/tencent-connect/dsh-qqbot) | 53 | 手动 |
| 模型接入 | [Mars-Sea/dsh-commandcode-provider](https://github.com/Mars-Sea/dsh-commandcode-provider) | 44 | 需脚本审阅（`prepare`） |
| 安全 | [THEWOLFWALKER/dsh-notifier](https://github.com/THEWOLFWALKER/dsh-notifier) | 31 | 一键安装 |

构成：**5 一键 · 2 需脚本审阅 · 2 手动 —— 共 9 项。** 市场会逐项显示真实安装状态，串行执行，首个失败即停止。需脚本审阅的条目会原文展示脚本内容并要求逐项同意；手动条目没有自动安装路径，市场会链接到对应仓库。整合包本身不代替你做任何同意。

## 面向市场扫描器

本仓库带有 `dsh-plugin` + `dsh-plugin-pack` 主题标签和 [`dsh.pack.json`](dsh.pack.json) 清单。条目为 `owner/repo` 引用，扫描时解析为稳定的仓库 id；某条目退出目录时会显示为不可用，而不是被隐藏。
