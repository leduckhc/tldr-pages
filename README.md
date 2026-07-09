# tldr-pages (personal)

My personal [tldr](https://tldr.sh/) pages — simplified, example-driven help for the
command-line tools I actually use.

## Contents

Pages live in `pages/common/`. Current set:

`agent-browser`, `claude`, `cmux`, `codex`, `copilot`, `ffmpeg`, `flutter`,
`gh`, `herdr`, `pi`, `uv`, `uvx`, `wt`

## Usage

Install any tldr client, then point it at this repo:

```sh
# Python client (via uv)
uv tool install tldr
export TLDR_PAGES_SOURCE_LOCATION="file:///Users/le/Work/Vibe/tldr-pages/pages"
export TLDR_CACHE_ENABLED=0   # always read the local files, no stale cache

tldr pi
tldr flutter
```

## Adding a page

1. Create `pages/common/<command>.md` following the [tldr format](https://github.com/tldr-pages/tldr/blob/main/contributing-guides/style-guide.md).
2. Lint it: `npx tldr-lint pages/common/<command>.md`
3. Commit: `git add pages/common/<command>.md && git commit -m "<command>: add page"`

## Page format

```markdown
# command-name

> Short description.
> More information: <https://example.com>.

- Example description:

`command {{argument}}`
```

## License

Pages are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/),
following the upstream tldr-pages project.
