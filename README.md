# Anti-Defensive Writing

A reusable AI agent skill for revising English academic manuscripts and reviewer responses with clearer, evidence-aligned, non-defensive writing.

It helps authors make their strongest supported contribution easier to understand without turning legitimate uncertainty, methodological limits, or unfavorable results into omissions.

## What It Does

- Removes unnecessary disclaimers, apology-like framing, and repetitive caveats.
- Replaces vague or stacked hedging with calibrated, evidence-appropriate language.
- Clarifies contribution statements, scope, paragraph logic, and argumentative structure.
- Supports manuscript polishing, shortening, abstract revision, narrative restructuring, experiment presentation, and reviewer responses.
- Keeps claims aligned with the available evidence and the requested revision scope.

## When to Use It

Use this skill when the text to revise is in English, even if the request itself is written in another language.

Typical requests include:

- “Polish my paper”
- “Revise this abstract”
- “Shorten this section”
- “Strengthen the paper’s narrative”
- “Improve this rebuttal”
- “润色论文”
- “改摘要”
- “压缩篇幅”
- “调整论文主线”
- “写 rebuttal”
- “回复审稿意见”

The skill also supports drafting new English manuscript or rebuttal text from notes or bullet points written in another language.

## What It Does Not Do

This skill does not handle translation.

Converting an already-written Chinese or other non-English passage into English is a translation task and should be handled separately. In contrast, drafting a new English paragraph, abstract, or rebuttal from Chinese notes remains in scope.

The skill does not invent evidence, results, mechanisms, citations, representativeness claims, or favorable trade-offs to make writing seem stronger.

## Core Approach

The skill distinguishes unnecessary defensive framing from information that readers need to interpret the work correctly.

It removes empty self-limitation, such as repeated statements of what a paper does not claim, while preserving qualifications that affect:

- claim validity;
- interpretation of evidence;
- scope of application;
- research design;
- methodological transparency; or
- correct use of the findings.

For substantive revisions, the skill organizes the manuscript around the most meaningful contribution supported by the evidence. It does not redefine success to conceal an unfavorable result or selectively omit evidence that materially changes the interpretation of a claim.

## Common Revisions

| Defensive framing | Evidence-aligned revision |
| --- | --- |
| “Unfortunately, our method only achieves 82% accuracy.” | “Our method achieves 82% accuracy.” |
| “We do not attempt to examine rural settings.” | “The analysis focuses on urban settings.” |
| “The evidence may possibly suggest an association.” | “The evidence suggests an association.” |

These examples illustrate changes in framing. A revision should retain relevant comparisons, limitations, uncertainty, and scope conditions when they materially affect the claim.

## Installation

Copy the `anti-defensive-writing` directory into your Codex skills directory:

```text
~/.codex/skills/anti-defensive-writing/
└── SKILL.md
```

Restart or reload your agent environment if required.

## Usage

Use the skill explicitly:

```text
$anti-defensive-writing Polish the following introduction while preserving all technical claims and citations.
```

Or ask naturally:

```text
Please revise this abstract to foreground the main contribution without strengthening claims beyond the reported results.
```

```text
Please shorten this discussion section while preserving necessary methodological limitations.
```

```text
根据以下中文要点，起草一份英文 rebuttal，逐条回应审稿意见，并保持证据一致。
```

## Scope

The skill applies to:

- English academic manuscripts;
- English abstracts, introductions, methods, results, discussions, and conclusions;
- English reviewer responses and rebuttals;
- English text drafted from notes or bullet points in any language.

The skill excludes:

- translation of existing non-English prose into English;
- requests to fabricate or overstate findings;
- removal of limitations that are necessary for accurate interpretation.

## Repository Structure

```text
.
├── SKILL.md
├── README.md
└── LICENSE
```

## Acknowledgements

This skill was developed with reference to:

- [Kiterlin/anti-defensive-writing](https://github.com/Kiterlin/anti-defensive-writing)
- [Adkid-Zephyr/anti-defensive-writing-Skill](https://github.com/Adkid-Zephyr/anti-defensive-writing-Skill)

It develops these ideas for long-term academic-paper revision, with explicit rules for English-only revision, translation exclusion, evidence alignment, revision scope, experiment presentation, and reviewer responses.

## License

This project is licensed under the [MIT License](LICENSE).
