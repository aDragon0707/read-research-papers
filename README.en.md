# Read Research Papers

[中文](./README.md) | [English](./README.en.md)

`read-research-papers` is a Codex skill based on S. Keshav's three-pass method. It divides paper reading into three progressively deeper stages.

Its central principle is not to read every paper linearly from beginning to end. Instead: **build a global map first, inspect the argument and evidence next, and reconstruct the work only when deeper reading is justified.**

> This skill is a reading-depth framework. By itself, it is not a systematic-review protocol, an experimental-reproduction framework, or proof that a learner has mastered a paper.

## Scope

Use this skill when the task is to:

- screen or triage a research paper;
- understand, review, or critique a paper at progressively greater depth;
- reconstruct a paper's argument, method, system, or experimental reasoning;
- perform exploratory citation chaining in an unfamiliar field.

A single-number lookup, citation extraction, translation, or proofreading task usually does not require the full three-pass workflow.

## The Three Passes

| Pass | Typical time | Goal | Main output |
|---|---:|---|---|
| First | 5–10 minutes | Obtain a bird's-eye view | The five Cs and a continue/stop decision |
| Second | Up to 1 hour | Understand the main thrust and supporting evidence | Key points, evidence, comments, and background references |
| Third | About 4–5 hours for a beginner | Reconstruct the work and challenge key assumptions | Reconstructed structure, strengths, weaknesses, assumptions, and future work |

Stop after any pass when the completed depth is sufficient for the reading purpose.

### First Pass — Map the paper

Read:

1. the title, abstract, and introduction;
2. section and subsection headings;
3. the conclusion;
4. the reference list.

Then answer the five Cs:

1. **Category** — What type of paper is this?
2. **Context** — What related work and theoretical basis does it use?
3. **Correctness** — At this preliminary depth, do its assumptions appear reasonable?
4. **Contributions** — What does the paper claim as its main contribution?
5. **Clarity** — Is the paper clearly written?

The first pass supports screening. It forms only a preliminary plausibility judgment and does not independently verify the paper's claims.

### Second Pass — Follow the argument and evidence

Read more carefully while temporarily setting aside details such as complete proofs. Inspect:

- figures, tables, diagrams, and other illustrations;
- graph axes, units, and error bars;
- experiments or analyses supporting the main conclusions;
- background references worth reading next.

The pass is complete when you can explain the paper's main thrust and the evidence the authors use to support it.

If the paper remains unclear, identify the cause: unfamiliar terminology, an unfamiliar proof or experimental technique, poor writing, unsupported assertions, excessive forward references, or reader fatigue. Then pause, repair the missing background, or continue to the third pass.

### Third Pass — Reconstruct the work

Read by virtually re-implementing the paper:

1. temporarily adopt the authors' assumptions and recreate the work;
2. compare your reconstruction with the paper;
3. identify innovations, hidden failures, and implicit assumptions;
4. consider how you would present or implement the ideas independently;
5. record possible future work.

The pass is complete when the paper's overall structure can be reconstructed and its strengths, weaknesses, assumptions, missing citations, and possible technical problems can be identified.

For an AI agent, a fluent reconstruction report proves only that the paper was analyzed. It does not automatically prove human closed-book recall, implementation, experimental replication, or mastery.

## Exploratory Literature Survey

The method also supports citation-chain exploration:

1. Find three to five recent seed papers and, when available, a recent survey.
2. Identify shared citations, repeated researchers, and candidate key papers.
3. Inspect recent proceedings from the field's main conferences.
4. Apply additional passes and add repeatedly cited work that is still missing.

This produces an exploratory literature set, not a systematic review. A systematic review additionally requires explicit databases, search strings, inclusion and exclusion criteria, deduplication, and coverage reporting.

## Report Contract

The skill reports only material supported by the passes actually completed:

- the completed pass and the reason for stopping or continuing;
- the five Cs after the first pass;
- the main thrust, supporting evidence, and relevant background references after the second pass;
- reconstructed structure, strengths, weaknesses, assumptions, technique issues, missing citations, and future-work ideas after the third pass;
- seed papers, shared citations, repeated researchers, conferences, proceedings, and iteration changes for a literature survey.

## Example Requests

```text
Use the three-pass method to screen this paper. Stop after the first pass and tell me whether it is worth continuing.
```

```text
Apply the first and second passes, then explain the paper's main claim and the evidence supporting it.
```

```text
Read this paper to third-pass depth and clearly separate conceptual reconstruction, implementation, and experimental results that were not reproduced.
```

```text
Use citation chaining to survey this research direction and record which key papers were added in each iteration.
```

## Installation

Place `SKILL.md` in the Codex skills directory:

```text
~/.codex/skills/read-research-papers/SKILL.md
```

Repository layout:

```text
read-research-papers/
├── README.md       # Chinese documentation
├── README.en.md    # English documentation
└── SKILL.md        # Complete Codex runtime instructions
```

Reload or restart Codex if the newly installed skill is not detected immediately.

## Method Boundaries

This version intentionally preserves the compact structure of Keshav's original method. It is useful for mapping papers and selecting reading depth, but it does not include:

- discipline-specific evidence audits;
- tensor-shape, masking, training-configuration, or reproduction checks for machine-learning papers;
- a complete search and inclusion protocol for systematic reviews;
- learner-mastery validation through closed-book generation, transfer tasks, or delayed recall.

These boundaries do not make the three-pass method ineffective. They distinguish reading a paper from proving that the paper has been learned or reproduced.

## Original Source

This skill is based on S. Keshav, *How to Read a Paper*, ACM SIGCOMM Computer Communication Review, 37(3), 2007:

- [DOI: 10.1145/1273445.1273458](https://doi.org/10.1145/1273445.1273458)
- [Author-hosted PDF](https://web.stanford.edu/class/ee384m/Handouts/HowtoReadPaper.pdf)

This repository provides an operational adaptation for Codex and does not claim authorship of Keshav's original method.