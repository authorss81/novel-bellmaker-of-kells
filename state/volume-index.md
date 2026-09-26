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
| 0011 | 03 | **no phase directory — see the note below** | 101–110 | 87–96 | `state/batch-0011-summary.md` | spent |
| 0012 | 03 | `workspace/volume-03/batch-0002/` | 111–120 | 97–106 | `state/batch-0012-summary.md` | spent |
| 0013 | 03 | `workspace/volume-03/batch-0003/` | 121–130 | 107–116 | — | **next** |

**The rule: global batch number = (volume − 1) × 5 + batch-within-volume.** Volume 01 has five batches and one audit; Volume 02 has five; Volume 03 has five.

**Volume 01, *The Bell Before the Crime*, is complete at Chapter 50. Volume 02, *The Unpaid Names*, is complete at Chapter 100. Volume 03, *The Quiet Office*, is open and Batch 0002 is complete at Chapter 120.** Day 0 is the morning the carrier arrived at the Vale Bellhouse. **Chapter 100 falls on Day 86, Chapter 110 on Day 96, and Chapter 120 on Day 106. The volume closes on Chapter 150 on Day 136, and there are three more batches after Batch 0002.**

## One volume arc per line

- **Volume 01 — The Bell Before the Crime (Ch 1–50, Days 0–33).** A Crown survey carrier arrives with its clapper missing. A ward answers a form out loud in four columns. The archive burns, the yard is sealed, and Tomas Vale is taken out of his own lane. A district withdraws a finding, a captain releases a bell in a cradle that cannot be rung, and a bellmaker leaves Kells before dawn with a question he cannot answer.
- **Volume 02 — The Unpaid Names (Ch 51–100, Days 34–86).** A man with a barrow walks four counties with a list that cannot be unrolled. Nine pitches come off a market and a child goes on a cart. A man with no standing says one true sentence in a room and it costs a household a row. A practice is stopped in one district in writing. A room, a bench and the only copy of a form are taken lawfully under a clause he asked for. He rings a bell he did not make in a market square, apologises to about nine hundred people, and walks out of a town of two thousand with a barrow and no place.
- **Volume 03 — The Quiet Office (Ch 101–150, Days 87–136).** A bell on a post above a notice-board rings with nobody near it, and the sheet under it is dated four days forward, and the whole of a coercion is arithmetic. A smith says a store in four seconds and refuses a theory. A bell is on a roll with an empty keeper's box. A leaf on a public board confirms a sister's hand and refuses to answer, and it is not taken. A woman with a slate finds a form with a box for the person who repeated a thing, and rings her own bell once in a market of about nine hundred people. Three sheets go on a trestle and a clause of a larger Renewal operation is read out to four hundred people. A notice in his own name goes on a board because a man with no standing cannot be served a document. A clerk at a counter names the second kind of paper. **A format has no door, and ninety-six days of learning to ask a person end at a building there is nothing in to ask. Then a city: the flat and its waiting bells, a counter that takes papers and not people, a court that publishes, a wire nobody can blame, a store with a column nobody will fill in, a hearing held off the page, a public record of it that says the person named produced nothing, a clerk who put his own hand on a public wall and lost four days, and three people in three yards who each said one true thing and were not thanked. And a man who has got one of the three answers, and not two, and not three: *if there were three of me.*

## Known gaps in the planning layer

- **THERE IS NO `workspace/volume-03/batch-0001/` DIRECTORY AND THERE NEVER WAS ONE.** Batch 0011's ten cards are `outline/batches/volume-03-batch-0001.md` and the prose is `chapters/volume-03/chapter-0101.md` to `chapter-0110.md`. Earlier drafts of this table and of `state/current.md` pointed at a phase prompt directory that was never created, and that dead path has been removed rather than left for a later writer to open. **Every other row in the table is a real phase directory with a tracked `PROMPT.md` and a `.done` marker; this one is the exception and is now marked as the exception in the row itself.**
- **`outline/volume-03.md` EXISTS** and was written before the first Volume 03 chapter, after the Volume 02 close, because `state/current.md` and this file both named the absence as a real gap. `outline/batches/volume-03-batch-0001.md` holds the ten chapter cards. **The volume runs to Chapter 150 and closes there.**
- **The two Volume 02 payoffs are BOTH PAID**, in Volume 03 Batch 0001, in the required order: **Mara Vale's trail in Chapter 0105** and **the Silent Muster proved by a document and a date in Chapter 0107.** The record of what was paid and of what each payment deliberately did not do is `state/continuity.md` §11. `outline/volume-02.md` and `state/continuity.md` still carry the deferral note as history; **§11 of the continuity file is the live statement and it says PAID.**
