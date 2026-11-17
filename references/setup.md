# Setup

Run on first use (no `profile.md`) or when the user says "set up driver-tree". Ask a few questions at a time, in plain language. Links to the website, product docs, a pitch deck, case studies, comparison pages or a battlecard are welcome: read them, draft the answer yourself, then confirm. Anything the user skips is `unknown`; never fill it in.

**Encourage rich answers.** The profile is what points every tree at what this seller can move. A thin or outdated profile gives a tree full of things the seller can't act on.

## Questions
1. **What do you sell?** One paragraph, as you'd say it to a customer. Website and product-docs links. What is established, and what is new or not yet proven?
2. **What does it actually do?** How the product is built (the core, and what sits on top of it), its concrete capabilities (not benefits), and where each one is deployed or used.
3. **What does it change, for which segment and role?** Value usually depends on the industry and the role. For each segment you sell to: which roles' work changes (behaviors, e.g. "support engineers answer fewer repeat questions") and which metrics move (drivers, e.g. "ticket volume", "time to first design-in"). Which business metrics are easy to tie your product to, and which are relevant but hard to tie to it?
4. **Proof.** What can you say about customers? Usually there are two rules, one for naming customers and one for quoting metrics. Which customer results are published (customer, metric, before → after)? Which numbers are internal only?
5. **Who buys?** What makes a company a true ICP (the conditions that must all hold)? Size floors, segments, regions, and the tiers you use, if any.
6. **Who do you talk to?** Per segment: the roles you contact first, who tends to become the champion, and who signs. What each is graded on, if you know.
7. **Signals.** What makes an account a priority right now? Separate the **big changes in the business or industry** that make the account a priority (a strategic expansion, joining an ecosystem, a competitor's move) from the **smaller signals** that point to the person (a hire, a relaunch, a complaint).
8. **Alternatives.** Competitors (per segment if they differ), building in-house, and the "do nothing" buyers usually pick. Where you win and lose against each, and why. A comparison page or battlecard helps.
9. **Where you're weak.** Accounts or situations where you're a poor fit. (The tree should say so when it sees one.)
10. **Output.** Folder to save trees in (default: `./driver-trees/` in the current directory), and language.

## Profile template
Write `profile.md` in the skill folder:

```markdown
# Seller profile
*Updated YYYY-MM-DD. Edit freely; the skill reads this before every run.*

## What we sell
[one paragraph]
**Emerging, not yet proven:** [what's new; use it to spark interest, never as proof]
Website: [link]. Product docs (source of truth): [link]

## The product
[the core, and what sits on top of it]

### Deployment channels
- [channel]: [what it does, where]

## What it changes (by segment and role)
### [Segment]
| Role | Behavior that changes | Driver |
| --- | --- | --- |
| [role] | [behavior] | [metric] |

## Business metrics we sell against
- **Easier to tie the product to:** ...
- **Relevant but harder to tie to it:** ...

## Proof
**Customer names:** [the rule]
**Metrics:** [the rule]
| Customer | Segment | Deployment | Published result |
| --- | --- | --- | --- |

## Ideal customers and tiers
**True ICP:** [the conditions that must all hold]
**Size floor:** ...
**Segments, regions, tiers:** ...

## Roles
**Buyer and signer:** [who, and how to tell]
### [Segment]
| Role | Usually | Notes |
| --- | --- | --- |
| [title] | contact / champion / signer | [what they're graded on] |

## Signals that make an account a priority now
**Big changes (make the account a priority):**
- ...
**Smaller signals (pick the person):**
- ...

## Alternatives
| Alternative | Where we win | Where we lose |
| --- | --- | --- |
| Build in-house | | |
| Do nothing | | |

## Poor fit
- ...

## Output
- Folder: [path]
- Language: [language]
```
