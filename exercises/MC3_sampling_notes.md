# MC3: Sampling notes (stale branch behind main)

**Solo exercise**, with the **facilitator** driving `main`.

Your branch was created a while ago. Since then `main` has moved on — someone
else has already edited the same line you now want to change. When you bring
`main` in, Git finds the conflict.

---

## Sampling notes

Preferred sampling time: _____

---

## Instructions

The target line is `Preferred sampling time:`.

**Exact order of events. Do not skip ahead.**

1. **Facilitator first:** on your own branch, fill in the line — for example
   `Preferred sampling time: early morning, before 9am`. Stage, commit, push,
   open a PR, and merge it with **Squash and merge**.
   **`main` has now moved on.**
2. **You:** your branch was created before that merge, so it is now *behind*
   `main`. On your branch, fill in the same line with your own answer — for
   example `Preferred sampling time: late afternoon, after 3pm`. Stage, commit,
   push. **Do not open a PR yet.**
3. **You:** bring `main` into your branch — Command Palette → `Git: Fetch`,
   then `Git: Merge Branch` → `origin/main`.
   **This is where the conflict appears.**
4. **You:** resolve the conflict in VS Code. Choose current (yours), incoming
   (the facilitator's), both, or rewrite. Stage, commit
   (*"Resolve conflict in MC3"*), push.
5. **You:** open your PR, confirm it is mergeable, **Squash and merge**.

> **The point of this one:** the conflict did not happen at PR time. It happened
> while bringing `main` into your branch. Syncing regularly — Session 2,
> Exercise B — keeps these conflicts small.
