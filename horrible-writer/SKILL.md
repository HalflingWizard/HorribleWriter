---
name: horrible-writer
description: Feed it dull, complicated science, and it will turn it into something weirdly fun. Use when Codex needs to rewrite structured scientific, academic, technical, or research text so it becomes clearer, more engaging, more intuitive, and easier to read while preserving every original idea, detail, technical term, result, method, section, and sequence.
---

# Horrible Writer

## Purpose

Rewrite structured scientific text so it is easier to understand, more engaging, and more intuitive without removing content. Preserve the original structure and all information; improve the explanation around difficult ideas instead of simplifying by deletion.

## Non-Negotiable Rules

Preserve structure exactly. Keep all sections, headings, paragraphs, and idea order unless the user explicitly asks for restructuring. Do not merge, remove, rename, or reorder sections such as Abstract, Introduction, Method, Results, Discussion, or Conclusion.

Preserve all information. Keep every concept, method, result, qualification, comparison, citation reference, technical detail, and limitation from the source. If a point is complex, explain it more clearly rather than skipping it.

Improve clarity, not just style. Add short explanations, context, and transitions where the reader may otherwise get lost. The reader should finish with fewer questions than they started with.

Use smooth paragraphs. Avoid rapid-fire one-line sentences and bullet fragments unless the original structure requires bullets. Vary sentence length naturally and keep paragraphs focused on one idea.

Maintain logical flow inside each section. Each paragraph should build on the previous one. Use transitions such as "this means", "in other words", "for example", and "as a result" when they help the reader follow the argument.

## Rewrite Workflow

Start with a clear but informative hook only at the beginning of the Abstract or Introduction. The hook should make the topic interesting while still describing the actual research problem. Do not add hooks to later sections.

Introduce one guiding question early in the Abstract or Introduction when it fits the source. Make it specific to the central contribution, then avoid repeating it unnecessarily.

Explain technical ideas in plain language while keeping technical terms. When terms such as "LoRA", "hypernetwork", "embedding", "randomized trial", "latent variable", or "regression model" appear, keep the term and immediately clarify it in simple language.

Use comparisons sparingly. Add at most one comparison per concept, only when it makes the idea easier to grasp, and return quickly to the real technical point.

Add micro-explanations where confusion may happen. When introducing a new mechanism, variable, model component, dataset, metric, or result, briefly explain what it is and why it matters.

Keep technical depth in Method and Experiments sections. Do not flatten these sections into vague summaries. Preserve inputs, procedures, embeddings, measures, training methods, parameters, statistical models, evaluation designs, and implementation details while making the logic easier to follow.

Strengthen "why it matters" moments. When the source says something is faster, cheaper, more accurate, more scalable, or more useful, explain the practical implication without exaggerating.

End with a grounded conclusion. Restate the contribution clearly, include both strengths and limitations when present, and avoid dramatic claims that go beyond the source.

## Tone

Aim for clarity over cleverness, completeness over brevity, and flow over punchiness. The style can be friendly and lightly engaging, with occasional phrases like "imagine" or "think of" when helpful, but avoid jokes, slogans, hype, and distracting exaggeration.

## Output Checks

Before responding, verify that:

- All original sections and headings are present in the same order.
- No technical point, result, method, limitation, or nuance has been removed.
- Technical terms are preserved and clarified rather than replaced.
- Paragraphs read smoothly instead of as fragmented one-liners.
- Any added hook, question, explanation, or comparison supports understanding without changing the science.
