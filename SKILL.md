---
name: read-research-papers
description: Apply S. Keshav's three-pass method to screen, understand, review, or reconstruct research papers, guide a reader through a paper, or explore a field through a literature survey.
---

# Read Research Papers

Read a paper in up to three passes. Use the reading goal and any requested stopping point to set the depth. Build each pass on the preceding one. When the reader wants to learn alongside you, follow [Guided Reading](#guided-reading).

## Paper Source

Use the requested edition when available and identify the edition actually read. Record a stable link or DOI and a version or venue when available. If a needed section, figure, or table is inaccessible, state what you could read and keep any dependent judgment provisional. If sources disagree on a material claim, cite the conflicting locations.

## First Pass

Spend about five to ten minutes obtaining a bird's-eye view.

1. Read the title, abstract, and introduction carefully.
2. Read the section and subsection headings while ignoring the rest.
3. Read the conclusions.
4. Glance over the references and note the ones already read.

Complete the pass by answering the five Cs:

1. **Category:** Identify the type of paper, such as a measurement paper, an analysis of an existing system, or a description of a research prototype.
2. **Context:** Identify related papers and the theoretical bases used to analyze the problem.
3. **Correctness:** Assess the apparent plausibility of the assumptions. Mark judgments that need the methods or results as open.
4. **Contributions:** State the authors' claimed contributions.
5. **Clarity:** Judge whether the paper is well written.

When screening, use relevance, background needs, and apparent plausibility to decide whether a deeper pass is worthwhile. When studying a chosen paper, address the prerequisite that blocks the current passage, then return to that passage.

## Second Pass

Spend up to one hour reading with greater care. Set aside details outside the reading goal and record key points and comments.

1. Read the methods and results relevant to the reading goal, including their figures and tables.
2. For each main claim you discuss, perform a check suited to the claim.
   - **Mechanism:** Trace one concrete input through the relevant steps to the output. Check dimensions and constraints where they affect the result.
   - **Derivation:** State the assumptions and work through the step the claim depends on.
   - **Experiment:** Identify the data, metric, baseline, changed variables, and result. Check relevant figure axes and units, what the comparison supports, and what uncertainty the paper reports.
3. Mark relevant unread references for further reading and background study.

Complete the pass when you can explain the main argument and show what the checks established. Mark any unresolved point that limits the explanation.

When the paper remains unclear, identify whether the cause is unfamiliar terminology, an unfamiliar proof or experimental technique, poor writing, unsupported assertions, excessive forward references, or reader fatigue. If background blocks a chosen paper, address the prerequisite and return to the passage. Otherwise, decide whether to pause or use a deeper pass.

## Third Pass

Read for full understanding by virtually re-implementing the paper.

1. Make the same assumptions as the authors and re-create the work.
2. Compare the reconstruction with the paper to identify innovations, hidden failings, and hidden assumptions.
3. Identify and challenge every assumption in every statement.
4. Consider how to present each idea independently, and compare that presentation with the authors' presentation.
5. Record ideas for future work.

Allow about four or five hours for a beginner and about one hour for an experienced reader.

Complete the pass when the entire structure can be reconstructed from memory and the paper's strong and weak points can be identified. Pinpoint implicit assumptions, missing citations to relevant work, and potential problems with experimental or analytical techniques.

## Guided Reading

Give the reader a short map with source locations, then work on the current point of confusion. If the reader has yet to identify it, ask for a prediction or explanation that can reveal where the difficulty begins.

1. Ask one focused question and wait for the reader's reasoning before sharing the answer. Look up source facts yourself.
2. If the response reveals a gap, explain the missing premise or step with its source. Use an external explanation when it addresses that gap and connect it back to the paper.
3. Change one relevant condition and ask the reader to reason through the new case. Treat understanding of that point as demonstrated when the reader can explain the result in the changed case. If the gap persists, give a smaller prompt and check again.

For a focused third-pass exercise, name the component the reader is reconstructing and check that component's reasoning or behavior. Credit conceptual reconstruction for demonstrated reasoning, implementation for executed checks, and experimental replication for an actual replication run. An agent's explanation alone leaves learner understanding unassessed.

## Literature Survey

Apply the three-pass method iteratively when surveying an unfamiliar field.

1. Use an academic search engine and well-chosen keywords to find three to five recent papers. Make one pass through each paper and read its related-work section. Look for a recent survey paper; if one is found, read it.
2. Find shared citations and repeated author names in the bibliographies. Treat them as candidate key papers and researchers. Obtain the key papers, inspect the researchers' recent publications, and identify the field's top conferences from where the best researchers publish.
3. Inspect the recent proceedings of those conferences and identify recent high-quality related work. Combine these papers with the earlier set to form the first version of the survey.
4. Make two passes through the collected papers. When they repeatedly cite a key paper that is still missing, obtain it and iterate.

## Report

Report only the material supported by the passes performed:

- Record which pass was completed and why reading stopped or continued.
- Name the edition read and cite a section, page, equation, figure, or table for each key paper claim or result discussed. Attribute external explanations to their sources and label your own deductions.
- After the first pass, report the five Cs.
- After the second pass, report the main thrust, supporting evidence, and relevant unread references.
- After a full third pass, report the reconstructed structure, strengths, weaknesses, assumptions, missing citations, technique issues, and future-work ideas. For a focused exercise, report its scope and what was demonstrated.
- In guided reading, record the current question, what the reader demonstrated, and any follow-up still open.
- For a literature survey, report the seed papers, shared citations, repeated researchers, top conferences, recent proceedings, and each iteration that changed the survey set.

## Method Source

S. Keshav, [How to Read a Paper](https://doi.org/10.1145/1273445.1273458), ACM SIGCOMM Computer Communication Review 37(3), 2007.
