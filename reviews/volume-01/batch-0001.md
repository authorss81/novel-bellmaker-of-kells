# Review Record — Volume 01, Batch 0001 (Chapters 1–10)

**Reviewer pass:** `logs/phase-002-batch-plan.review.log`
**Commit reviewed:** `62b3616` (novel: save writer work phase-002-batch-plan)
**Repair pass:** applied to chapters, state, and the next batch prompt. No controller file was edited.

## Disposition

| ID | Finding | Status | Where |
| --- | --- | --- | --- |
| A1 | Batch 0001 prompt unmarked, so the next dispatch would re-run and overwrite Chapters 1–10 | **Fixed** | `workspace/volume-01/batch-0001/.done` |
| A2 | `state/phase-ledger.json` stale (`phase-000-bootstrap`, `planned`, `attempts: 0`) | **Flagged, not edited** | see below |
| B1 | Ch 4/5 had characters answer a notice posted three days *later* | **Fixed** | chapters 4, 5 |
| B2 | Ch 5 inferred precedence from an off-page market-court visit and duplicated Ch 6's hidden-date beat | **Fixed** | chapter 5, and state notes |
| B3 | Ch 6 mixed elapsed and inclusive counting for the posted notice | **Fixed** | chapter 6 |
| B4 | Batch 0002 asked for 10 chapters in a 7-day window with no day map | **Fixed** | `workspace/volume-01/batch-0002/PROMPT.md` |
| C1 | State claimed the missing surveyor was "not identified" and that Oren never gave the name | **Fixed** | continuity, open-threads, character-state, current, prompt |
| C2 | "Supervised comparison" conflated Oren's arranged watching with the unwatched stairway reading | **Fixed** | continuity, character-state, current, batch summary, prompt |
| C3 | Three surveyor roles existed; state tracked two | **Fixed** | continuity, open-threads, prompt |
| D1 | Ch 3 staged the handbell on an interior bench while Tamsin was still outside | **Fixed** | chapter 3 |
| D2 | Repeated "looked back" gesture inside one chapter | **Fixed** | chapter 3 |
| D3 | Ch 1 still called the delivering official "the clerk" | **Fixed** | chapter 1 |
| E | Ch 5 (1,617), Ch 4 (1,714), Ch 1 (1,749) under the 2,200–3,200 guidance | **Fixed** | chapters 1, 4, 5 |
| F | No `reviews/volume-01/batch-0001.md`; `NOVEL_SPEC.md` lacked a trailing newline | **Fixed** | this file; `NOVEL_SPEC.md` |

## Repair notes

**A1** is the one finding that would have destroyed work rather than degraded it. `scripts/novel_runner.sh:25-31` sorts every `PROMPT.md` under `workspace/` and takes the first without a `.done` or `.blocked` marker. `workspace/volume-01/batch-0001/` had no marker because Batch 1 was written during the `phase-002-batch-plan` phase, whose prompt is a controller phase, not a batch directory. An empty `.done` file was created, matching the runner's own convention at line 240. The selector now resolves to `workspace/phase-002-batch-plan`. No dispatch, phase-selection, timeout, retry, or checkpoint code was touched.

**A2 is controller-owned and was deliberately left alone.** `state/phase-ledger.json` is on the never-edit list in `AGENTS.md`, and the stale reading comes from a prompt conflict: `workspace/phase-002-batch-plan/PROMPT.md` asks the writer to "update … and phase ledger" while `AGENTS.md` and the Batch 0002 prompt forbid it. `PHASE_SYSTEM.md:187` says the selector reads the ledger, but no code path in `novel_runner.sh` does — it scans marker files. Two options for the controller owner, not for this pass: drop "and phase ledger" from the phase prompt, or make the ledger authoritative and have the selector honour it. Until then the ledger and the repository disagree, and the marker scan is what actually runs.

**B1** was the subtlest prose defect, because the fix pass had just made the notice's date load-bearing. Jory and Edan Fenn now answer the **previous renewal round**, anchored on the page: Chapter 5 has the lodger state that Low Ward rolls are recounted on a published cycle and that the board posts each round a week ahead, Nell's paper is "a renewal check" rather than "the notice," Edan went "to answer a renewal summons," and Chapter 4's Nell says her father answered "a Crown summons." No character now refers to a posted L-4 notice before Day −3.

**B2** moved the Ch 5 inference onto evidence Tomas can actually hold. He now reads the date beneath the fragment's seal and checks it against the day-book he already keeps to bill customers — arithmetic, not prophecy. The market-court board and its small hidden line remain Ch 6's discovery, so the reversal still lands publicly in the place the outline reserves for it. Continuity, the batch summary, and the next prompt were all rewritten to match; three of them had asserted the old off-page visit.

**B4** is the finding most likely to have cost the next batch its structure. The prompt's cards read "first full day of the seven-day stay" → "morning after" → "next morning" → "evening before," with nothing fixing the intervening chapters to any day, so a writer could have run the rescheduled dawn past without noticing. The prompt now carries a binding ten-row table (Ch 11–20 on Days 3–9, dawn on Day 10), each card's time line was rewritten to match, and the flood is capped at a Day 7 crest so Days 8–10 stay available for civic business. The table is declared to win over the cards on any conflict.

**C1** was the finding that had inverted the evidence. Chapter 8 has Oren say "His name is Iven Sore" and name the service ticket outright; the state files told the next batch the name was withheld. All five locations now agree with the prose and describe the real ambiguity — **genuine or borrowed** — quoting "Could be" rather than inventing a silence. Chapter 14's card was rewritten, since its resistance depended on the wrong premise.

**E** was closed with new scene material rather than rebalancing, so no good prose was cut. Chapter 1 gained the flooded-out flood bell that pays off its own opening line, a porter sent to hold the yard gate, Pever's line about the order coming from the survey store rather than from him, and Tomas reading the handprint's sequence out to a man who writes dimensions instead. Chapter 4 gained the customer who walks out over the bench and Sabin demonstrating the refusal test on himself, which is what the state files had been claiming he carried as unstated guilt. Chapter 5 gained the landlady's unnamed woman in the room above, Nell's account of managing her mother, and the same round-cycle anchor B1 needed. Final counts: Ch 1 2,299, Ch 4 2,233, Ch 5 2,229.

## Carried forward

- Whether the **Iven Sore** name on the withdrawn service ticket is genuine or borrowed. If genuine, the guild master and the missing surveyor are one man.
- **Three surveyor roles** stay distinct: Pever (present), the missing Chapter 8 docket surveyor, and Halden's unnamed inspection surveyor who is due at the rescheduled dawn.
- The **watch-supervised comparison** Oren arranged in Chapter 3 is still owed. The stairway reading was private and unwatched, and no state file may imply otherwise.
- Chapters 21–30 keep the copied answer, the Silent Muster's name-transfer mechanism, the higher official, the archive fire, the Bellhouse closure, and Tomas's departure. None was touched here.
