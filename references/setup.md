# Setup

Run on first use (no `profile.md`) or when the user says "set up driver-tree". Ask a few questions at a time, in plain language. Links to the website, a pitch deck, case studies or a battlecard are welcome: read them and draft the answer yourself, then confirm. Anything the user skips is `unknown`; never fill it in.

## Questions
1. **What do you sell?** One paragraph, as you'd say it to a customer. Website link?
2. **What does it actually do?** The 3–6 concrete capabilities (not benefits). Where is it deployed or used?
3. **What does it change for a customer?** For each capability, which work or metric changes, for whom. Think in behaviors ("support engineers answer fewer repeat questions") and drivers ("ticket volume", "time to first design-in").
4. **Proof.** Customer results you can stand behind: customer (or anonymised), metric, before → after. Which ones may be named in conversation?
5. **Who buys?** Industries, company size, regions, and the tiers you use for accounts.
6. **Who do you talk to?** The roles you usually contact, who tends to become the champion, and who signs. What each is graded on, if you know.
7. **Signals.** What makes an account a priority right now (hiring for X, launching Y, a public complaint about Z)?
8. **Alternatives.** Competitors, building in-house, and the "do nothing" the buyer usually picks. Where you win and lose.
9. **Where you're weak.** Accounts or situations where you're a poor fit. (The tree should say so when it sees one.)
10. **Output.** Folder to save trees in (default: `./driver-trees/` in the current directory), and language.

## Profile template
Write `profile.md` in the skill folder:

```markdown
# Seller profile
*Updated YYYY-MM-DD. Edit freely; the skill reads this before every run.*

## What we sell
[one paragraph]

## Capabilities
- [capability]: [what it does, concretely]

## What it changes (capability → behavior → driver)
- [capability] → [behavior at the customer] → [driver it moves]

## Proof
| Customer | Metric | Before → after | Nameable? |
| --- | --- | --- | --- |

## Ideal customers and tiers
[industries, size, regions; how tiers are defined]

## Roles
| Role | Usually | What they're graded on |
| --- | --- | --- |
| [title] | contact / champion / signer | [metric] |

## Signals that make an account a priority now
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
