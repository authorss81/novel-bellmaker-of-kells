# Volume and Batch Index

**This file exists because summary filenames do not match batch numbers.** `state/batch-000N-summary.md` is the **global** batch number, counted across the whole novel. It is **not** the batch number inside a volume. Picking a predecessor summary by filename will pick the wrong file: **`state/batch-0005-summary.md` is Volume 01 Batch 0005, and Volume 02 Batch 0005 is `state/batch-0010-summary.md`.**

**Always resolve a predecessor summary through the table below, never by arithmetic on the filename.**

## The load set

Read these five. Everything else in `state/` is history and should be opened only when a specific fact is needed and its location is known.

| file | what it is | size class |
|---|---|---|
| `state/current.md` | **immediate state only** — where the manuscript is, object custody, the document register, ground, power, the two house rules | short |
| `state/continuity.md` | **the binding canon** — the one clock, the rules, the boundaries, the do-not-age list, the canon corrections | the one long file |
| `state/character-state.md` | who everybody is and what this volume did to them | short |
| `state/open-threads.md` | the live threads, and only the live ones | short |
| `state/volume-index.md` | this file | short |

`state/chapter-summaries.md` is **archive tier and is not in any batch prompt's read list.** Per-chapter detail for a batch is in that batch's summary. `state/batch-000N-summary.md` is the record of how a batch went and is read one at a time, not all ten together.

## Batch map

| global batch | volume | batch dir | chapters | days | summary file | prompt |
|---|---|---|---|---|---|---|
| 0001 | 01 | `workspace/volume-01/batch-0001/` | 1–10 | 0–4 | `state/batch-0001-summary.md` | spent |
| 0002 | 01 | `workspace/volume-01/batch-0002/` | 11–20 | 5–9 | `state/batch-0002-summary.md` | spent |
| 0003 | 01 | `workspace/volume-01/batch-0003/` | 21–30 | 10–15 | `state/batch-0003-summary.md` | spent |
| 0004 | 01 | `workspace/volume-01/batch-0004/` | 31–40 | 16–21 | `state/batch-0004-summary.md` | spent |
| 0005 | 01 | `workspace/volume-01/batch-0005/` | 41–50 | 22–33 | `state/batch-0005-summary.md` | spent |
| — | 01 | `workspace/volume-01/audit/` | volume audit | — | — | spent |
| 0006 | 02 | `workspace/volume-02/batch-0001/` | 51–60 | 34–44 | `state/batch-0006-summary.md` | spent |
| 0007 | 02 | `workspace/volume-02/batch-0002/` | 61–70 | 45–55 | `state/batch-0007-summary.md` | spent |
| 0008 | 02 | `workspace/volume-02/batch-0003/` | 71–80 | 56–66 | `state/batch-0008-summary.md` | spent |
| 0009 | 02 | `workspace/volume-02/batch-0004/` | 81–90 | 67–76 | `state/batch-0009-summary.md` | spent |
| 0010 | 02 | `workspace/volume-02/batch-0005/` | 91–100 | 77–86 | `state/batch-0010-summary.md` | spent |

**The rule: global batch number = (volume − 1) × 5 + batch-within-volume.** Volume 01 has five batches and one audit; Volume 02 has five.

**Volume 01, *The Bell Before the Crime*, is complete at Chapter 50. Volume 02, *The Unpaid Names*, is complete at Chapter 100.** Day 0 is the morning the carrier arrived at the Vale Bellhouse. Chapter 100 falls on Day 86.

## One volume arc per line

- **Volume 01 — The Bell Before the Crime (Ch 1–50, Days 0–33).** A Crown survey carrier arrives with its clapper missing. A ward answers a form out loud in four columns. The archive burns, the yard is sealed, and Tomas Vale is taken out of his own lane. A district withdraws a finding, a captain releases a bell in a cradle that cannot be rung, and a bellmaker leaves Kells before dawn with a question he cannot answer.
- **Volume 02 — The Unpaid Names (Ch 51–100, Days 34–86).** A man with a barrow walks four counties with a list that cannot be unrolled. Nine pitches come off a market and a child goes on a cart. A man with no standing says one true sentence in a room and it costs a household a row. A practice is stopped in one district in writing. A room, a bench and the only copy of a form are taken lawfully under a clause he asked for. He rings a bell he did not make in a market square, apologises to about nine hundred people, and walks out of a town of two thousand with a barrow and no place.

## Known gaps in the planning layer

- **There is no `outline/volume-03.md`.** `outline/series.md` and `outline/ending.md` are the only Volume 03 planning documents that exist. A volume outline has to be written before Volume 03 chapters can be planned against one.
- **Two Volume 02 payoffs were required by `outline/volume-02.md` and are not paid**, and are recorded in `state/current.md` and `state/open-threads.md`: **Mara Vale does not appear anywhere in Volume 02**, and **the Silent Muster is never proved**. Both are carried into Volume 03 as its first obligations. `outline/volume-02.md` has been amended to record the deferral rather than to pretend the payoff landed.
