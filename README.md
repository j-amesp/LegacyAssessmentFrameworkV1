# The Legacy Assessment Framework

A vendor-neutral instrument for assessing whether a system can still be changed — and for turning legacy from a surprise into a managed trajectory.

**Version 1.0  ·  May 2026**

---

## What this is

Most organisations can recognise the symptoms of legacy. Far fewer can describe the underlying condition consistently enough to act rationally and early. This framework exists to close that gap.

It treats legacy not as old technology, but as **lost optionality** — the gradual erosion of an organisation's ability to change, move, replace, or modernise a system without a coordinated, high-risk rebuild. A ten-year-old system can be highly evolvable. A six-month-old system can already exhibit classic legacy behaviours. The difference is not age. It is whether the system can still change safely, economically, and with confidence.

The framework assesses that condition across seven dimensions, scores them against anchored descriptors, and rolls the result up to a system-level rating that survives a hostile review.

## What's in this repository

| File | What it is |
|---|---|
| `The_Legacy_Assessment_Framework_V1.0.pdf` | The full framework document. Read this first. |
| `Legacy_Assessment_Framework_v1.0.xlsx` | The operational workbook — per-component assessment sheets, gating logic, evidence discipline, and a system-level dashboard. |

## The seven dimensions

The framework measures optionality across seven headings, ordered deliberately from the artefact to the people to whether you can actually move:

1. **Portability** — Can it be moved?
2. **Modularity** — Can one part change without forcing the rest to change?
3. **Integration** — Can its connections be changed plug-and-play?
4. **Modernisation** — Can the language and code be brought forward?
5. **Embedded IP** — Is critical bespoke logic buried and unextractable?
6. **Knowledge Transferability** — Can anyone pick it up and work with it?
7. **Observability & Testability** — Can you change it with confidence rather than on faith?

Each heading carries five tests, anchored at scores 1, 3, and 5. Twelve of the thirty-five tests are designated **gating tests**: a low score on a gating test floors the heading regardless of the others. The weakest load-bearing element governs.

## How to use it

**Read the PDF first.** It's the authority. The workbook operationalises it.

**Then open the workbook.** Start on the *Instructions* sheet — it sets the calibration rules, the gating logic, the RAG thresholds, and the roll-up rule explicitly so the instrument is defensible in front of a programme team with a budget and a reputation to defend.

**For each component:**

1. Complete the header block — name, owner, assessor, date, mode, dependency classification, trajectory state.
2. Score each of the thirty-five tests against the anchored descriptors. Pick a score from the drop-down (1–5, or N/A where genuinely inapplicable).
3. Record evidence status (Present / Partial / Absent), what the evidence is, and who is responsible for it. *Evidence beats assertion. If it cannot be shown, it is not a 5.*
4. The workbook computes each heading rating using the gating rule, then the component rating from the worst heading.

**For the system:** complete the *System Dashboard*. The system rating is set by the worst rating among components classified as **Load-bearing**. Contributing and Peripheral components are visible as context but do not drive the headline.

Evidence indicators for every test sit as cell comments on the test title — hover and they appear.

## Calibration rules

These rules sit ahead of the tests because they are what make the framework defensible:

- **Demonstrated reality, not intent.** The score reflects what is true now, not what is planned.
- **Score as-is, not as-designed.** The cost of restoring optionality is the output, not an input.
- **When uncertain, score down.** A defensible amber is worth more than a flattering green.
- **Evidence absent ≠ score skipped.** If evidence cannot be obtained, score the floor and flag the absence. The flag preserves the distinction; the score does not let the gap hide.

## Two modes of assessment

- **Full assessment** runs all thirty-five tests. At design baseline, go-live, major architectural change, and at least annually for load-bearing components. The go-live score is the registered baseline and is non-optional.
- **Light check** runs the twelve gating tests only, fed wherever possible from telemetry. Quarterly, or continuously where instrumentation allows. Its job is to detect movement on the tests most likely to floor a heading and to trigger a full assessment. *The light check is the smoke detector; the full assessment is the inspection.*

## A note on neutrality

The framework measures optionality. It does not road toward any product, supplier, or remediation approach. A green score does not imply migration. A red score does not prescribe a supplier. The rating is only worth defending if the framework was capable of returning the answer no one wanted.

## Known open areas

Version 1.0 deliberately leaves two areas open. Numeric dependency weighting is not used as the spine because categorical roll-up is what survives a hostile review; a weighting layer may be added later as a tiebreaker for ranking multiple red systems against a finite remediation budget. Assessor competence is not defined by the framework; consistency depends on the anchored descriptors, the evidence indicators, and continuity of assessors across consecutive assessments.

## Licence
The framework and workbook are published under the Creative Commons Attribution 4.0 International License (CC BY 4.0). See License.MD for terms.

## Author

**James Patrick CITP MBCS**  
Chief Field Architect - Defence and National Security, Oracle · Member, techUK National Security Committee

*I work for Oracle. These views are my own. The framework is deliberately vendor-neutral — it was designed to be capable of returning answers nobody wanted, including answers that don't favour my employer.*
