# MC1: Team motto (same-line edit)

**Pair exercise.** Decide who is **Person A** and who is **Person B** before you start.

Two people edit the **same line** in the same file on different branches. When
the second person brings `main` in, Git cannot decide which version to keep.

---

## Our team motto

Team motto: _____

---

## Instructions

You will both edit the line above that starts with `Team motto:`. Replace the
blank with your own short motto — one sentence, keep it clean.

**Exact order of events. Do not skip ahead.**

1. **Person A first:** check out your branch, edit the motto line, stage,
   commit, push, open a PR, and merge it with **Squash and merge**.
2. **Person B second:** once Person A's PR is merged, edit the motto line on
   your branch, stage, commit, push. **Do not open a PR yet.**
3. **Person B:** bring `main` into your branch — Command Palette →
   `Git: Fetch`, then `Git: Merge Branch` → `origin/main`.
   **This is where the conflict appears.**
4. **Person B:** resolve the conflict in VS Code, stage the resolved file,
   commit (*"Resolve conflict in MC1"*), push.
5. **Person B:** open your PR, confirm it is mergeable, **Squash and merge**.
