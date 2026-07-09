# herdr

> Terminal-native agent multiplexer with workspaces, tabs, and panes.
> Control the running instance from the CLI over a local unix socket.
> More information: <https://herdr.dev/docs/socket-api/>.

- List panes and identify the focused (current) one:

`herdr pane list`

- List workspaces or tabs:

`herdr {{workspace|tab}} list`

- Create and name a new tab in a workspace:

`herdr tab create --workspace {{1}} --label "{{logs}}"`

- Read another pane's screen contents:

`herdr pane read {{1-1}} --source {{visible|recent|recent-unwrapped}} --lines {{50}}`

- Split a pane without moving focus:

`herdr pane split {{1-2}} --direction {{right|down}} --no-focus`

- Run a command in a specific pane:

`herdr pane run {{1-3}} "{{npm run dev}}"`

- Focus or close a tab:

`herdr tab {{focus|close}} {{1:2}}`
