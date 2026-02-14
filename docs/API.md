---
slug: /api
sidebar_position: 1
---

# API Reference

`booktabs` exports the following functions:

## `toprule`

`toprule(stroke: heavyrulewidth)`

Adds a horizontal table rule with a default `stroke` width of `0.08em`.

## `midrule`

`midrule(stroke: lightrulewidth)`

Adds a horizontal table rule with a default `stroke` width of `0.05em`.

## `bottomrule`

`bottomrule(stroke: heavyrulewidth)`

Adds a horizontal table rule with a default `stroke` width of `0.08em`.

## `cmidrule`

`cmidrule(y: auto, start: 0, end: none, stroke: cmidrulewidth)`

Adds a partial horizontal table rule with a default `stroke` width of `0.03em`.

- `y`: row position within the table body (same coordinate system as `table.hline`)
- `start`: starting column index; `0` (the default) means no explicit start index is passed so the rule begins at the first column, while any value `> 0` is treated as a 1-based column index for `\cmidrule`
- `end`: ending column index; `none` (the default) or `0` means no explicit end index is passed so the rule extends to the last column, while any value `> 0` is treated as a 1-based column index for `\cmidrule`
- `stroke`: line width for the rule

## `booktabs-default-table-style`

`booktabs-default-table-style(doc)`

Applies a default style that disables all table borders (`#set table(stroke: none)`) so only explicit booktabs rules are shown.
