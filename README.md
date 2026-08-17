# DSH Category Star Leaders

**A solution pack for [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) (DSH), installable through the [DSH Plugin Marketplace](https://github.com/w2112515/dsh-plugin-marketplace): the highest-starred catalog-admitted entry of each marketplace category.**

**中文文档：[README.zh-CN.md](README.zh-CN.md)**

## Selection rule

Mechanical, no editorial judgment:

1. Take every entry admitted by the marketplace catalog (statically validated, non-archived).
2. Group by marketplace category (theme, memory, ui, tool, provider, usage, skill, security, channel).
3. Take the entry with the most GitHub stars in each category.

Data source: catalog snapshot of **2026-08-17** (3,543 admitted entries). Star counts change over time; the table below restates the snapshot, and each line links to the repository for its current count.

Inclusion states a fact about the catalog ("highest star count in category X at the snapshot date"). **It is not an evaluation, an endorsement, or a recommendation.**

## Contents

| Category | Plugin | Stars (snapshot) | Install (per catalog) |
| --- | --- | --- | --- |
| skill | [liustack/modlens](https://github.com/liustack/modlens) | 2486 | One-click |
| ui | [omdsh-dev/DSH-better-sidebar](https://github.com/omdsh-dev/DSH-better-sidebar) | 1720 | Script review (`prepare`) |
| memory | [sandbaseai/sandbase-harness](https://github.com/sandbaseai/sandbase-harness) | 608 | Manual |
| tool | [superdesigndev/treg](https://github.com/superdesigndev/treg) | 428 | One-click |
| theme | [kingOfSoySauce/dsh-liang-skin](https://github.com/kingOfSoySauce/dsh-liang-skin) | 66 | One-click |
| usage | [Han-1413141/dsh-cost-meter](https://github.com/Han-1413141/dsh-cost-meter) | 57 | One-click |
| channel | [tencent-connect/dsh-qqbot](https://github.com/tencent-connect/dsh-qqbot) | 53 | Manual |
| provider | [Mars-Sea/dsh-commandcode-provider](https://github.com/Mars-Sea/dsh-commandcode-provider) | 44 | Script review (`prepare`) |
| security | [THEWOLFWALKER/dsh-notifier](https://github.com/THEWOLFWALKER/dsh-notifier) | 31 | One-click |

Composition: **5 one-click · 2 script-review · 2 manual — 9 items.** The marketplace shows each item's real install status and proceeds serially, stopping at the first failure. Script-review items display their script bodies verbatim and require your per-item consent; manual items have no automatic install path and the marketplace links their repositories instead. The pack itself never consents on your behalf.

## For the marketplace scanner

This repository carries the `dsh-plugin` + `dsh-plugin-pack` topics and a [`dsh.pack.json`](dsh.pack.json) manifest. Items are `owner/repo` references resolved to stable repository ids at scan time; an item that leaves the catalog shows as unavailable rather than being hidden.
