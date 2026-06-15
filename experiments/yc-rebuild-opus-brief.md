# YC-style AgentDiligence rebuild brief — Opus 4.8

# AgentDiligence Landing Page Blueprint

## 1. Headline / Subhead / CTA

**Headline:** Test every agent before you trust one.

**Subhead:** Run your real workflow across vendor agents, your own build, and a baseline — side by side. See the evidence, get a recommendation, then buy.

**Primary CTA:** Run your first comparison
**Secondary CTA:** See a sample report →

---

## 2. Above-Fold Visual Concept

A clean **three-column comparison board** — the literal product, not a metaphor. Think a results scoreboard for agents running the same task.

**Top bar (shared task):**
`TASK: Resolve refund dispute · 50 cases · Your support workflow`

**Three side-by-side cards, equal width:**

| Card A | Card B | Card C |
|---|---|---|
| **Vendor: Acme Agent** | **Your Build (v3)** | **Baseline: GPT-4o + tools** |
| ✅ Resolved 47/50 | ✅ Resolved 49/50 | ✅ Resolved 41/50 |
| ⏱ 12.4s avg | ⏱ 8.1s avg | ⏱ 15.2s avg |
| 💲 $0.018/task | 💲 $0.031/task | 💲 $0.009/task |
| ⚠ 2 policy violations | ⚠ 0 policy violations | ⚠ 6 policy violations |
| [View transcript] | [View transcript] | [View transcript] |

**Center card (B) is visually elevated** — subtle lift, accent border — as the recommended pick.

**Recommendation strip below the cards:**
`✓ Recommendation: Your Build (v3) — highest accuracy, zero policy violations, acceptable cost. Full reasoning →`

This single image telegraphs: same workflow → multiple candidates → comparable evidence → decision.

---

## 3. Visual Design Tokens

**Palette:**
- Background: near-black `#0B0D10` with a very subtle warm-charcoal gradient
- Surface cards: `#15181D` with `#222831` 1px borders
- Primary text: `#F2F4F7`
- Muted text: `#8B95A5`
- Accent (single, confident): electric lime-green `#C6F24E` or signal cyan `#5BE9C9` — pick one, use sparingly for CTA + recommended state
- Status colors: green `#4ADE80`, amber `#FBBF24`, red `#F87171` (used only inside data cells)

**Typography:**
- Headlines: tight, geometric sans — Inter Tight, General Sans, or Söhne; large, -2% letter-spacing, weight 600–700
- Body: Inter / Geist, 16–18px, generous line-height
- Data/labels in cards: monospace (Berkeley Mono, JetBrains Mono) — signals "real test output"

**Layout:**
- Max content width 1200px, generous vertical rhythm (96–128px section padding)
- Sharp corners or max 8px radius — avoid soft/pillowy
- One accent color only; let dark + mono carry the "edgy infra" feel
- Subtle grid/border lines, no glows or blur blobs

---

## 4. Section Sequence

1. **Hero** — headline + the comparison board visual
2. **Problem** — "You can't trust a demo." three short pain points
3. **How it works** — 3 steps: Define workflow → Run candidates → Get recommendation
4. **Product close-up** — zoom into one capability (transcript diff / evidence drill-down)
5. **What you compare** — accuracy, cost, latency, policy adherence, failure modes (chip row)
6. **Who it's for** — buyers, platform teams, agent builders evaluating vendors
7. **Sample report** — link/preview to a full diligence output
8. **Trust band** — quiet logos / "Built for enterprise procurement"
9. **Final CTA** — repeat primary action
10. **Minimal footer**

---

## 5. Copy Snippets

**Problem section:**
> **Demos lie. Procurement guesses.**
> Vendor pitches show happy paths. You deploy and discover the edge cases in production — with real customers and real liability.

**How it works (3 steps):**
1. **Define the job.** Bring your actual workflow and a set of real cases.
2. **Run the field.** Vendor agents, your in-house build, and a baseline — same task, same data.
3. **Get a verdict.** Side-by-side evidence and a clear recommendation you can defend.

**What you compare (chips):**
`Task success` · `Cost per task` · `Latency` · `Policy adherence` · `Failure modes` · `Edge-case handling`

**Product close-up:**
> **Every claim is clickable.** Drill into any transcript. See exactly where an agent succeeded, stalled, or broke policy — not a score, the actual run.

**Final CTA:**
> **Stop buying on vibes.** Run the diligence before the deployment.

---

## 6. Emphasize / Avoid

**Emphasize:**
- The **same workflow, multiple candidates** mental model — repeat it visually and in copy
- **Evidence you can click into** (transcripts, real runs) — credibility through concreteness
- A **decision/recommendation** as the payoff — buyers want an answer, not a dashboard
- Buyer-side framing: procurement confidence, defensible choice, pre-deployment

**Avoid:**
- Robots, neural blobs, shields, badges
- Folders, stamps, paperclips, any audit/compliance/gov visual language
- Telemetry/observability jargon ("traces," "spans," "instrumentation") in headlines
- Multiple accent colors or glowing gradients — keep it one sharp accent on dark
- Abstract data-viz that doesn't map to a real decision

The whole page should read like *a scoreboard for agents you're about to buy* — concrete, comparative, decisive.