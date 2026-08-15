# DSH Essentials

A curated solution pack for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) (DSH), installable through the [DSH Plugin Marketplace](https://github.com/w2112515/dsh-plugin-marketplace). The goal: give a fresh DSH a **complete, Codex-grade capability baseline** in one reviewed action — not a pile of plugins, but a coherent set where each item covers one capability area.

DSH is days old, so the honest curation rule is: **100+ stars preferred; where no 100-star option exists in a capability area, the pick is hand-selected** for build quality, license, and maintenance activity. Every item below is admitted by the marketplace catalog (statically validated, non-archived, MIT).

## Contents

| Capability | Plugin | Stars | Install |
| --- | --- | --- | --- |
| Workspace UI | [omdsh-dev/DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) | 970+ | Script review (`prepare: tsdown`) |
| @path references | [omdsh-dev/dsh-at-file](https://github.com/omdsh-dev/dsh-at-file) | 180+ | One-click |
| Vision | [liustack/modlens](https://github.com/liustack/modlens) | 1600+ | One-click |
| Architecture-aware coding | [GanyuanRan/Aegis](https://github.com/GanyuanRan/Aegis) | 1000+ | One-click |
| Multi-agent teams | [NanmiCoder/dsh-agent-teams](https://github.com/NanmiCoder/dsh-agent-teams) | 290+ | Manual (no shipped build) |
| Usage & quotas | [Ychris12138/dsh-usage-stats](https://github.com/Ychris12138/dsh-usage-stats) | 25 | One-click — hand-picked |
| Security audit | [omdsh-dev/dsh-security-audit](https://github.com/omdsh-dev/dsh-security-audit) | 11 | One-click — hand-picked, read-only |
| Theming | [KinGao294/dsh-skin](https://github.com/KinGao294/dsh-skin) | 11 | One-click — hand-picked |
| Turn notifications | [omdsh-dev/dsh-notification](https://github.com/omdsh-dev/dsh-notification) | 44 | One-click — hand-picked |

**7 one-click · 1 script-review · 1 manual — 9 items.** The marketplace shows each item's status explicitly and installs serially, stopping at the first failure. Script-gated items show their script bodies verbatim and require your per-item consent — the pack never consents on your behalf.

**Memory: deliberately empty for now.** The original pick ([adoresever/graph-memory](https://github.com/adoresever/graph-memory), 510+ stars) turned out to have a broken clean-room build (its `tsc` references `openclaw/plugin-sdk`, which the package never declares — reported upstream), so it cannot be installed by any automatic path. Rather than backfill the slot with an unproven alternative, the slot stays empty while the memory-plugin ecosystem settles — 宁缺毋滥. Candidates under observation: omdsh-dev/dsh-mnemon, Aik358/dsh-auto-memory.

### Deliberate exclusions

- **Competing plugin marketplaces** (several exist) — a pack shipped by one marketplace should not install another.
- **Paid relay services** — capability that costs money per call is a choice, not a baseline.
- **Whole runtimes** (`sandbase-harness`, 580+ stars) — an agent runtime is not a plugin baseline.
- **Parody/joke plugins** — fun, but not a foundation.

## For the marketplace scanner

This repository carries the `dsh-plugin` + `dsh-plugin-pack` topics and a [`dsh.pack.json`](dsh.pack.json) manifest. Items are `owner/repo` references resolved to stable repository ids at scan time.

---

# DSH 精选起手包

为 [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) 策展的整合方案，可通过 [DSH 插件市场](https://github.com/w2112515/dsh-plugin-marketplace) 安装。目标：一次审阅，让全新的 DSH 获得**类似 Codex 的完整能力基线**——每个插件覆盖一个能力面，而不是一堆杂烩。

DSH 发布仅数日，因此策展规则是务实的：**优先选择 100 star 以上的插件；某能力面确实没有百星选项时，由维护者按构建质量、许可证与维护活跃度精挑细选；仍然没有可靠候选的槽位宁可空缺也不凑数（宁缺毋滥）**。所有条目均已通过市场目录收录（静态校验通过、未归档、MIT）。

**7 个一键安装 · 1 个需审阅脚本 · 1 个手动安装，共 9 项。** 市场会逐项显式标注状态并串行安装，首个失败即停止；需审阅脚本的条目会逐字展示脚本内容并需你逐项同意——整合包绝不代为同意。

**记忆槽位暂时空缺。** 原选 graph-memory（510+ star）净室构建实测失败（`tsc` 引用了未声明的 `openclaw/plugin-sdk`，已报告上游），任何自动路径都装不上；我们不用未经验证的替代品凑数，持续观察 omdsh-dev/dsh-mnemon、Aik358/dsh-auto-memory 等候选。

明确排除：竞品插件市场（利益冲突）、按调用付费的中继服务（基线不应产生费用）、完整运行时（不是插件基线）、恶搞插件。
