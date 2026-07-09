# pi

> Minimal, extensible terminal coding agent harness.
> Runs in interactive, print/JSON, RPC, and SDK modes.
> More information: <https://github.com/earendil-works/pi-coding-agent>.

- Start an interactive session in the current directory:

`pi`

- Run a single prompt and print the result (non-interactive):

`pi {{[-p|--print]}} "{{prompt}}"`

- Pipe `stdin` into a prompt:

`cat {{path/to/file}} | pi {{[-p|--print]}} "{{Summarize this}}"`

- Continue the most recent session:

`pi {{[-c]}}`

- Browse and resume a past session:

`pi {{[-r]}}`

- Start an ephemeral session that is not saved:

`pi --no-session`

- Install a pi package (extension, skill, theme):

`pi install {{npm:@scope/package}}`

- Fork an existing session into a new one:

`pi --fork {{session_path_or_id}}`
