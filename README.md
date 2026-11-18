# unreasonable-outbound-skills

Claude skills for outbound sales. The first one is **driver-tree**.

## driver-tree

Before you reach out to an account, it builds a **value driver tree**:
- the goal the account's leadership is committed to;
- how that goal gets produced, link by link, down to the operational metrics your product can move;
- which role owns those metrics, so you know who to contact;
- a point of view and cold questions that could start a real conversation.

It adapts Nate Nasralla's value driver tree ("Driver Graph"), a tool for live enterprise deals, to outbound, where you have only public information and no champion yet. Read Nate's original: [Value driver trees in sales](https://www.natenasralla.com/resources/value-driver-tree-sales).

### What you get
For each account, one markdown note with:
- the story in one line, the role to contact first, and whether your starting context held up;
- the priorities leadership has committed to, weighed by weight, size and fit with what you sell, and the reason one was chosen;
- the tree as a Mermaid diagram: outcome → engines → key drivers → behaviors, with pressure and owned nodes marked;
- a point of view about *their* business, cold questions, and (Deep mode) discovery questions;
- why the path from the owned behavior to the outcome holds, with the mechanism for each link;
- a private *Where we fit* section, which compares you against what they already have and suggests an angle of attack;
- alternative paths, an evidence table with a source for every figure, and a review section with the claims that were re-checked.

### How a run goes
1. **Gather** public evidence, steered by your seller profile and any context you add.
2. **Weigh the priorities,** choose the outcome, and sketch the engines.
3. **Checkpoint:** Claude writes a short brief with a Mermaid sketch and the sources so far, and asks if it's on the right track. With no reply within 30 minutes, it continues unattended. Say "no checkpoint" to skip it.
4. **Build the tree:** the 3–5 key drivers of each engine on the path, one metric per node, including the ones you can't move. Each driver gets a specific behavior.
5. **Where we fit, alternatives, POV and questions.**
6. **Review:** Claude re-checks the claims the argument rests on against their sources, then runs the checklist.

### Modes
- **Quick**: one path, a ~5-minute read, for volume.
- **Deep** (default): the full tree for tier 1 accounts.
- **Practice**: you draft the tree first, then Claude builds its own and compares, to build your intuition.

### Install
Clone this repo and link (or copy) it into `~/.claude/skills/driver-tree/`.

On first use, Claude asks about 10 questions about what you sell and saves the answers in `profile.md`. The profile is required: it is what points the research at what you can actually move. Your feedback on trees goes in `calibration.md` and overrides the defaults. Both files are git-ignored, and so are the trees themselves (`runs/`).

### Use
- "driver tree for [company]"
- "driver tree for [company] - context: [what you know or suspect]". The context is optional, but it improves the tree a lot.
- "quick tree on [company], for [role]"
- "practice tree on [company]"
- "set up driver-tree"

### How it got here
The commit history shows each version, and why it changed. The tags are `v0.1` to `v0.5`. Two experiments are in the history too, each added and then removed:
- **A profile-free variant,** dropped because without the seller's profile the research drifts to things the seller can't act on.
- **A multi-tree variant** that built several candidate trees in parallel. It was dropped for a single pass with one checkpoint after the outcome and engines.

## Credit
Method: Nate Nasralla. This skill's wording and the outbound adaptation are our own.

## License
[MIT](LICENSE)
