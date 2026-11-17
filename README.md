# driver-tree

A Claude skill that builds a **value driver tree** for a target account before you reach out: how the company makes money, where the pressure is landing, which role owns the part you can help with, and what point of view and opening questions would start a real conversation.

It adapts Nate Nasralla's value driver tree ("Driver Graph"), a tool for live enterprise deals, to **outbound**. Read Nate's original: [Value driver trees in sales](https://www.natenasralla.com/resources/value-driver-tree-sales).

## What you get
For each account, one markdown note with:
- the story in one line and the role to contact first;
- the tree as a Mermaid diagram (outcome → engines → drivers → behaviors, with pressure and owned nodes marked);
- why the path from that role to the outcome holds, link by link;
- a point of view about *their* business and 2–4 opening questions;
- a private *Where we fit* map, alternative paths, unknowns turned into discovery questions, and an evidence table with a source for every figure.

## Modes
- **Quick**: one branch, ~5-minute read, for volume.
- **Deep**: the full tree for tier 1 accounts.
- **Practice**: you draft the tree first; Claude builds its own and compares, to build your intuition.

## Install
Copy (or link) this folder into `~/.claude/skills/driver-tree/`. On first use, Claude asks ~10 questions about what you sell and saves the answers in `profile.md` (git-ignored). Your feedback on trees goes in `calibration.md` (git-ignored) and overrides the defaults.

## Use
- "driver tree for [company]"
- "quick tree on [company], for [role]"
- "practice tree on [company]"
- "set up driver-tree"

## Credit
Method: Nate Nasralla. This skill's wording and the outbound adaptation are our own.
