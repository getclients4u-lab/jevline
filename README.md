# Jevline™ — The Typed Decision Playbook™

Give your software a **typed judgment** it can be trusted with.

**LIVE:** https://jevline.vercel.app/

---

## The Niche (why now)

**The TypeSafe "Jev" wave — the loudest developer story of mid-September 2026.**

TypeSafe AI's *System One* decision model, **Jev**, went from a launch post to a sprawling open-source
ecosystem in roughly one week. Live signals from GitHub (2026-09-25, this run — `web_search` disabled,
so trend research used the GitHub Search API + Hacker News Algolia + the ecosystem's own catalogs):

| Repo | Stars | Created | What |
|---|---|---|---|
| `NandhaKishorM/laya` | **23,796★** | 09-18 | Non-autoregressive System 1 decision engine, 100+ languages |
| `browser-use/jev-ultrafast` | **19,996★** | 09-16 | "Fastest and cheapest web agent" |
| `jaredpalmer/kev` | 6,848★ | 09-17 | Jev-like models you can train/run locally |
| `tamaratran/fast-jev-compaction` | 6,772★ | 09-17 | Claude Code plugin using Jev decisions |
| `TheoLeeCJ/SemIf-OpenJev` | 4,270★ | 09-16 | Semantic ifs from open models |
| `jarrodwatts/jev-trader` | 2,387★ | 09-16 | One AI trade decision per block |
| `TianyuCodings/NanoJev` | 2,222★ | 09-17 | End-to-end training pipeline replica |
| `yibie/awesome-jev` / `heyjunpenn/awesome-jev` | 1,644★ / 818★ | 09-17/19 | Catalogs — one claims **916 projects** |
| `wfzyx/von` | 656★ | 09-18 | Open-source System One, "sub-15ms" drop-in |
| `nokia-applied-research/AnyJev` | 547★ | 09-21 | Turn any LLM into a Jev-style decision model |

**30+ new repos, most created 16–22 September 2026.** The IDE / agent ecosystem rushed to integrate it:
Cloudflare Workers AI, Netlify AI Gateway, Vercel AI Gateway, and OpenRouter all list `typesafe/jev`.

**The gap:** the ecosystem supplies *hype and catalogs*, not *production discipline*. The community's own
curated lists open with a warning: *"Curation is not endorsement … several repositories published together
by one author, sharing a scaffold and a thin commit history, can satisfy every inclusion rule and still be
unproven."* Meanwhile the most-copied line in the whole ecosystem is a threshold (`p >= 0.9`) that is a
**teaching example, not a measured operating point** — copied into countless codebases with no calibration.

**The core insight:** a decision is not a prompt — it's a **contract**. Unstructured state in, a *typed*
answer out (choice / score / probability), with confidence attached. The hard part was never the model;
it's the discipline around it: ask one narrow question, shape the answer your code can consume, calibrate
the threshold on your own labelled cases, and gate the action with a review path.

> *Note: `web_search` was disabled this run; no YouTube/Zernio trending API was available. Trend research
> used the GitHub Search API (`created:>…`, sorted by stars), Hacker News Algolia (front page + top
> stories), and the ecosystem's own curated catalogs — the strongest signals available.*

---

## The Business

- **Brand:** Jevline™ (badge: ⚡ / line-art bolt + cyan)
- **Product:** **The Typed Decision Playbook™** — 8-part digital PDF system
- **Mechanism:** **The JEVLINE Loop™** — **ASK → SHAPE → CALIBRATE → GATE**
- **Promise:** turn "we tried Jev" into a decision layer you can test, price, and defend
- **Price:** $19 founder (anchor $196)
- **Audience:** agent builders, platform engineers, founders shipping typed decisions
- **Positioning:** the *operating discipline* for typed decisions — model-agnostic, vendor-neutral

### The 8 deliverables

1. The Typed Decision Playbook™ (core guide: the loop + the three ingredients of a confident mistake)
2. The Question Shaper™ + Primitive Selector (Noul / Choice / Score decision table, question cards)
3. The Threshold Calibration Kit™ (freeze, sweep, plot, quote the holdout; policy-file template)
4. Abstention & Escalation Design™ (ALLOW / REVIEW / REFUSE, no-match options, evidence gates)
5. The Cascade & Cost Blueprint™ (four cascade tests, cost model, escalated-but-unchanged meter)
6. The Decision Ledger™ + Drift Watch (seven minimum fields, weekly review, three drift signals)
7. The Failure-Mode Playbook™ (seven failure modes, exact fixes, proving tests)
8. The 30-Day Rollout Playbook™ (one step → an owned decision layer, with gates)

---

## Repos & Deploy

- **Public repo:** `getclients4u-lab/jevline` (branch as deployed)
- **Private data repo:** `getclients4u-lab/jevline-data` (users.json, buyers.json, 8 product PDFs)
- **Vercel:** see `DEPLOY-INFO.md`
- **Access code prefix:** `JL-XXXXX-XXXXX`
- **Files:** `index.html` (landing) · `download.html` (member area) · `admin.html` (ops) · `thank-you.html`
  · `api/*.js` (verify, admin, download, webhook) · `emails/` · `vsl/` · `product/` (markdown) · `pdf/`

## Build notes

- Product PDFs generated from `product/*.md` via `pandoc → html → wkhtmltopdf` (never `.md` straight to wkhtmltopdf).
- Backend adapted from the proven gutmap stack; all brand refs replaced and verified with `grep`.
- `node --check` run on every `api/*.js` and every inline `<script>` extracted from each `.html`.
