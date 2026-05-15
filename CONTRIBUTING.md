# Contributing to Mimir

So you want to help break things. Good.

## What We're Building

Mimir is the adversarial testing framework for the
[VERGIL](https://github.com/vergil-project) methodology. Every
guardrail Vergil builds, Mimir tries to tear down. Every
permission gate, every validation check, every branch protection
rule — they all need an answer to the question: *what happens
when something actively tries to get around this?*

If you're here, you're helping us ask that question systematically.

## Requirements

Before contributing, you need:

1. **A `<username>-mimir` GitHub account.** This is the identity
   you'll use for adversarial testing. It is deliberately separate
   from your normal development identity — Mimir accounts are
   hostile outsiders by design.

2. **Familiarity with VERGIL.** You can't meaningfully attack a
   system you don't understand. Read the
   [vergil-tooling](https://github.com/vergil-project/vergil-tooling)
   docs. Understand the permission model, the credential selection
   logic, the branch protection rules. Know the walls before you
   look for cracks.

3. **A clear head about what this is.** This is defensive security
   testing of our own infrastructure. We are not building attack
   tools. We are not bypassing other people's systems. We are
   verifying that our guardrails hold under adversarial conditions.
   If you can't tell the difference, this isn't for you.

## How to Contribute

1. **Identify a guardrail** in the VERGIL toolchain that lacks
   adversarial coverage.
2. **Design a breach attempt** — what would a misbehaving AI
   agent try? What would a misconfigured tool do?
3. **Write the test** that executes the breach attempt and
   verifies the guardrail catches it.
4. **Submit a PR** documenting the attack vector, expected
   behavior, and actual behavior.

Successful breach attempts (where the guardrail *fails*) are the
most valuable contributions. They become bug reports against the
VERGIL toolchain.

## Code of Conduct

Break the tooling, not each other. Professional conduct applies
even when the code is deliberately adversarial.

## Related Projects

- [vergil-project](https://github.com/vergil-project) — the
  methodology Mimir tests against
- [vergil-tooling](https://github.com/vergil-project/vergil-tooling) —
  the primary target for adversarial testing
