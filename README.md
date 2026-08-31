# Rohan Vinaik

If you've ever wondered why proving a theorem in Lean requires 671B parameters and a datacenter — or asked how many tests it actually takes to pin down what a program does — you're in the right place.

I build deterministic systems that show their work: a verifier that proves a refactor changed nothing, a prover that navigates instead of predicts, and measurement instruments that abstain instead of guess. Everything runs on consumer hardware, the load-bearing claims are machine-checked in Lean 4, and every repo has a section that says where it stops. That last part is on purpose.

`deterministic · warrant-carrying · Lean-checked where it counts · laptop-scale`

---

## Use one today

| | | |
|:---|:---|:---|
| [**Detective**](https://github.com/rohanvinaik/Detective) | `uv add detective-spec` | Refactor a Python function — or let a model rewrite it — and prove the behavior didn't change. |
| [**Wesker**](https://github.com/rohanvinaik/Wesker) | `pip install wesker` | Mutation testing that counts the behavioral questions your tests leave open — one mutant per question, zero dependencies. |
| [**Prism**](https://github.com/rohanvinaik/Prism) | `uv tool install prism-mcp` | Every Claude Code session writes down exactly what it did. Prism is the part that reads it back. |

---

## The claim, in one function

`assert add(1, 1) == 2` passes — and so does `3*a - b`, and so does `a*b + 1`, and so do infinitely many functions that are not addition. A green suite proves your code was right once, not that it's pinned. Closing that gap turns out to be a computable problem, and the number of tests it takes — the specification complexity σ — is the same quantity five fields discovered independently: teaching dimension, exact-learning query complexity, identity testing, local testability, certificate size. That identification, and the dynamics that follow from it, are formalized in Lean 4. Everything below hangs on that thread.

## The map

**Specification — green is not proof.**

| | |
|:---|:---|
| [Wesker](https://github.com/rohanvinaik/Wesker) | In-process AST mutation testing; the greedy (1−1/e) selection bound machine-checked in Lean against Mathlib. |
| [Detective](https://github.com/rohanvinaik/Detective) | Mutation-complete suites as behavioral contracts. Applies nothing it cannot prove. |
| [Uroboros](https://github.com/rohanvinaik/Uroboros) | The same loop run unattended across a whole repository — CPU-only, the model never drives. |
| [LintGate](https://github.com/rohanvinaik/LintGate) | The research workbench where σ was born: specification measurement, decomposition prescriptions, the theory. |

**Navigation — structure does the work that scale gets credit for.**

| | |
|:---|:---|
| [ModelAtlas](https://github.com/rohanvinaik/ModelAtlas) | ~50K HuggingFace models as coordinates in a signed 8-bank space. Search by meaning — under 100 ms, no embeddings, no GPU. |
| [Wayfinder](https://github.com/rohanvinaik/Wayfinder) | Lean 4 proof search as navigation: 1,277 of a frozen 2,000-theorem Mathlib split, raw, one neural pass per proof state. |
| [GenomeVault](https://github.com/rohanvinaik/GenomeVault) | A genome read as Z₂ × Z₂ — balanced ternary — so privacy, security, and utility stop trading against each other. |

**Instruments — measurement that shows its work.**

| | |
|:---|:---|
| [MeasuringAGI](https://github.com/rohanvinaik/MeasuringAGI) | A 12-dimensional metacognitive fingerprint that resolves models accuracy benchmarks call identical. 33 frontier LLMs mapped. |
| [TriageGeist](https://github.com/rohanvinaik/triagegeist) | Auditable emergency triage: 99.86% of decisions with zero LLM in the path; the rest typed and certified. |
| [Peitho](https://github.com/rohanvinaik/Peitho) | A retail decision engine in pure Python — zero runtime dependencies, a reason on every line, every decision mutation-pinned. |
| [Yami](https://github.com/rohanvinaik/Yami) | A chess game read as a story — recognition instead of tree search, every rule one a human could state. |
| [Ephemeris](https://github.com/rohanvinaik/Ephemeris) · [Ansatz](https://github.com/rohanvinaik/Ansatz) | Certified surrogates for chaotic systems: the output carries a certificate on the shape of its own error — and a method for minting more. |

---

<details>
<summary><b>Foundations & record (2025 – early 2026)</b></summary>
<br/>

**Behavioral model identity** — the question that started all of this: what a model *is* when you can't see the weights.

| | |
|:---|:---|
| [PoT_Experiments](https://github.com/rohanvinaik/PoT_Experiments) | Cryptographically pre-committed behavioral challenges; model identity on a consumer Mac. |
| [REV](https://github.com/rohanvinaik/REV) | Restriction sites: layer boundaries where behavioral variance spikes, verified in a fraction of the memory. |
| [HBT_Validator](https://github.com/rohanvinaik/HBT_Validator) | Hyperdimensional fingerprints that capture architectural lineage without weight access. |

Archived as a completed record — this line continues in [MeasuringAGI](https://github.com/rohanvinaik/MeasuringAGI).

**Semantic foundations** — the primitives the later systems stand on.

| | |
|:---|:---|
| [semantic_probing](https://github.com/rohanvinaik/semantic_probing) | 62 universal semantic primitives with Hadamard-exact orthogonality; antonyms at −1.0 by construction. |
| [sparse-wiki-grounding](https://github.com/rohanvinaik/sparse-wiki-grounding) | Typed knowledge links with explicit reasoning chains — *why* a claim is wrong, not just that it is. |
| [negative-learning](https://github.com/rohanvinaik/negative-learning) | Minsky's censors: constraints learned from failures, 22× more sample-efficient than positive examples. |
| [orthogonal-validators](https://github.com/rohanvinaik/orthogonal-validators) | Structurally independent validators — when all report low confidence, that's signal, not noise. |
| [experience-memory](https://github.com/rohanvinaik/experience-memory) | O(1) fix lookup for recurring errors; no gradient descent. |
| [semantic_knowledge_graph](https://github.com/rohanvinaik/semantic_knowledge_graph) | Knowledge graphs where position encodes meaning. |

**Applied** — [ShortcutForge](https://github.com/rohanvinaik/ShortcutForge): a natural-language compiler for Apple Shortcuts. The LLM is the front-end; the compiler is the reliability.

</details>

<details>
<summary><b>Foundations (the people)</b></summary>
<br/>

Kanerva (hyperdimensional computing) · Wierzbicka (semantic primitives) · Minsky (censors, suppressors, K-lines) · Collins & Loftus (spreading activation) · Winston (near-miss learning, story understanding)

</details>

---

<sub>Independent researcher · Cambridge, MA · biochemist by training · [RohanV.me](https://www.RohanV.Me) · [rohanpvinaik@gmail.com](mailto:rohanpvinaik@gmail.com)</sub>
