# uvx

> Run a command from a Python package in a temporary, isolated environment.
> Alias of `uv tool run`; the package is fetched and cached automatically.
> More information: <https://docs.astral.sh/uv/reference/cli/#uvx>.

- Run a command provided by a package (installs it ephemerally if needed):

`uvx {{command}}`

- Run a command from a package whose name differs from the command:

`uvx --from {{package}} {{command}}`

- Run a specific version of a package:

`uvx {{package}}{{==1.2.3}}`

- Run with an extra dependency available in the environment:

`uvx --with {{extra_package}} {{command}}`

- Run using a specific Python version:

`uvx {{[-p|--python]}} {{3.12}} {{command}}`

- Run a tool from a git repository:

`uvx --from git+{{https://github.com/owner/repo}} {{command}}`

- Show help:

`uvx --help`
