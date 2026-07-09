# wt

> Git worktree CLI helper: create, resume, and clean up per-task worktrees.
> Worktrees live in `~/.worktrees/<project>-<task-name>` on branch `<task-name>`.
> More information: <https://github.com/leduckhc/macos-setup>.

- Create a new worktree and branch for a task:

`wt start {{task_name}}`

- Create a worktree branched from a specific base branch:

`wt start {{task_name}} --from {{branch}}`

- Create a worktree for an existing local or remote branch:

`wt resume {{task_name}}`

- Change into a worktree (opens a subshell):

`wt cd {{task_name}}`

- List all current worktrees:

`wt list`

- Merge the branch into the default branch, then remove the worktree and branch:

`wt finish {{task_name}}`

- Remove a worktree and its branch without merging:

`wt delete {{task_name}}`

- Open a worktree in an editor/multiplexer after creating it:

`wt start {{task_name}} {{--zed|--cmux|--herdr}}`
