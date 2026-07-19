![Horrible Writer banner](assets/horrible-writer-banner.png)

# Horrible Writer

Feed it dull, complicated science, and it will turn it into something weirdly fun.

Scientific writing often has a good reason for being dense: it is carrying methods, caveats, definitions, results, and careful claims all at once. Horrible Writer does not solve that problem by cutting the hard parts away. It keeps the science intact and makes the explanation better, so a reader can follow the same ideas with less friction.

The central question is simple. Can structured text become easier to read without losing its structure, technical depth, or original meaning?

## Inspiration

Horrible Writer is inspired by the *Horrible Science* book series written by Nick Arnold and Phil Gates and illustrated by Tony de Saulles. The series was designed to get children interested in science by focusing on the trivial, unusual, gory, or unpleasant parts of scientific topics, which is exactly the spirit this skill borrows: make science feel alive without making it less scientific.

Learn more: [Horrible Science on Wikipedia](https://en.wikipedia.org/wiki/Horrible_Science).

## What It Does

Horrible Writer rewrites scientific, academic, technical, historical, medical, and research text so it feels clearer, more intuitive, and more engaging. It preserves every section, important detail, and the original order of ideas, then adds short explanations, context, transitions, and plain-language clarifications.

Think of it as a careful editor for complicated research prose. It does not turn a paper into a slogan or a summary. It guides the reader through the same material with better signposts.

## What It Preserves

The skill is built around completeness. It keeps the exact input envelope, whether the source is a LaTeX fragment or a complete document. It preserves headings, lists, comments, labels, citations, equations, tables, figures, block markers, methods, results, and limitations. It also keeps technical terms such as embeddings, hypernetworks, LoRA, regression models, experimental conditions, measures, parameters, datasets, and limitations.

When a concept is difficult, Horrible Writer explains it instead of deleting it. That means Methods and Experiments sections stay technically meaningful, while becoming easier to follow.

## How It Improves the Writing

Horrible Writer explains technical terms in plain language, uses comparisons only when they help, and adds micro-explanations where a reader might otherwise pause. Humor stays dry and source-supported. It does not invent facts, force jokes, or turn serious subjects into comedy.

## Educational figures

Figures are optional. The skill adds one only when it materially improves understanding of a mechanism, process, sequence, anatomy, comparison, workflow, spatial arrangement, or cause-and-effect relation.

It skips decorative figures and does not use a fixed figure count. Every new figure uses a real LaTeX `figure` environment and a detailed multiline `% IMAGE GENERATION PROMPT` comment. Prompts specify the subject, composition, visual teaching purpose, labels or arrows, style, accessibility, factual limits, and ethical limits.

Reusable guidance is included in these files

- `horrible-writer/references/latex-rules.md`
- `horrible-writer/references/image-prompt-templates.md`
- `horrible-writer/references/examples.md`

The style stays grounded. The goal is not comedy, hype, or oversimplification. The goal is a friendly, readable version of the same science, with better flow and fewer unanswered questions.

## Using the Skill

Invoke the skill as:

```text
Use $horrible-writer to rewrite this scientific text so it is clearer, more engaging, and still complete.
```

Then provide the structured text you want rewritten. The skill returns only the converted LaTeX and keeps the source envelope unchanged.

## Repository Contents

- `horrible-writer/SKILL.md`: the agent-facing skill instructions.
- `horrible-writer/agents/openai.yaml`: UI metadata for Codex skill listings.
- `horrible-writer/references/`: LaTeX rules, figure templates, and calibration examples.

## Design Principle

Clarity over cleverness. Completeness over brevity. Flow over punchiness.

The reader should finish the text with fewer questions, not fewer ideas.
