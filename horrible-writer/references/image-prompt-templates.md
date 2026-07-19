# Image prompt templates

Use a figure only when it materially teaches nearby source content. Every new figure must use a real LaTeX figure environment followed immediately by a detailed multiline comment.

## Base figure environment

```latex
\\begin{figure}[ht]
    \\centering
    \\fbox{
        \\parbox[c][6cm][c]{0.85\\textwidth}{
            \\centering
            \\textbf{IMAGE PLACEHOLDER}
        }
    }
\\end{figure}
```

Use a narrower or taller `parbox` only when the visual clearly needs it. Do not use display math, a plain text marker, or an invented image path as the placeholder.

## General prompt template

```latex
% IMAGE GENERATION PROMPT
% Create an educational illustration of [exact subject from the nearby source].
% Composition and viewpoint, [specific angle, scale, framing, and layout].
% Include [specific objects, people, parts, or steps from the source].
% Show [the mechanism, process, comparison, spatial relation, or cause and effect].
% Use arrows, labels, captions, or dialogue for [specific relationships], only when they teach the idea.
% Style, [a suitable educational visual style for this subject].
% Accessibility, high contrast, readable text, simple layout, large labels, and no clutter.
% Factual constraints, stay faithful to the source, do not add unsupported details, and do not exaggerate certainty.
% Ethical constraints, avoid stereotypes, misleading symbols, and mockery of serious subjects.
```

Replace every bracketed field with concrete content. Never leave generic wording in the final prompt.

## Mechanism template

Use for anatomy, systems, algorithms, physical processes, and feedback loops.

```latex
% IMAGE GENERATION PROMPT
% Create a clear educational diagram of [mechanism].
% Show [input] entering [system], moving through [ordered stages], and producing [source-supported output].
% Use a [front view, side view, cross-section, flow diagram, or other useful viewpoint].
% Label only [essential parts]. Use arrows to show [direction or relationship].
% Make the teaching point visible by separating [contrasting states or stages].
% Style, clean educational line art with strong contrast and restrained detail.
% Accessibility, readable labels, generous spacing, simple shapes, and no decorative background.
% Factual constraints, show only relationships stated or directly supported by the source.
% Ethical constraints, avoid misleading anatomical, cultural, or medical imagery.
```

## Sequence or workflow template

Use for procedures, historical processes, reviews, experiments, and multi-step explanations.

```latex
% IMAGE GENERATION PROMPT
% Create an educational step-by-step visual of [source process].
% Arrange [number] stages from [start] to [finish] in a clear reading direction.
% Show [specific action or evidence] in each stage and connect stages with arrows.
% Label stages with short source-faithful phrases, not invented conclusions.
% Make the visual explain why [key transition or consequence from the source] occurs.
% Style, [suitable educational comic, diagram, map, or timeline style].
% Accessibility, high contrast, large readable labels, consistent symbols, and uncluttered spacing.
% Factual constraints, preserve the source order and uncertainty.
% Ethical constraints, avoid glamorizing harm or turning serious events into a joke.
```

## Comparison template

Use when the source distinguishes two or more states, models, groups, or interpretations.

```latex
% IMAGE GENERATION PROMPT
% Create a side-by-side educational comparison of [source subjects].
% Give each side the same viewpoint and visual scale.
% Show [exact source-supported differences] and keep shared features visibly shared.
% Add labels or callouts for [essential contrasts].
% The image should teach [the distinction or tradeoff], not merely make the page attractive.
% Style, clear comparison infographic with restrained educational humor if helpful.
% Accessibility, high contrast, aligned panels, readable labels, and a simple legend.
% Factual constraints, include no details that are absent from or unsupported by the source.
% Ethical constraints, avoid stereotypes and avoid implying value judgments not made by the source.
```
