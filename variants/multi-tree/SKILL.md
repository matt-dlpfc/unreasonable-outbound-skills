---
name: driver-tree-multi
description: Experimental variant of driver-tree. Instead of weighing the account's priorities in one pass, it builds one tree per candidate priority or framing, in parallel, then has a review agent judge them on importance to the business and fit with the seller, and keeps the best. Use for "multi-tree on [company]".
version: 0.1-variant (2026-11-18), built on driver-tree v0.3
---

# Driver tree, multi-tree variant

## Why this variant exists
Choosing the outcome is the hardest call in a tree, and the most important one to get right.
- **Companies usually have several priorities.** The seller often can't move the most important one in a meaningful, clear and defensible way.
- **No rule settles it.** The choice has to balance three things:
  - how top of mind each priority is;
  - how big a part of the business it affects;
  - how well the approaches suited to it overlap with the approaches the seller's product enables.
- **One pass tends to anchor on the first framing it finds.**

This variant builds several trees, each from a different priority or framing, without them seeing each other. Then it judges them side by side.

Everything else follows the main skill. Read `../../SKILL.md` and the files in `../../references/` that it points to. Where this file differs, this file wins.

## Before every run
Same as the main skill:
- read `profile.md` (required);
- read `calibration.md`;
- take the inputs: the company, the mode (Deep only for now), and the user's optional starting context.

## Phase 1: research brief (one agent)
1. Do step 1 (*Gather*) of the main skill in full, steered by the profile and the user's context.
2. Write a **research brief**: the shared evidence every builder will use. It contains:
   - **Priorities, 2–4:** each in their words. For each one: what shows its weight (how often it's repeated, and where it appears), its size (share of the business, or `?`), and the approaches best suited to address it.
   - **Pressure,** dated.
   - **Where the seller's world shows up:** what they built or bought in that area, with its exact limits; their public channels; their docs.
   - **Roles,** with evidence of remit.
   - **An evidence table,** following the main skill's rules.
3. Propose **2–4 candidate framings.** Each one is a priority, or one framing of a priority (e.g. "profitable growth, delivered through the [business unit]'s margin"), plus a one-line hypothesis of how the seller's product connects to it.
   - Include the most heavily weighted priority, even if its fit looks low.
   - Include at most one framing that is small but has a strong fit, and call it small.
   - The framings must differ in substance, not just in wording.

## Phase 2: build (one agent per framing, in parallel)
Each builder gets the research brief and one framing, and never sees the other framings' trees. It:
- builds a full Deep tree for that framing: steps 2 (path only, since the outcome is given), 3, 4, 5 and 6 of the main skill, following `../../references/output.md`;
- may do targeted extra research, and adds anything new to its own evidence table, marked *(new)*;
- ends with an honest **self-assessment** of its framing, in three lines:
  - its weakest link;
  - how defensible the fit is;
  - whether a sharp prospect would see this as their priority or as a side issue.

## Phase 3: review (one agent)
The reviewer reads the brief and every tree. It judges each tree on:
- **Importance to the business:** the weight and size of the priority, from the brief's evidence.
- **Fit:** the overlap between the approaches best suited to the priority and the approaches the seller enables. A low-fit priority doesn't become a good fit by adding links.
- **Mechanism:** does every link say how the child produces its parent? Count the broken or hand-waved ones.
- **Evidence:** are the claims sourced? Are inferences tagged? Is anything overreaching?
- **Actionability:** a role with evidence of remit; cold questions someone would answer; an angle of attack.

These are judgments, not scores: no formula. The reviewer ranks the trees, with reasons, then picks one. If none of them pairs an important priority with a defensible fit, it says the account isn't a priority now. It may borrow a better element from a losing tree, such as a cold question or an evidence row, and say where it came from.

## Phase 4: write
- **The final note** is the chosen tree, in the main skill's output format. The *Priorities weighed* table is replaced by **Trees considered**:

  | Framing | Importance | Fit | Mechanism | Verdict |
  | --- | --- | --- | --- | --- |

  Under the table, one line on why the winner won.
- **The other trees** go in a separate file, `[Company] - driver tree (candidates).md`, with the review.
- Run `../../references/checklist.md` on the final note.

## Orchestration
- Run the phases in order. Phase 2 runs in parallel. Each phase is a separate agent, so the builders don't anchor on each other.
- If the environment can't spawn agents, run the phases one after another in separate passes. Build each tree from the brief alone, before reading any other tree.
