# 3 Visual Directions for AgentDiligence

## Direction 1: "The Evidence Trail"
Visualize evaluation as a verifiable path — each claim links to proof. Conveys rigor and traceability without folders/stamps.

**Motif:** Horizontal flow of nodes connected by lines. Some nodes "verified" (filled, checkmark), branching to expandable evidence cards on hover.

```html
<svg viewBox="0 0 600 120" class="evidence-trail">
  <line x1="40" y1="60" x2="560" y2="60" stroke="#1f2937" stroke-width="2" stroke-dasharray="2 6"/>
  <circle cx="100" cy="60" r="10" fill="#0ea5e9"/>
  <circle cx="250" cy="60" r="10" fill="#0ea5e9"/>
  <circle cx="400" cy="60" r="10" fill="#10b981"/>
  <circle cx="550" cy="60" r="10" fill="#10b981"/>
  <!-- branch to evidence -->
  <path d="M400 60 L400 30 L470 30" fill="none" stroke="#10b981" stroke-width="1.5"/>
  <rect x="470" y="18" width="60" height="24" rx="4" fill="#ecfdf5" stroke="#10b981"/>
</svg>
```
**Palette:** ink (#111827) + signal blue (#0ea5e9) + verify green (#10b981). **Why it works:** reads as "audit trail" / "claim → proof," technical and trustworthy.

---

## Direction 2: "Scorecard Telemetry"
Treat the agent eval like instrumentation — live, measured, dashboard-native. Feels like product, not paperwork.

**Motif:** Compact radial/bar score gauges with animated fill-on-load. Sparse grid, monospace numerals, tight micro-labels.

```html
<div class="gauge">
  <svg viewBox="0 0 80 80">
    <circle cx="40" cy="40" r="34" fill="none" stroke="#1f2937" stroke-width="6"/>
    <circle cx="40" cy="40" r="34" fill="none" stroke="#0ea5e9" stroke-width="6"
      stroke-dasharray="213" stroke-dashoffset="64" stroke-linecap="round"
      transform="rotate(-90 40 40)"/>
  </svg>
  <span class="score">87</span>
</div>
```
```css
.score { font-family: 'JetBrains Mono', monospace; font-weight: 600; }
.gauge circle:last-child { transition: stroke-dashoffset 1.2s cubic-bezier(.4,0,.2,1); }
```
**Palette:** near-black canvas + electric blue accent + one warning amber (#f59e0b). **Why it works:** measurable, dashboard-credible, YC-modern.

---

## Direction 3: "Pre-Deployment Gate"
A literal go/no-go checkpoint metaphor — emphasizes *buyer-side, before procurement*. Decisive and confident.

**Motif:** A vertical pass-line with candidate agents flowing left, gate marker in center, evaluated agents emerging right with status tags. Use a subtle "wireframe agent" as a labeled abstract token (no robot faces).

```html
<svg viewBox="0 0 600 160">
  <!-- gate line -->
  <line x1="300" y1="20" x2="300" y2="140" stroke="#0ea5e9" stroke-width="2"/>
  <!-- abstract agent tokens (hexagons, not robots) -->
  <polygon points="120,80 140,68 160,80 160,104 140,116 120,104"
    fill="none" stroke="#6b7280" stroke-width="1.5"/>
  <polygon points="440,80 460,68 480,80 480,104 460,116 440,104"
    fill="#ecfdf5" stroke="#10b981" stroke-width="1.5"/>
  <text x="445" y="135" font-family="monospace" font-size="10" fill="#10b981">PASS</text>
</svg>
```
**Palette:** cool gray inputs → green/red verdicts. **Why it works:** crystallizes the core value prop (evaluate *before* you deploy) in one glance.

---

### Cross-cutting system
- **Type:** Geometric sans (Inter/Geist) + monospace for scores/IDs.
- **Texture:** flat + thin strokes (1–2px), generous whitespace, single accent.
- **Motion:** subtle on-load fills/draws (`stroke-dashoffset`), never decorative.
- **Avoid:** gradients-as-glow, 3D, drop shadows on everything.

**My pick:** Lead hero with **Direction 1 (Evidence Trail)** — most differentiated and on-message ("evidence-backed") — and use **Direction 2 gauges** as the method/proof section.