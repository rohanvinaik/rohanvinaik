Why does proving a theorem in Lean take 671 billion parameters and a datacenter? Why does a green test suite say so little about what a function actually computes? Why does a language model answer in the same confident voice whether it read the paragraph or guessed?

Most of what's here started as one of those questions and then got out of hand.

The bet is the same every time: don't give everything a number — give it a role. A thing, its opposite, or neither: −1, 0, +1. Find the story the data is already telling, and structure ends up doing the work that scale usually gets credit for. The tools that fall out are deterministic — run them twice, get the same answer — and where nothing follows, they say so. A zero is an answer.

## What's on the bench

The domains look scattered on purpose: it's one mechanism, studied wherever it's cheapest to watch.

| | |
|:---|:---|
| **Genomes** · [GenomeVault](https://github.com/rohanvinaik/GenomeVault) | DNA isn't base-4. It's base-2² — the oldest idea on the bench, where the ternary geometry was born — and read that way, privacy stops fighting utility. |
| **Programs** · [Detective](https://github.com/rohanvinaik/Detective) · [Wesker](https://github.com/rohanvinaik/Wesker) · [Uroboros](https://github.com/rohanvinaik/Uroboros) | `assert add(1,1) == 2` also passes for `a*b + 1`. What would it take to *prove* a function can't quietly change? |
| **Theorems** · [Wayfinder](https://github.com/rohanvinaik/Wayfinder) | Proof search as navigation, not prediction — 1,277 of 2,000 Mathlib theorems, one neural pass per proof state, on a laptop. |
| **Models** · [ModelAtlas](https://github.com/rohanvinaik/ModelAtlas) · [MeasuringAGI](https://github.com/rohanvinaik/MeasuringAGI) | Search ~50K models by what you mean, not what you type. Fingerprint how frontier LLMs *think* — benchmarks call them identical; they aren't. |
| **Chess** · [Yami](https://github.com/rohanvinaik/Yami) | Read the game as a story and brilliancy becomes legible: the queen wasn't lost. She was spent. |
| **Triage** · [TriageGeist](https://github.com/rohanvinaik/triagegeist) | 99.86% of emergency-triage decisions with zero LLM in the path — and it knows exactly which 0.14% it shouldn't touch. |
| **Retail** · [Peitho](https://github.com/rohanvinaik/Peitho) | The decision and its explanation are the same object. Nothing to interrogate afterward, because no model decided. |
| **Chaos** · [Ephemeris](https://github.com/rohanvinaik/Ephemeris) · [Ansatz](https://github.com/rohanvinaik/Ansatz) | You can't predict a chaotic orbit. You *can* certify the shape of your own error — which turns out to be worth more. |

<sub>The names are load-bearing. A few of them check out on three layers at once — start with the question of who powers the Detective.</sub>

## Try one

Five minutes, no GPU:

| | | |
|:---|:---|:---|
| [**Detective**](https://github.com/rohanvinaik/Detective) | `pip install detective-spec` | refactor a function — or let a model rewrite it — and prove the behavior didn't change |
| [**Wesker**](https://github.com/rohanvinaik/Wesker) | `pip install wesker` | one mutant per behavioral question your tests leave open, zero dependencies |
| [**ModelAtlas**](https://github.com/rohanvinaik/ModelAtlas) | `gh repo clone rohanvinaik/ModelAtlas` | search ~50K models by what you mean; an ambiguous ask gets you one clarifying question back instead of a guess — privately known as Jeeves mode |

Every repo has a section that says where it stops. Those were the hardest parts to write, which makes them the best place to start reading.

<details>
<summary><b>The record (2025 – early 2026)</b></summary>
<br/>

**Behavioral model identity** — what a model *is* when you can't see the weights. [PoT_Experiments](https://github.com/rohanvinaik/PoT_Experiments) · [REV](https://github.com/rohanvinaik/REV) · [HBT_Validator](https://github.com/rohanvinaik/HBT_Validator) — archived as a completed record; the line continues in [MeasuringAGI](https://github.com/rohanvinaik/MeasuringAGI).

**Semantic foundations** — the primitives the later systems stand on. [semantic_probing](https://github.com/rohanvinaik/semantic_probing) · [sparse-wiki-grounding](https://github.com/rohanvinaik/sparse-wiki-grounding) · [negative-learning](https://github.com/rohanvinaik/negative-learning) · [orthogonal-validators](https://github.com/rohanvinaik/orthogonal-validators) · [experience-memory](https://github.com/rohanvinaik/experience-memory) · [semantic_knowledge_graph](https://github.com/rohanvinaik/semantic_knowledge_graph)

**Applied** — [ShortcutForge](https://github.com/rohanvinaik/ShortcutForge): a natural-language compiler for Apple Shortcuts. The LLM is the front-end; the compiler is the reliability.

</details>

---

A lot of this follows a road someone else cut. Patrick Winston spent his last decade insisting that we are storytelling animals — that intelligence was never the pile of data, it's the story built over it, and different viewers holding different pieces can still arrive at the same understanding. The field mostly moved on. He documented his tools anyway — help boxes wired, examples loaded — for a collaborator who hadn't arrived yet. This workshop came in through the door he left open. Kanerva, Wierzbicka, Minsky, and Ashby left doors too; half the names in the repo list are thank-you notes.

<sub>Independent researcher · Cambridge, MA · biochemist by training · [RohanV.me](https://www.RohanV.Me) · rohanpvinaik@gmail.com</sub>
