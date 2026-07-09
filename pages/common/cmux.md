# cmux

> Control cmux terminal topology and routing: windows, workspaces, panes, and surfaces (tabs).
> More information: <https://github.com/cmuxterm/cmux>.

- Identify the current caller context:

`cmux identify --json`

- List windows, workspaces, or panes:

`cmux {{list-windows|list-workspaces|list-panes}}`

- List surfaces (tabs) in a pane:

`cmux list-pane-surfaces --pane {{pane:1}}`

- Create a new workspace:

`cmux new-workspace`

- Split a pane to a given side:

`cmux new-split {{right}} --panel {{pane:1}}`

- Move a surface to another pane and focus it:

`cmux move-surface --surface {{surface:7}} --pane {{pane:2}} --focus true`

- Flash a surface to draw attention:

`cmux trigger-flash --surface {{surface:7}}`

- Print settings docs, schema, and config paths:

`cmux docs settings`
