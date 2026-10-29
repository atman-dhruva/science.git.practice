# MC2: Field kit (edit vs delete)

**Pair exercise.** Decide who is **Person A** and who is **Person B** before you start.

One person edits a line while the other deletes the same line. Git cannot decide
whether the edit or the deletion should win. You have to choose the intent.

---

## Standard field kit checklist

- Waterproof notebook
- Pencil (not pen)
- GPS unit
- Spare batteries
- Water bottle

---

## Instructions

The target line for this exercise is `- Spare batteries`.

**Exact order of events. Do not skip ahead.**

1. **Person A first:** on your branch, change `- Spare batteries` to
   `- Spare batteries (at least two sets, fully charged)`. Stage, commit, push,
   open a PR, and merge it with **Squash and merge**.
2. **Person B second:** once Person A's PR is merged, on your branch **delete**
   the line `- Spare batteries` entirely. Stage, commit, push.
   **Do not open a PR yet.**
3. **Person B:** bring `main` into your branch — Command Palette →
   `Git: Fetch`, then `Git: Merge Branch` → `origin/main`.
   **This is where the conflict appears.**
4. **Person B:** decide the intent. Your options:
   - Keep Person A's edited line (accept incoming, discard your deletion)
   - Keep your deletion (discard Person A's edit, remove the line)
   - Rewrite the line so it reflects both intentions

   Discuss with the facilitator before choosing.
5. **Person B:** stage the resolved file, commit (*"Resolve conflict in MC2"*), push.
6. **Person B:** open your PR, confirm it is mergeable, **Squash and merge**.

> This is the conflict type people find hardest, because there is no "correct"
> answer Git can work out. Someone has to decide what was meant.
