# Read Research Papers

`read-research-papers` is a Codex skill that applies S. Keshav's three-pass method to research papers and exploratory literature surveys.

这是一个面向 Codex 的论文阅读 skill：先建立全局地图，再检查论证与证据，最后在确有必要时进行深度重建。它保留 Keshav 原始方法的紧凑结构，不把每篇论文都强制读到同一深度。

## Scope

Use this skill when the task is to:

- screen or triage a research paper;
- understand and review a paper at progressively greater depth;
- reconstruct a paper's argument, method, or system;
- perform exploratory citation chaining in an unfamiliar field.

This is a reading-depth framework. It is **not**, by itself, a systematic-review protocol, an experimental-reproduction framework, or proof that a learner has mastered the paper.

## The Three Passes

| Pass | Typical time | Goal | Main output |
|---|---:|---|---|
| First | 5–10 minutes | Obtain a bird's-eye view | The five Cs and a continue/stop decision |
| Second | Up to 1 hour | Understand the main thrust and supporting evidence | Key points, evidence, comments, and background references |
| Third | About 4–5 hours for a beginner | Reconstruct the work and challenge its assumptions | Reconstructed structure, strengths, weaknesses, assumptions, and future-work ideas |

Stop after any pass when that depth is sufficient for the reading purpose.

### First Pass — Map the paper

Read the title, abstract, introduction, section headings, conclusion, and references. Then report the five Cs:

1. **Category** — What type of paper is this?
2. **Context** — What prior work and theoretical basis does it use?
3. **Correctness** — Do its assumptions appear valid at this preliminary depth?
4. **Contributions** — What does the paper claim as its main contribution?
5. **Clarity** — Is the paper clearly written?

The first pass supports screening; it does not establish that the paper's claims are verified.

### Second Pass — Follow the evidence

Read more carefully while temporarily setting aside details such as full proofs. Inspect figures, diagrams, graph axes, error bars, and relevant references. The goal is to explain the paper's main thrust and the evidence used to support it.

If the paper remains unclear, identify why: missing terminology, unfamiliar proof or experimental technique, poor writing, unsupported assertions, excessive forward references, or reader fatigue. Then stop, repair the missing background, or continue to the third pass.

### Third Pass — Reconstruct the work

Virtually re-implement the paper: adopt the authors' assumptions, recreate the reasoning or system, compare the reconstruction with the paper, challenge important assumptions, and record weaknesses and future-work ideas.

For an AI system, a generated reconstruction is analysis evidence—not proof of a human reader's memory, implementation, replication, or mastery.

## Exploratory Literature Survey

The skill also supports iterative citation chaining:

1. Find three to five recent seed papers and, if available, a recent survey.
2. Identify shared citations, repeated researchers, and candidate key papers.
3. Inspect recent proceedings from the field's main conferences.
4. Make additional passes and add repeatedly cited missing work.

This produces an exploratory survey set. A systematic or scoping review additionally requires an explicit database strategy, search strings, inclusion/exclusion criteria, deduplication, and coverage reporting.

## Report Contract

The skill reports only what the completed passes support:

- completed pass and the reason for stopping or continuing;
- five Cs after the first pass;
- main thrust, supporting evidence, and relevant background references after the second pass;
- reconstructed structure, strengths, weaknesses, assumptions, technique issues, missing citations, and future-work ideas after the third pass;
- seed papers, shared citations, repeated researchers, conferences, proceedings, and iteration changes for a literature survey.

## Example Requests

```text
Use the three-pass method to screen this paper. Stop after the first pass.
```

```text
Apply the first and second passes, then explain the paper's main claim and supporting evidence.
```

```text
Read this paper to third-pass depth and clearly separate conceptual reconstruction from anything not implemented or reproduced.
```

```text
用三遍阅读法带我读这篇论文。先完成第一遍，并告诉我是否值得继续。
```

## Installation

Place the skill file at:

```text
~/.codex/skills/read-research-papers/SKILL.md
```

Repository layout:

```text
read-research-papers/
├── README.md    # Documentation; not part of the runtime instructions
└── SKILL.md     # Complete Codex skill
```

Restart or reload Codex if the newly installed skill is not detected immediately.

## Source

This skill is based on S. Keshav, *How to Read a Paper*, ACM SIGCOMM Computer Communication Review, 37(3), 2007:

- [DOI: 10.1145/1273445.1273458](https://doi.org/10.1145/1273445.1273458)
- [Author-hosted PDF](https://web.stanford.edu/class/ee384m/Handouts/HowtoReadPaper.pdf)

The repository documents an operational adaptation for Codex; it does not claim authorship of Keshav's original method.