# AgentDiligence Hero Visual Concepts

The core insight from your feedback: the visual must show **comparison** as the hero action, not measurement. Buyers think in terms of "which one wins," not "how we instrument the test." Below are 3 concepts that lead with side-by-side evaluation.

---

## Concept 1: The Scorecard Lineup

**Mental model:** A bake-off. Multiple agents run the same task; one column wins.

**Copy labels:**
- Headline: **"Test every agent on your real work. Pick the one that's ready."**
- Subhead: "Run the same buyer scenarios across vendors before you sign."
- Column headers: `Vendor A` · `Vendor B` · `Your Custom Agent`
- Row labels: `Accuracy` · `Safety` · `Cost` · `Speed`
- Verdict chip: ✅ **Ready to deploy**

**Why it works:** Buyers instantly recognize a comparison table with a winner highlighted. Zero jargon.

```html
<div class="scorecard">
  <div class="task-bar">Same scenario → "Process a refund dispute"</div>
  <div class="grid">
    <div class="col header">Metric</div>
    <div class="col header">Vendor A</div>
    <div class="col header winner">Vendor B</div>
    <div class="col header">Custom</div>

    <div class="col label">Accuracy</div>
    <div class="col">82%</div>
    <div class="col winner">96%</div>
    <div class="col">71%</div>

    <div class="col label">Safety</div>
    <div class="col">⚠︎</div>
    <div class="col winner">✅</div>
    <div class="col">⚠︎</div>

    <div class="col label">Cost / task</div>
    <div class="col">$0.40</div>
    <div class="col winner">$0.22</div>
    <div class="col">$0.18</div>
  </div>
  <div class="verdict">✅ Vendor B — Ready to deploy</div>
</div>

<style>
.scorecard {
  font-family: 'Inter', system-ui, sans-serif;
  max-width: 560px;
  background: #fff;
  border-radius: 16px;
  box-shadow: 0 12px 40px rgba(0,0,0,.08);
  padding: 24px;
}
.task-bar {
  font-size: 13px; color: #6b7280;
  background: #f3f4f6; padding: 10px 14px;
  border-radius: 8px; margin-bottom: 18px;
}
.grid {
  display: grid;
  grid-template-columns: 1.2fr 1fr 1fr 1fr;
  gap: 1px; background: #eef0f3;
  border-radius: 10px; overflow: hidden;
}
.col { background:#fff; padding: 14px 12px; font-size: 14px; text-align:center; }
.col.label { text-align:left; color:#6b7280; font-weight:500; }
.col.header { font-weight:600; color:#111827; background:#fafbfc; }
.col.winner { background:#ecfdf5; color:#065f46; font-weight:600; }
.verdict {
  margin-top: 18px; text-align:center;
  font-weight:700; color:#065f46;
  background:#ecfdf5; padding:12px; border-radius:10px;
  animation: pulse 2.4s ease-in-out infinite;
}
@keyframes pulse { 0%,100%{opacity:1} 50%{opacity:.7} }
</style>
```

---

## Concept 2: Same Task, Split Lanes

**Mental model:** A race. One task fans out to multiple agents in parallel lanes; a checkmark lands on the winner.

**Copy labels:**
- Headline: **"One task. Every agent. One clear answer."**
- Subhead: "We run your scenarios across agents side-by-side and tell you which is safe to ship."
- Center node: `Your Work Scenario`
- Lane endpoints: `Agent 1` `Agent 2` `Agent 3` with pass/fail badges

**Why it works:** The branching motif visually screams "multi-agent comparison" before anyone reads a word.

```html
<svg viewBox="0 0 560 280" width="560" font-family="Inter, sans-serif">
  <!-- Source task -->
  <rect x="20" y="120" width="130" height="44" rx="10" fill="#111827"/>
  <text x="85" y="147" fill="#fff" font-size="13" text-anchor="middle">Your Scenario</text>

  <!-- Branch lines -->
  <path d="M150 142 C 230 142, 230 50, 320 50" stroke="#d1d5db" stroke-width="2.5" fill