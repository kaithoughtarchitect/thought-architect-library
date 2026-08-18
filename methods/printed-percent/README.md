# Is a printed percent a verdict?

**Audience:** a coding agent (or a human using one) looking at a claim that an agent or harness got better by N percent.  
**Status:** portable checklist. Distilled from the hole “the number printed; the verdict did not.”  
**Claim boundary:** this does not prove a system works. It does not name a product. It does not grade a stranger’s post. It asks whether *this* percent is something you are entitled to believe.

A score can print overnight. A verdict you can defend is a different object.

## The hole

People now run loops that propose harness changes, run a number, and keep the winner. That loop is real work. The failure mode is treating the printed delta as proof.

You cannot know from the headline:

- what the baseline was in absolute units
- what scored the run (a unit test, a bench, the same model)
- how many candidates lost
- whether one seed or a distribution
- whether the lift transfers off the bench you optimized

If those are missing, you do not have a verdict. You have a number.

## What you should do

Hand this file to the agent. Point it at the claim (a README, a blog, a PR, a chat log). The agent reports the checklist. It does not invent the missing numbers. It does not dunk on the author.

```text
Claim:
Scorer (external bench / same-model judge / unknown):
Baseline (absolute, not just +N%):
N of tries kept / thrown away:
Variance or seeds:
Transfer / held-out:
What this percent does *not* prove:
Verdict: defendable / printed-only / cannot tell
```

If a cell is unknown, write `unknown`. Do not fill it.

## What not to do

- Do not treat “it kept the winner” as “the winner is true.”
- Do not report a relative percent without the absolute before and after.
- Do not let the same model that proposed the change be the only scorer, then call that independent.
- Do not bash a person for publishing a loop. Argue the hole.
- Do not upgrade `unknown` into a vibe.

## When this is enough

Stop after the checklist if the claim is only a headline. If they want a product that turns this hole into a defendable verdict, that is a different layer. This page is the questions. It is not that product.
