# arrow — live world board

A typed, evidence-bearing relationship graph, rendered to a single self-contained page.

**What you are looking at is the window, not the instrument.** arrow is built to be consumed by
machines: automations query it — pattern matches, typed path derivations, staleness checks — and a
verification layer holds claims over its outputs. The rendering exists so humans can audit what the
machines are reasoning over. In production the same engine maps a platform's dependency topology and
detects structured patterns (for example, laundering rings in transaction graphs), with every finding
carrying a control run that proves the detector needed the whole pattern.

- **[The world board](https://jaredfhelm.github.io/arrow-live/)** — the public stress test: real daily
  world-event data, thousands of edges, each carrying a source, a date, and a basis (official /
  reported / inferred). Click an edge for its evidence; click a node to light its neighborhood; click
  two nodes for their computed composites.
- **[A platform-topology sample](https://jaredfhelm.github.io/arrow-live/platform-sample.html)** — the
  deployment shape: the same instrument pointed at a developer platform's capability map.

Conclusions are computed from a declared composition algebra, never stored, and facts expire honestly
— each type on its own clock. Snapshots rendered by `arrow render`; the engine is a small
deterministic Rust binary. No model inside: same inputs, same map, on any machine.
