**Released today** (v24 - Universal SQL) @channel

This is a large release containing significant **Breaking Changes** and major new features. If you haven’t seen it already, here’s a recording of our [recent community call](recent community call) discussing these changes.

We will continue to support legacy Evidence projects, and publish bug fixes for those earlier versions for some time.

Thank you to everyone who helped us by providing feedback on the pre-release.


**New Features**
- **Evidence Query Engine**: fast query engine powered by [DuckDB WASM](https://duckdb.org/2021/10/29/duckdb-wasm.html) included in every project
- [**Inputs and filters in pure SQL**](https://docs.evidence.dev/core-concepts/filters/): using query parameters, e.g. `where month='${input.selected_month}'`
- [**Dropdown component**](https://docs.evidence.dev/components/dropdown): allowing end users to pick parameters - the first input component with more coming soon
- [**Multiple data sources**](https://docs.evidence.dev/core-concepts/data-sources/#connect-your-data-sources): query and join data from multiple databases, flat files and / or other third party data sources
- [**Pluggable connectors and components**](https://docs.evidence.dev/plugins/source-plugins): easily add your own custom sources

**Docs & Guides**
- **New docs site** for Universal SQL is live at [docs.evidence.dev](https://docs.evidence.dev)
- **Legacy docs site accessible** at [legacy.docs.evidence.dev](https://legacy.docs.evidence.dev)
- [**Migration guide**](https://docs.evidence.dev/guides/usql-migration-guide) - to assist with migrating your existing legacy Evidence project, and change deprecated syntax
- [**VSCode migration script**](https://docs.evidence.dev/guides/usql-migration-guide#using-the-vs-code-migration-command): to migrate legacy projects to USQL

**Use Universal SQL**
- [**Start a new Universal SQL project**](https://docs.evidence.dev/getting-started/install-evidence)
- [**Migrate an existing Evidence project**](https://docs.evidence.dev/guides/usql-migration-guide)