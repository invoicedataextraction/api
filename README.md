# Invoice Data Extraction REST API

Upload files, submit an extraction that says in plain words what to extract, wait for it to finish, and read the rows as JSON or download an XLSX, CSV or JSON file. An extraction submitted with `options.ask_questions` can stop and ask when the documents leave something unsettled; the caller answers and the extraction continues.

- `openapi.yaml`: the contract as the API enforces it, OpenAPI 3.1. The copy kept current is https://invoicedataextraction.com/openapi.yaml (JSON: https://invoicedataextraction.com/openapi.json); this repository mirrors it.
- The reference, with the same facts told in order and a ready-to-run script: https://invoicedataextraction.com/docs/api (Markdown: https://invoicedataextraction.com/docs/api.md).
- What changed and when, and how the API is versioned: https://invoicedataextraction.com/docs/changelog.
- A guide for AI agents and the people directing them: https://invoicedataextraction.com/docs/agents.

The base URL is `https://api.invoicedataextraction.com/v1`, with an API key as a bearer token; keys are created at https://invoicedataextraction.com/dashboard?view=API. Every account includes 50 free pages per month.

Official SDKs: Node.js, `@invoicedataextraction/sdk` ([sdk-node](https://github.com/invoicedataextraction/sdk-node)), and Python, `invoicedataextraction-sdk` ([sdk-python](https://github.com/invoicedataextraction/sdk-python)). For agents: the [MCP server](https://github.com/invoicedataextraction/mcp) and the [skill](https://github.com/invoicedataextraction/skills). Licensed under the MIT License.
