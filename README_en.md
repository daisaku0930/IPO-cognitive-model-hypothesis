# IPO Cognitive Model — Source Text

> A starting-point map for re-framing human cognition in engineering terms.

---

## What is this?

People look at the same situation but differ in **where they direct their attention**.

This model captures all human cognition as a flow of Input → Process → Output, and provides a framework to observe, describe, and operate on those differences. It is not a "theory" but an observational framework. It is formalized (has notation) but not operationalized (has no measurement methods).

---

## Model Structure

```
IPO × C

C = (W, n, m | α, Θ, Δ)
```

- **IPO**: the flow axis (Input → Process → Output)
- **C**: the state axis (the current cognitive configuration)
- **Left of the bar (W, n, m)**: state variables
- **Right of the bar (α, Θ, Δ)**: correction parameters (P layer)

| Variable | Meaning |
| --- | --- |
| W | direction of attention allocation (where among I/P/O attention is directed) |
| n | resolution vector `(n_i, n_p, n_o)` (granularity of input / parallelism / output) |
| m | depth of processing (recursion stages inside P) |
| α | firing probability of correction |
| Θ | threshold of unconscious correction (boundary of ①↔②) |
| Δ | upper limit of correction capacity (boundary of ②↔③) |

---

## What this model can explain

- **Conversational mismatch**: described via IPO structure as a gap in W and n, not a difference in ability
- **Why teaching fails to land**: described as the difference in n and m between sender and receiver, corrected by Δ
- **Why people change**: explained as a dynamic loop in which O_int self-updates C (C_t → C_t+1)
- **Conditions for learning and creation**: described as a phase transition where an intermediate product Pk turns into I'
- **Qualia**: described as an attribution constructed by observer B from A's boundary surface (B's O)

---

## Structure (§0–§11)

| Section | Content |
| --- | --- |
| §0 | The formula (model signature and state definition) |
| §1 | Skeleton — IPO and three orientations |
| §2 | W — direction of attention allocation |
| §3 | n — resolution (width of interface and parallelism) |
| §4 | m — depth of processing |
| §5 | Correction — α・Θ・Δ |
| §6 | Update — self-update of C |
| §7 | Origin — infinite IPO continuum and OPI |
| §8 | Qualia (treated as attribution) |
| §9 | Summary of confidence |
| §10 | Open questions (summary) |
| §11 | Record of development |

---

## License

**CC BY 4.0 (Creative Commons Attribution 4.0 International)**

As long as the source (Daisaku Nagano) is credited, anyone is free to modify, research, run empirical tests, or use commercially, without prior notice.

---

## Message from the author

This model is published as a starting-point map. The author does not plan active updates or moderation of discussion.

Feel free to fork, test, extend, and evolve it in your own domain. Issues are welcome.

---

## Files

| File | Content |
| --- | --- |
| `README.md` / `README_en.md` | Overview and entry point |
| `IPO_model_genten.md` / `IPO_model_genten_en.md` | Full source text (§0–§11) |
