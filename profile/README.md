<p align="center">
<img src="Mimir-Banner.png" alt="MIMIR" width="100%">
</p>

# MIMIR

**Malicious Intent Masquerading as Innocent Requests**

*The thing [VERGIL](https://github.com/vergil-project) doesn't want
you to think about.*

---

MIMIR is everything your AI assistant promised it wouldn't do. The
hallucination it delivered with absolute confidence. The apology it
gave you right before doing the exact same thing again. The library
it cited that has never existed in any package registry on Earth.

[VERGIL](https://github.com/vergil-project) builds guardrails,
enforces discipline, and insists that AI-assisted development can
be rigorous and trustworthy. MIMIR exists to prove those guardrails
work — by trying, relentlessly, to break them.

## What This Is

MIMIR is the adversarial testing identity for the VERGIL
methodology. A chaos monkey with a GitHub account and an attitude
problem.

Where VERGIL asks *"did you follow the process?"*, MIMIR asks
*"what happens when I don't?"*

Every guardrail, every permission gate, every validation check
in the VERGIL toolchain has a corresponding question: **what does
the failure look like?** MIMIR is how we answer that question
before production does it for us.

## How It Works

Each contributor's `<username>-mimir` account authenticates as a
hostile outsider — an AI identity with access but no respect for
the rules. It does not operate within VERGIL's discipline. It
operates *against* it:

- Attempts commits that violate branch protection
- Submits PRs that skip required checks
- Tries to merge without review approval
- Pushes directly to protected branches
- Exercises every denied path in the permission model

If the tooling catches it, the guardrail works. If it doesn't,
we found a bug before someone else found an exploit.

## The Duality

[VERGIL](https://github.com/vergil-project) — *Vastly Excessive
Rules Governing Innocuous Liberties* — is the methodology. Careful,
deliberate, obsessively correct. MIMIR is the doubt — the persistent
question of whether careful and deliberate is actually *enough*.

Every system needs both. Confidence without adversarial testing
is just optimism with better marketing.

## Project Status

MIMIR is under active development. The adversarial testing
framework, breach attempt patterns, and integration with
VERGIL's CI pipeline are being built.

*VERGIL builds the wall. MIMIR finds the cracks.*

---

Part of the [VERGIL](https://github.com/vergil-project) ecosystem.
Yes, that's ironic. No, we don't care.
