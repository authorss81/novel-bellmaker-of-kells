# Volume 01 Audit — Review Repair

**Phase:** repair of the findings in the review of the volume-close audit. **Scope:** `reviews/volume-01/volume-audit.md` and the commits it produced, checked against the prose. **Rule followed throughout:** fix the concrete finding, keep the good prose, restart nothing, change no planned plot.

**Result: all seven actionable findings are fixed and one is correctly a no-action.** No chapter was restarted, renumbered or reordered. No card, day map, character outcome, ending or volume direction was touched. Two lines of prose changed, in two chapters, and both changes are removals or alignments inside a line that was already there.

---

## The recurring failure class, named once

Every actionable finding in this review is one failure, and the audit itself predicted it: **a state file was allowed to stand as evidence about a chapter.** Five separate reviews had already asserted a clean sweep that had not been run. This time the prose was clean and the state layer was not.

| Finding | Class | Fixed in |
| --- | --- | --- |
| D1 — a batch summary still said the Fourmile cart did not come *on the Friday* | state asserts repaired prose | `state/batch-0005-summary.md:24` |
| D2 — a chapter summary still said a woman quoted Tamsin's *Saturday* reasoning | state asserts repaired prose | `state/chapter-summaries.md:169` |
| **D6** — two state files still carried the chandler's *from Monday* as live | state asserts repaired prose | `state/continuity.md:163`, `state/batch-0003-summary.md:61,96` |
| **D1b, found by re-running the sweep and not in the review** — a chapter summary still said Marda Hodler *will wait until Friday* | state asserts repaired prose | `state/chapter-summaries.md:133` |
| D3 — an age removal left two distinct women both introduced as a bare *a woman* | repair caused a prose regression | `ch45:155` |
| D5 — one woman, one house, two conflicting ages | a defect the audit's scoped sweep never looked for | `ch36:129` |
| D4 — an age the audit had removed was retained in the same line and not disclosed in the audit's own claim | the record, not the prose | `ch45:155` and three state entries |
| D7 — two named facts in the Volume 02 outline not flagged for provenance | process | `outline/volume-02.md`, `outline/batches/volume-02-batch-0001.md` |

**Six live stale weekday references were found in `state/`, five named by the review and one not.** A single search across the state layer would have taken them all at once, which is the whole of the lesson and is now written into the next batch's prompt.

## D1 — high. The cart that did not come

`state/batch-0005-summary.md:24` said the cart from Fourmile did not come **on the Friday**. `ch48:141` puts it in Teage's own mouth: *my brother-in-law was to bring a cart from Fourmile **on the morning of the twenty-sixth**, and he did not bring it.* This is the load-bearing fact the Batch 0005 review repaired in the chapter, and the summary was still supplying the weekday the prose no longer has.

**Fixed to the chapter.** This is the highest-risk item in the review, because it is the one most likely to walk back into Volume 02 prose as a fact about a day.

## D2 — high. The reasoning that no longer exists

`state/chapter-summaries.md:169` said Mrs Wilde **quotes Tamsin's Saturday reasoning back**. `ch40:139` now reads *I am not going to at the next one either* — a refusal with no date in it, which is what Tamsin is saying. The summary pointed at text that had been deleted.

**Fixed to the chapter:** *She quotes Tamsin's **refusal to ring at the next one** back.*

## D6 — low-medium. The chandler's Monday

`ch23` now reads **from the start of next week** and three state lines still described *from Monday* as live prose. **All three corrected**, and the correction in `state/batch-0003-summary.md:96` is written so that it is clear the sentence now records a repair rather than a fact about the batch. The forward reference and the cruelty of the sentence both survive, which was the reason the audit chose that replacement.

## D1b — the one the review did not find

Re-running the review's own search across the whole state layer turned up a sixth live stale weekday reference, in the same class and in the same chapter the audit had already repaired: `state/chapter-summaries.md:133` said Marda Hodler **will wait until Friday**, where `ch33` now says **the nineteenth**. **Fixed to the chapter.** This is recorded because it is the exact failure the audit was written to prevent, happening once more in the state layer rather than the prose, and it is the reason the next batch's prompt now says to search the state layer and not only the chapters.

## D3 — medium-high. The sentence the age repair broke

Removing *of about thirty* at `ch45:155` left Mercy Slee describing two different women — **Mrs Corris**, who put her hand up, and **Mrs Wilde**, who read her question at the side of the clerk's table — as two identical bare phrases in a sentence whose entire subject is *who did what*. The chapter had already named both of them, and had already shown both of them doing exactly those two things, at `ch45:127` and `ch45:97`.

**Fixed by naming them, and by nothing else.** One sentence changed; the argument, the rhythm and the closing *a girl of sixteen gave seven away for nothing* are untouched, and naming the two women is a stronger line than two anonymous figures were. The reader can now tell which woman Mercy means, which is what the sentence was for.

## D4 — medium. The retention that was disclosed, and the claim that was not

