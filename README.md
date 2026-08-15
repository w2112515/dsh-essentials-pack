# DSH Essentials

**A curated solution pack for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) (DSH): one reviewed action gives a fresh DSH a complete, Codex-grade capability baseline — sidebar workspace UI, @path references, vision, architecture-aware coding, multi-agent teams, usage dashboards, a security audit, theming, and turn notifications.**

**中文文档：[README.zh-CN.md](README.zh-CN.md)**

Installable through the [DSH Plugin Marketplace](https://github.com/w2112515/dsh-plugin-marketplace). Not a pile of plugins: each item covers exactly one capability area, and every item is admitted by the marketplace catalog (statically validated, non-archived, MIT).

## Curation rule

DSH is days old, so the rule is pragmatic: **100+ stars preferred; where no 100-star option exists in a capability area, the pick is hand-selected** for build quality, license, and maintenance activity; **where no reliable candidate exists at all, the slot stays empty** — 宁缺毋滥 (quality over quantity), never padding.

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

**Memory: deliberately empty for now.** The original pick ([adoresever/graph-memory](https://github.com/adoresever/graph-memory), 510+ stars) turned out to have a broken clean-room build (its `tsc` references `openclaw/plugin-sdk`, which the package never declares), so no automatic install path can succeed. Rather than backfill the slot with an unproven alternative, it stays open while the memory-plugin ecosystem settles. Candidates under observation: omdsh-dev/dsh-mnemon, Aik358/dsh-auto-memory.

### Deliberate exclusions

- **Competing plugin marketplaces** (several exist) — a pack shipped by one marketplace should not install another.
- **Paid relay services** — capability that costs money per call is a choice, not a baseline.
- **Whole runtimes** (`sandbase-harness`, 580+ stars) — an agent runtime is not a plugin baseline.
- **Parody/joke plugins** — fun, but not a foundation.

## For the marketplace scanner

This repository carries the `dsh-plugin` + `dsh-plugin-pack` topics and a [`dsh.pack.json`](dsh.pack.json) manifest. Items are `owner/repo` references resolved to stable repository ids at scan time.
