# agent-browser

> Fast browser automation CLI built for AI agents: navigate, interact, and extract page data.
> Bundled skills document workflows; start with `agent-browser skills get core --full`.
> More information: <https://github.com/agent-browser/agent-browser>.

- Open a URL in the browser:

`agent-browser open {{https://example.com}}`

- Dump the accessibility tree with element refs (best starting point for agents):

`agent-browser snapshot`

- Click an element by CSS selector or `@ref`:

`agent-browser click {{button.submit}}`

- Clear and fill an input field:

`agent-browser fill {{input#email}} "{{user@example.com}}"`

- Wait for an element to appear (or wait a number of milliseconds):

`agent-browser wait {{.results|2000}}`

- Extract text, HTML, or an attribute from the page:

`agent-browser get {{text|html|url}} {{selector}}`

- Take a screenshot or save the page as a PDF:

`agent-browser {{screenshot output.png|pdf output.pdf}}`

- Run arbitrary JavaScript in the page context:

`agent-browser eval "{{document.title}}"`
