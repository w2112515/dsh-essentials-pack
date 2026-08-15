# DSH 精选起手包（DSH Essentials）

**为 [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness)（DSH）策展的整合方案：一次审阅，让全新的 DSH 获得类似 Codex 的完整能力基线——工作区侧边栏 UI、@路径引用、视觉、架构感知编码、多智能体团队、用量面板、安全审计、主题与通知。**

**English documentation: [README.md](README.md)**

通过 [DSH 插件市场](https://github.com/w2112515/dsh-plugin-marketplace)安装。这不是一堆杂烩：每个插件恰好覆盖一个能力面，且全部通过市场目录收录（静态校验通过、未归档、MIT）。

## 策展规则

DSH 发布仅数日，因此规则是务实的：**优先选择 100 star 以上的插件；某能力面没有百星选项时，按构建质量、许可证与维护活跃度精挑细选；连可靠候选都没有的槽位宁可空缺**——宁缺毋滥，绝不凑数。

## 内容

| 能力面 | 插件 | Stars | 安装方式 |
| --- | --- | --- | --- |
| 工作区 UI | [omdsh-dev/DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) | 970+ | 需审脚本（`prepare: tsdown`） |
| @路径引用 | [omdsh-dev/dsh-at-file](https://github.com/omdsh-dev/dsh-at-file) | 180+ | 一键 |
| 视觉 | [liustack/modlens](https://github.com/liustack/modlens) | 1600+ | 一键 |
| 架构感知编码 | [GanyuanRan/Aegis](https://github.com/GanyuanRan/Aegis) | 1000+ | 一键 |
| 多智能体团队 | [NanmiCoder/dsh-agent-teams](https://github.com/NanmiCoder/dsh-agent-teams) | 290+ | 手动（未随仓库提交构建产物） |
| 用量与配额 | [Ychris12138/dsh-usage-stats](https://github.com/Ychris12138/dsh-usage-stats) | 25 | 一键 · 精挑 |
| 安全审计 | [omdsh-dev/dsh-security-audit](https://github.com/omdsh-dev/dsh-security-audit) | 11 | 一键 · 精挑（只读） |
| 主题 | [KinGao294/dsh-skin](https://github.com/KinGao294/dsh-skin) | 11 | 一键 · 精挑 |
| 轮次通知 | [omdsh-dev/dsh-notification](https://github.com/omdsh-dev/dsh-notification) | 44 | 一键 · 精挑 |

**7 个一键安装 · 1 个需审阅脚本 · 1 个手动安装，共 9 项。** 市场会逐项显式标注状态并串行安装，首个失败即停止；需审阅脚本的条目逐字展示脚本内容并需你逐项同意——整合包绝不代为同意。

**记忆槽位暂时空缺。** 原选 [adoresever/graph-memory](https://github.com/adoresever/graph-memory)（510+ star）净室构建实测失败（`tsc` 引用了未声明的 `openclaw/plugin-sdk`），任何自动路径都装不上；我们不用未经验证的替代品凑数，持续观察 omdsh-dev/dsh-mnemon、Aik358/dsh-auto-memory 等候选。

### 明确排除

- **竞品插件市场**（已有数个）——一个市场出品的整合包不该安装另一个市场。
- **按调用付费的中继服务**——基线不应产生费用。
- **完整运行时**（如 `sandbase-harness`，580+ star）——agent 运行时不是插件基线。
- **恶搞插件**——有趣，但不是地基。

## 给市场扫描器

本仓库携带 `dsh-plugin` + `dsh-plugin-pack` 两个 topic，并提供 [`dsh.pack.json`](dsh.pack.json) 清单。条目为 `owner/repo` 引用，扫描时解析为稳定的仓库 id。