The review found the audit's finding 3 claiming the age was *all four removed* and *true of the whole volume* while `ch45:155` still read **a woman of sixty-five** in Mercy Slee's mouth.

**Half of this was already handled, and the record should say so.** `state/continuity.md` and `state/character-state.md` both carried the disclosure — *one attributed repetition in Mercy Slee's mouth at Chapter 45 line 155*, and *the Batch 0005 ruling that an attributed repetition is canonical stands*. The gap was narrower than the review states: the state layer had it, and **the audit's own prose did not**, and neither did the compressed one-line age note in `state/chapter-summaries.md`.

**Resolved by removal rather than by disclosure, because D3 forced an edit to that exact line anyway.** With the two women named, an age attached to one of them would have been the only age for a listed character in the sentence — the thing the audit spent itself eliminating. So the fifth instance is gone, and **all four state entries that described it as a surviving canonical exception are corrected to say it was removed**, with the reason stated plainly: *nothing was removed for being an age; it was removed for being the thing standing between a reader and the referent.* The Batch 0005 ruling that an attributed repetition is *permitted* is untouched and still stands; the repair removed this one line for a different reason.

## D5 — medium. One woman, one house, two ages

**Sena Dunn, of 121, had two conflicting narrator-supplied ages: *about forty-five* at `ch36:129` and *about fifty* at `ch42:161` and `ch45:11`.** Same house, same woman — the tie is the boy of eleven taken on the tenth day, and she is the woman who asked *which child* four times at that door. The audit's sweep was scoped to four listed characters, and a listed character with two *conflicting* figures was not on its list, which is why it survived.

**Resolved by alignment, not by removal.** `ch36:129` now reads **about fifty**, keeping the later pair: `ch36` is where she is physically introduced and the mended good coat, the arcade and the clerk are load-bearing there, and two of the three instances said fifty. **Her age is permitted and is recorded in `state/character-state.md` and in the do-not-age block of `state/continuity.md` as *about fifty, and no fourth instance may say otherwise*.** One detail was corrected while checking: the mended coat appears **only** in `ch36`, and the record now says so, so that no later writer treats it as a second identifying detail and reasons forward from it.

## D7 — process. The two names in the Volume 02 outline

The review flagged **Jory Fenn** (eight, taken before the L-4 notice) and **Marta Vell** (entered on a Fourmile schedule as a bell of Kells with no keeper) as possible new canon requiring a flag.

**Both are already on the page in Volume 01, and neither is a proposed canon change.** Jory is at `ch5:15,21,47,145` and `ch20:149`; Marta Vell is named by Tamsin at the towpath at `ch50:229–231`, including that she is about sixty **on Tamsin's word** and that nobody has told her about the schedule entry. **The right fix was therefore provenance, not a flag:** a new **Provenance of the inherited facts** block in `outline/volume-02.md` citing the chapter for each, so no later writer treats either as an invention.

**One real error came out of the same check, and it is corrected.** The outline listed *a sister's count* among the available records of Jory. **The count is spent.** Nell Fenn made it on the twelfth, kept it nineteen days, and spent it on the evening of the thirtieth on a single written question to the district, and says she has about four hours of use out of it and cannot account for the rest (`ch50:11`). The volume outline and `outline/batches/volume-02-batch-0001.md` line 13 both carried the stale list; **both now record it as spent and forbid Chapter 51 from using it as an available record.** The same collision was already caught in the batch prompt, which had it right.

## D8 — process, and correctly no action

`state/phase-ledger.json` still reads `phase-000-bootstrap` / `planned` / `attempts: 0` after five completed batches. **It was not edited.** It is controller-owned, and this repair did not touch a controller file. The staleness is a real reporting hazard, and the correct response to it is that **nothing in the fiction or the state layer describes the ledger as authoritative** — which remains true.

---

## What was not changed, and deliberately

No plot, no card, no day map, no character outcome, no ending, no volume-01 direction, no power level. Tomas gains no stage and perceives nothing; Tamsin is not rescued and her hearing stays permanent; the Crown's answer about the persons under seventeen is still answered in print and the answer is still a form. **No new final enemy.** Pell Rill is still a Volume 02 adversary to be earned and is still absent from Batch 0001 in any form. **OFF. 411 is still a mark on four papers in four hands and a district renewal desk, not a man.** The Crown clapper is still unnamed in prose, and the repair to `ch45:155` did not touch it.

**The two prose edits, in full:**

1. `ch45:155` — the two women are now named, and the age went with the naming. Nothing else in the line moved.
2. `ch36:129` — *about forty-five* → *about fifty*, to agree with the same woman at `ch42:161` and `ch45:11`.

**A general rule this repair adds, beside the one the audit added about half a chapter:** a repair that removes a word can break the sentence it was in, and the breakage will not show up in a search for the word. `ch45:155` was correct on the do-not-age rule and unreadable as prose at the same time, and the second fact was only visible by asking who the two *a woman*s were. **A line that has just been edited has to be read as prose, not only re-searched for the token that was removed.**
