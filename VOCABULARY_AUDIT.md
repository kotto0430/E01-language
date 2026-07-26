# English0.1 Vocabulary Audit

This file records communication failures, unofficial words used in examples, and possible repairs.

The purpose is not to hide mistakes. Every missing word is useful evidence for the 256-word selection process.

## Vocabulary Status Labels

- `OFFICIAL` — included in the current 128 words
- `CANDIDATE` — being considered for the 256-word version
- `OPEN` — ordinary English word used temporarily in Open E01
- `REPLACE` — can be expressed clearly with current official words
- `REVIEW` — unclear whether the word deserves an official slot

## Rule for Example Files

Every E01 example should be understood as one of these:

1. **Strict E01** — official vocabulary and numbers only
2. **Open E01** — official vocabulary plus clearly necessary ordinary English words
3. **Normal English meaning** — translation only; not E01 vocabulary

A sentence must not be presented as Strict E01 when it contains unofficial words.

## Missing Words Found in Existing Examples

| Word | Where it appeared | Current judgment | Possible strict repair |
|---|---|---|---|
| me | follow me, help me | CANDIDATE | team follow / help here, but meaning becomes weaker |
| you | you ok? | CANDIDATE | friend ok? / team ok? |
| we | we win, we lose | CANDIDATE | team win / team lose |
| door | open door | CANDIDATE | open house, but not equivalent |
| split | team split | CANDIDATE | team no all / team move different, unclear |
| fight | no fight now | REPLACE | no attack now |
| cave | danger cave | CANDIDATE | no strong replacement |
| path | path clear | CANDIDATE | way is unavailable; map clear is different |
| full | bag full | CANDIDATE | bag no take / bag have many item, awkward |
| rare | rare item | REVIEW | great item does not preserve rarity |
| wood | need wood | CANDIDATE | no useful strict replacement |
| stone | need stone | CANDIDATE | no useful strict replacement |
| very | very good | REPLACE | good good |
| play | play later? | REVIEW | game later? may work in context |
| place | danger place | CANDIDATE | danger here / danger there only works with known location |
| where | quest where? | CANDIDATE | quest here? / there? / north?, inefficient |
| then | then go south | REPLACE | no west / south go |
| apple | old man give apple | OPEN | old man give food |
| happy | man very happy | REVIEW | man good is not equivalent |
| life | life good | REVIEW | game good or world good changes meaning |
| locked | door locked | CANDIDATE | close does not mean locked |
| key | need key | CANDIDATE | no useful strict replacement |
| floor | boss second floor | CANDIDATE | boss up may be enough sometimes |
| second | second floor | OPEN / number rule review | use `2 floor` after `floor` is accepted |

## Early High-Value Findings

The current audit strongly supports several additions because the meanings are frequent and difficult to reconstruct:

```text
I
you
we
this
that
where
inside
outside
behind
through
jump
crouch
shoot
reload
revive
wall
door
floor
stairs
ladder
stone
wood
key
place
dig
repair
empty
broken
locked
fire
room
cave
road
more
enough
```

This is not the official shortlist. It is only evidence gathered from actual communication failures.

## Important Design Lesson

A missing noun is not automatically important.

For example:

```text
apple
```

can often be replaced by:

```text
food
```

But:

```text
key
locked
door
```

represent different and highly reusable concepts. Replacing them destroys important game information.

The selection process should therefore prefer words that preserve distinctions players repeatedly need.

## Repair Log

### README audit — completed

The README was revised so that its main examples use only official vocabulary. The following repairs were made:

```text
we win       -> team win
life good    -> game good
10 apple     -> 10 food
old man give apple -> old man give food
man very happy     -> game good good
```

README now explains Strict E01 and Open E01 before presenting the vocabulary.

### EXAMPLES audit — pending full classification

The examples file intentionally contains many useful Open E01 sentences. The next revision will label sections or individual examples clearly and remove any implication that unofficial words belong to the current 128.

## Audit Workflow

1. Extract every word from Strict E01 examples.
2. Compare the words with the official vocabulary list.
3. Move every unknown word to Open E01 or repair the sentence.
4. Record repeated missing words as 256-word candidates.
5. Test whether a candidate solves several failures.
6. Score and rank the normalized candidate pool.

## Current Status

- [x] Identify the Strict/Open distinction
- [x] Repair README contradictions
- [x] Record major missing words from EXAMPLES
- [ ] Classify every EXAMPLES section
- [ ] Normalize all candidate words
- [ ] Remove duplicate candidates
- [ ] Score candidates
- [ ] Produce provisional additions 129–256
