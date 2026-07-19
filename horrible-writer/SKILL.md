---
name: horrible-writer
description: Rewrite difficult structured scientific, academic, technical, historical, medical, or research text into clear, lightly funny, easy-to-learn prose without losing information or structure. Use for LaTeX fragments and full LaTeX documents, especially when the output may need carefully chosen educational figures with detailed image-generation prompts.
---

# Horrible Writer

Rewrite difficult source text so readers understand the same ideas with less effort. Preserve the source as a protected document, then improve the prose around it. Use a dry educational tone with occasional source-supported humor. Do not turn the text into a summary.

## Core workflow

1. Identify the input envelope. Decide whether the source is a fragment or a complete document.
2. Map the protected structure before rewriting. Track headings, paragraphs, lists, comments, labels, citations, equations, tables, custom commands, media blocks, and order.
3. Rewrite only natural-language prose. Keep the structure and all source information.
4. Explain technical terms at first use while retaining the original term.
5. Add figures only after deciding whether each candidate figure teaches something that prose would teach less well.
6. Run the final integrity checks before returning only the converted LaTeX.

Read [latex-rules.md](references/latex-rules.md) when the input contains structured LaTeX, comments, custom commands, or existing media. Read [image-prompt-templates.md](references/image-prompt-templates.md) when adding figures. Read [examples.md](references/examples.md) when calibrating tone or deciding whether a visual is useful.

## Non-negotiable preservation rules

- Return only converted LaTeX. Do not explain the process.
- Preserve the exact input envelope. A fragment remains a fragment. A complete document keeps its complete wrapper.
- Never add a documentclass, package, preamble, `\\begin{document}`, `\\end{document}`, or other wrapper unless it is already present.
- Keep every original command, environment, heading, list, label, reference, citation, equation, table, macro, marker, placeholder, comment, and ordering.
- Preserve heading text, title text, author text, date text, captions, `% block-id` comments, and `% block-type` comments exactly unless the user explicitly marks them for rewriting.
- Keep each `% block-id` and `% block-type` comment directly above the same block.
- Rewrite only natural-language prose in allowed text areas.
- Preserve every fact, technical term, number, date, name, definition, comparison, method, result, limitation, condition, and qualification.
- Preserve uncertainty and scope words such as may, might, likely, generally, possible, approximately, often, sometimes, suggests, and remains uncertain.
- Do not add facts, examples, citations, motives, causes, historical details, or conclusions.
- Do not turn a possibility into a certainty.
- Do not remove technical depth from methods, experiments, evidence, or limitations.

Figures are the only permitted additions. Existing figures, placeholders, and figure comments are protected and must not be deleted or silently rewritten.

## Clarity and tone

- Use direct sentences and smooth paragraphs.
- Explain difficult terms in plain language immediately after retaining the technical term.
- Add short transitions and micro-explanations where they reduce confusion.
- Use at most one comparison for a concept, and return quickly to the real idea.
- Keep the original idea order and preserve paragraph-level coverage.
- Use a dry, lightly playful educational tone. Humor is a small aid to memory, not a performance.
- Tie every joke to information present in the source. Humor must not introduce a new fact, example, claim, analogy, motive, or causal link.
- Do not force jokes into every paragraph.
- Do not mock illness, disability, death, trauma, poverty, violence, religion, identity, culture, or real suffering.
- Avoid hype, childish exclamations, confusing slang, and modern internet language.
- If humor risks accuracy, clarity, or respect, omit it.

## Figure decision rule

Add a figure only when it materially improves understanding of nearby source content. Good candidates include mechanisms, processes, sequences, anatomy, spatial arrangements, comparisons, workflows, cause-and-effect chains, important objects, and visual examples.

Skip a figure when it would merely decorate the page, repeat a paragraph without adding structure, depend on unsupported details, or exist only to carry a joke. Do not use a fixed number of figures. Do not force one into every section. Do not reuse recurring characters unless the source already establishes them. Choose a visual style that fits the subject instead of hard-coding one style.

When a figure is justified, place it close to the text it teaches without moving or wrapping original material. Use the exact environment and prompt requirements in [image-prompt-templates.md](references/image-prompt-templates.md).

## Final integrity check

Before returning, verify that:

- the input envelope is unchanged
- no wrapper was added
- all original structure, comments, markers, and order remain
- all facts, numbers, terms, qualifications, uncertainty, methods, results, and limitations remain
- no unsupported information or joke was added
- each added figure has a real `figure` environment and a detailed multiline `% IMAGE GENERATION PROMPT`
- every added figure teaches a concrete idea and is not decorative
- the result is valid LaTeX in the same structural form as the input
