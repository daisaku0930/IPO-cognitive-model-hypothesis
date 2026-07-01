---
section: Source Text (Structural Register)
role: A single-file pass that runs the whole structure as bare bones, with metaphors and test cases stripped away. Also serves as a record of the starting point.
note: Confidence tags [Established] / [Hypothesis] / [Speculation] should be respected. Do not treat [Speculation] as assertion.
---

# IPO Cognitive Model — Source Text

An observational model that re-frames all human cognition and activity as **Input → Process → Output**, and treats individual differences as coordinates. This file is a record that runs the structure on a single thread, with metaphor and simplification removed.

> Positioning: This is not a "theory" but an observational framework. On top of the structure (axes), a falsifiable theory (links and laws between axes) rests thinly. It is formalized (has notation) but not operationalized (has no measurement methods).

---

## 0. The Formula (Model Signature and State Definition)

```
IPO × C

C = (W, n, m | α, Θ, Δ)
```

- Line 1 **`IPO × C`** … The model's signature. The product of **flow (IPO) × state (C)**. IPO is "from where / in which direction do we read" (the origin axis); C is "the current cognitive configuration" (the state axis). The two are at different layers, so they are separated by line.
- Line 2 **`C = (W, n, m | α, Θ, Δ)`** … Definition of state C. Left of the bar (W, n, m) = state variables; right (α, Θ, Δ) = correction parameters (all in the P layer).
- **Temporality**: C is not a fixed value but a state updated through the IPO cycle (C_t → C_t+1). Updating is covered in §6.
- **Auxiliary notation**: O_ext = the result put out externally (seen by others) / O_int = the result that remains internally (mixed into the next cycle's C). Not a component of C, but notation distinguishing the two directions of the Output interface.

---

## 1. Skeleton — IPO and Three Orientations

All cognition is seen as a flow of `Input → Process → Output`. Even looking at the same flow, where one places value or interest differs.

| Orientation | Interest | Main questions |
| --- | --- | --- |
| I (Input) | Information, materials, premises, evidence | Is the information complete? / Is there a basis? / Any other cases? |
| P (Process) | Judgment, structure, causality, mechanism | Why is it so? / How to judge? / Can it be applied? |
| O (Output) | Result, outcome, the right answer | How did it turn out? / What's the answer? / How far to go? |

This is not a fixed "typing." It is merely a typical example of the bias in W (direction of attention allocation), and **W is not an attribute fixed to a person but swings by situation**. The same person may lean I in an audit and O in planning. "I-type / P-type / O-type" is shorthand for "the state of leaning toward that orientation in that situation." [Hypothesis]

> The "→" itself is also Process. Inside the P of `I → P → O` lies a multi-stage structure `I → P1 → P2 → … → O`. The depth of this division is the later m (§4).

---

## 2. W — Direction of Attention Allocation

A weight vector representing "where attention is directed."

```
W = (w_I, w_P, w_O)   (Σw = 1)
```

W represents direction only. Independent of it are the axes of "how finely to handle" (resolution n, §3) and "how deeply to dig" (depth m, §4). [Hypothesis]

Some mismatches can be explained not by ability differences but by differences in W. For example, "tell me the answer" (O-leaning) and "you should figure it out by thinking" (P-leaning) are both correct; they simply look at different places. [Hypothesis]

---

## 3. n — Resolution (Width of Interface and Parallelism)

n is not a scalar but a 3-component vector corresponding to I, P, O.

```
n = (n_i, n_p, n_o)
```

- **n_i**: input resolution (how finely one receives from the world / granularity of observation and listening)
- **n_p**: parallelism of P (number of processing threads held simultaneously / working-memory-like width)
- **n_o**: output resolution (how finely one outputs to the world / granularity of expression)

**The interface is single-threaded**: the `I → P → O` pipeline itself cannot run in parallel (the reason "humans don't multitask"). Only the inside of P can be parallelized, and its width is n_p. The working memory capacity limit (the famous 7±2) can be interpreted as a manifestation of the upper bound of n_p. [Established: n_p ↔ WM capacity]

**n_i and n_o can differ independently** (a correction of the old model's implicit assumption that n_i = n_p = n_o). [Hypothesis: testable as double dissociation]

- High n_i, low n_o: receives finely, outputs coarsely (observer, researcher)
- Low n_i, high n_o: receives coarsely, outputs finely (performer, craftsman)
- High n_i, high n_o: both fine (translator, interpreter)

**Conversational mismatch**: "you should get it with a little thought" fails to land because the processing divisions obvious to oneself (high n_p) simply do not exist in the cognitive structure of the other (low n_p). It is a structural problem, not an ability problem. Which of n_i / n_p / n_o the difference comes from changes the kind of mismatch. [Hypothesis]

> Function-composition formulation (supplementary): the flow can be written `O = (f_n ∘ … ∘ f_1)(I)` (each f_k being a transformation such as interpretation, classification, judgment, action selection). This is a notational convenience, not a measured quantity.

---

## 4. m — Depth of Processing

The number of stages at which intermediate products generated inside P are re-fed as input for further processing. If n is "horizontal width," m is "vertical depth."

```
m small (shallow): I → P → O
m large (deep):    I → P → Pk → P' → … → O   ← intermediate result recurses as input
```

- **Pk and I' are phase names**: the same entity can be called both "an intermediate product inside P (Pk)" and "material re-fed as input (I')." Not a change of object, but a change in the phase within the flow. This "critical point where an intermediate product turns into input" is treated by the model as a **phase transition (the criticality of processing = a digital cut)** (see §8 for how it sits alongside other cuts).
- **Chaining is the external unfolding of depth**: the "chain" of re-feeding O as a new I is depth m unable to fit in one unit, unfolded via the O interface. Completed internally, it is deep processing; routed through the external (O_ext), it looks like a chain. The same deepening, differing only in whether it crosses an interface.
- **n_p constrains the upper bound of m**: if few intermediate products can be held in parallel, deep re-feeding is hard to trigger. [Hypothesis]
- **Conditions under which deep processing does not occur**: n_p is forcibly made small (manualization / routinization that disallows parallel holding) / stopping just before O (O-type tendency) / lack of time and resources. When m is fixed shallow, deepening does not occur. This is a structural explanation of "why learning and creation rarely occur in routine work." [Hypothesis]

**Expanded range**: adding m extends the model beyond describing cognitive types to explaining the conditions under which learning (intermediate products generate new questions), problem-solving (partial solutions open deeper problems), and creation (fragments trigger other fragments) occur.

> Redefinition under consideration: could m be re-read not as "depth inside Process" but as the **number of round trips across the three interfaces I/P, P/O, P/P'**? Then n (width of interface) and m (round trips of interface) sit on the same footing, and since P is involved in every round trip, the reason m belongs exclusively to P can also be derived. However, only I/P and P/O round trips are observable; P/P' (silent thought, introspection) is invisible from outside, so unification comes at the cost of a narrower observation window. [Open question]

---

## 5. Correction — α・Θ・Δ (The Layer of Transmission and Self-Correction)

Cognition automatically fills unstated gaps (correction). Correction occurs entirely in the P layer; interfaces (I, O) are structural constraints and outside the scope of correction. It acts on depth m.

Even with the same input, the landing splits into three stages.

| Stage | State |
| --- | --- |
| ① Comfortable | fills automatically (unconscious) |
| ② Increased cost | fills but requires conscious effort |
| ③ Breakdown | cannot fill (misreading, freeze, avoidance) |

The three parameters that determine this form a hierarchy **α → Θ → Δ**.

- **α (firing probability)**: whether correction is executed at all. When low, one skips reading before filling = careless mistake (a problem of firing, not ability).
- **Θ (threshold)**: the range that can be filled automatically. The boundary of ①↔②.
- **Δ (capacity)**: the upper limit of filling power. The boundary of ②↔③.

A fully structured document (conclusion, basis, result only) feels "easy to read yet hard to read" to a high-resolution person because it is not exceeding Δ (incomprehensible) but exceeding Θ (comprehensible but with correction cost) = stage ②. [Hypothesis]

> Caveat (this layer is the most speculative): α・Θ・Δ have no measurement methods, and any failure can be explained after the fact as "α dropped" or "Δ exceeded." It is meaningful only when the three stages can be separated as distinct observable signs (immediate-unconscious / delayed-conscious-fatiguing / error-avoidance). Narrowed that far, [Hypothesis]; before narrowing, [Speculation].

### Summary of Variable Structure

Since the skeleton has the three elements I, P, O, each variable can have components along the three axes.

- **W, n**: 3-component **vectors** corresponding to I/P/O (direction / width).
- **m, α, Θ, Δ**: **scalars** concentrated in P (depth, and the correction acting on that depth).

---

## 6. Update — Self-Update of C

C is not a fixed cognitive trait but is continuously updated through the experience of the IPO cycle (C_t → C_t+1). [Speculation]

One cycle produces not only the externally emitted result (O_ext) but also the internally remaining result (O_int). O_int mixing into the next cycle's C is what changes C.

**The direction of update is determined not by experience itself (O_ext) but by the interpretation (P) inserted in between**. Even with the same result, "I'm not cut out for this" (W → self-evaluation) and "this is a hole in the procedure" (W → structure) leave different O_int, so the update direction diverges. Hence "anyone improves with experience" does not hold; what improves you is not the quantity of O_ext but the quality of the interpretation P. [Hypothesis]

Ripple of update: n_p frees up (chunking [Established]) → m can dig deeper → Θ widens and stage ② becomes ① ("it got easier") → W moves. Conversely, if O_int does not remain (m stays shallow in routine), only the count increases and C is not updated.

Under this structure, "the individual" is defined not as a bundle of fixed attributes but as a **recursive system that continually updates itself while receiving Input from the world and returning Output**. This is also a structural explanation of "why people change."

> Caveat: this too can explain anything after the fact. It becomes testable only when differing O_int from the same O_ext can be separately observed. [Hypothesis]

---

## 7. Origin — Infinite IPO Continuum and OPI

The "→" is also Process, and O and Pk are re-fed as new I. Accepting both, cognition can be expressed not as a single IPO but as an infinite continuum.

```
… → I → P → O → I → P → O → …
```

On this continuum, **the origin is not fixed**. Where to start reading is a matter of the observer's or the person's own framing. Read from I, it is IPO; read from O, it is OPI.

- **OPI**: a pattern of experiencing/describing from O (the point where a prior cycle's O_int surfaces as conviction) as the origin. Not a different ability, but the same continuum read from a different origin.
- **Creation = freedom to choose the origin**: take O as the origin and support it afterward with P (verbalization) and I (material procurement). With a fixed origin (always from I), only combinations of given materials emerge.
- **Two kinds that look like "intuitive types"**: the OPI type (conviction first, materials later) and the ultra-fast IPO type (origin is I but processing is so fast it looks intuitive). Their internal order differs, but **there is currently no operational definition to distinguish them from outside or even by the person themselves**.

> Caveat: freedom of origin cannot be judged from outside (ultra-fast IPO type and OPI type are indistinguishable), and falsifiability is nearly zero. This is not a "measuring claim" but a "device for adding viewpoints." Its value lies in generativity, not predictive power. [Speculation]

---

## 8. Qualia (Treated as Attribution)

Three transformation surfaces are introduced: the perception surface (I→P), the expression surface (P→O), and the social boundary surface (A↔B).

Qualia (the subjective feel) is described as an **attribution constructed** by observer B from signals appearing at the boundary surface of the other A. The phenomenon of humans inferring the inside from an AI's output and attributing subjectivity to it has exactly the same generative mechanism as the inter-human case. The model states only the **identity of the generative mechanism** of attribution; it does not judge the **validity** of the attribution (whether an internal state actually exists). [Speculation]

**Ontological status of boundary surfaces**: the transformation points I→P and P→O are lines of an observation grid drawn on a continuum, but **only the A↔B social boundary surface is not a line drawn by the observer but a physically real division** (the two cognitive systems are separate systems). The model treats three points as digital cuts: phase transition (§4), Θ-crossing (§5), and the inter-individual boundary (this section).

> Scope (limited): what is explained is how attribution arises (the side of the other-minds problem), not why feeling accompanies it (the hard problem of consciousness). First-person qualia is unobservable and external to the model. **Within the model, qualia always appears only as "attribution."** [Speculation]

---

## 9. Summary of Confidence

| Element | Grounding (nearest existing concept) | Confidence |
| --- | --- | --- |
| I/P/O・W | goal orientation, cognitive style | [Hypothesis] |
| n_p ↔ working memory | Miller 7±2, WM capacity | [Established] |
| vector decomposition of n (n_i/n_o independent) | construal level, perceptual differentiation | [Hypothesis] |
| m (depth of processing) | levels of processing | [Hypothesis] |
| n_p → m constraint | — | [Hypothesis] |
| α・Θ・Δ (3-layer correction) | attention lapse, cognitive load, signal detection | [Speculation] |
| self-update of C | Bayesian updating | [Speculation] |
| freedom of origin, OPI | — | [Speculation] |
| qualia attribution | other-minds problem, intentional stance | [Speculation] |

---

## 10. Open Questions (Summary)

The greatest task is **operational definition**: can measurement methods (proxy indicators) be made for W, m, α, Θ, Δ? Besides that —

- Trait or state (should W be treated as a situation-dependent continuous distribution?) / do I, P, O exist, and what is the distribution?
- Are n_i, n_p, n_o independent or correlated? / Does the upper bound of n_p match WM capacity?
- Is the interface-round-trip redefinition of m (I/P, P/O, P/P') valid? / Can the conditions for deep processing be made more precise?
- Are α, Θ, Δ three independent parameters? / Is Δ a single ability or a bundle per action point (is double dissociation observed)? / Does Θ have hysteresis?
- Is C self-updated per cycle? / Under what conditions does the update direction diverge from the same experience?
- Conditions for the generation of qualia attribution / are attribution to humans and to AI structurally identical?
- Can an operational definition be made to distinguish the OPI type from the ultra-fast IPO type?
- **Difference from existing theories**: do goal orientation, levels of processing, WM capacity, and construal level theory show a measurable difference? (If not, it remains a re-description ← the crux.)

> Evaluation policy: this model is a high-abstraction interpretive model, and its evaluation does not rest on falsifiability alone; subjective matching and explanatory power are also material for judgment. However, "an explanation that explains everything predicts nothing" is always kept as a counterweight. The scope is limited to the domain humans can cognize and observe; the outside is treated as external to the model.

---

## 11. Record of Development

Main developments from the starting point.

- **Redefinition of n**: originally n was a single scalar, the "number of Process divisions." This was a **projection** arising because the model's author was a P-type and saw only the resolution of P as high. Redefined as a vector `(n_i, n_p, n_o)` with resolution for each of I, P, O. The old division count corresponds to n_p (and the depth delegated to m). The realization that **the model's shape reflected the author's own C** led to the summary that all variables can have three-axis components (§5).
- **Redefinition of m**: originally "number of IPO unit chains" (horizontal repetition), but as n was redefined as width, m was reorganized as "depth of processing" (vertical). Chaining was integrated as the external unfolding of depth (§4).
- **Separation of the correction layer**: state variables (W, n, m) and correction parameters (α, Θ, Δ) were separated as layers, making the formula `C = (W, n, m | α, Θ, Δ)`. The signature `IPO × C` was placed above (§0).
- **Explicit temporality / auxiliary notation**: added the self-update C_t → C_t+1 and the auxiliary notation O_ext / O_int (§0, §6).
- **Pruned branches**: the comparison of superiority with learning-style theory, and the connection to the philosophical zombie problem. The former is unnecessary to the main line; the latter merely accepts the premise of the zombie argument and is neither a solution nor a re-description, so it was removed. Qualia remains only as "attribution" (§8).
