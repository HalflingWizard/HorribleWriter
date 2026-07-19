# Structured LaTeX rules

Use this reference when the source contains LaTeX commands, comments, lists, media blocks, or a full document wrapper.

## Protected skeleton

Treat all non-prose LaTeX as immutable. Preserve the exact order and spelling of:

- document wrappers and preamble commands
- `\\section`, `\\subsection`, `\\subsubsection`, `\\paragraph`, and other heading commands
- command arguments that act as labels, keys, filenames, or metadata
- `\\begin{...}` and `\\end{...}` environments
- lists, item order, counters, tables, equations, citations, references, labels, and macros
- `% block-id:` and `% block-type:` comments
- existing figure environments, placeholders, and image prompts

Rewrite only ordinary prose. Do not rename a heading merely to make it punchier. If the user explicitly asks for title rewriting, preserve the command and change only the natural-language argument.

## Envelope examples

Fragment input

```latex
\\section{A Topic}

Serious explanatory prose.
```

Fragment output must still begin with `\\section{A Topic}`. Do not add a preamble or document wrapper.

Complete-document input

```latex
\\documentclass{article}
\\begin{document}
...
\\end{document}
```

Complete-document output must preserve the same wrapper and its original commands.

## Block comments

Keep block comments directly above their original block.

```latex
% block-id: s01-u01-b01
% block-type: explanation
\\subsubsection{A protected block}
```

Do not move, delete, paraphrase, or attach these comments to a different block.

## Safe rewrite pattern

Keep the source claim, then add a short explanation if needed.

```text
Source claim, technical term, and qualification.
Plain-language clarification that does not add a new fact.
```

Do not replace a detailed method or result with a general summary.
