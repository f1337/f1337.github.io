# Architectural Decision Records (ADRs)

> An architectural decision record (ADR) is a document that--captures an important architectural decision made along with its context and consequences. – [joelparkerhenderson/architecture_decision_record](https://github.com/joelparkerhenderson/architecture_decision_record)

They don’t have to be complicated. The most important thing™ is recording the decision and who made it. The next most important thing is to capture something to help us remember the reason(s) for making the decision. Resist the temptation to let perfect be the enemy of good: shorthand notes which jog the memory of the decision-makers are better than nothing.

## When should we use ADRs?

We will publish an ADR any time we make a technical or architectural decision which meets any of the following criteria:

- it introduces consequences or side-effects
- it is difficult or time-consuming to reverse
- we don’t want it reversed without due consideration (for whatever reason)
- we want to remember why we made the decision
- because we feel like it is important to document

## Create your first ADR

1. [Install adr-tools](https://github.com/npryce/adr-tools/blob/master/INSTALL.md).
2. `adr new summarize the decision`
3. Edit the file created by the above command, commit it to a branch, and submit a PR.

## Example ADR templates

- [Michael Nygard’s simple ADR template](https://github.com/joelparkerhenderson/architecture_decision_record/blob/master/adr_template_by_michael_nygard.md). Widely-used, easy, short.
- [A simple ADR template for the Alexandrian pattern](https://github.com/joelparkerhenderson/architecture_decision_record/blob/master/adr_template_for_alexandrian_pattern.md). Also short and easy, but more structured than Nygard’s.
- [MADR format template](https://github.com/joelparkerhenderson/architecture_decision_record/blob/master/adr_template_madr.md). Medium-length, structured, with thorough prompts for alternatives & other considerations.

## See also

- https://engineering.atspotify.com/2020/04/14/when-should-i-write-an-architecture-decision-record/
- https://adr.github.io/
- https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions
