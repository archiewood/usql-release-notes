# Release Notes (v24 - Universal SQL)

This is a large release containing significant upgrades to the functionality of Evidence.


## New Features

- [Multiple data sources](https://docs.evidence.dev/core-concepts/data-sources/#connect-your-data-sources): query and join data from multiple databases, flat files and / or other third party data sources
- [Pluggable connectors and components](https://docs.evidence.dev/plugins/source-plugins): easily add your own custom sources
- [Filter directly in SQL](https://next.docs.evidence.dev/core-concepts/filters/):                     using query parameters, e.g. `where month='${input.selected_month}'`
- [Dropdown component](https://next.docs.evidence.dev/components/dropdown): allowing end users to pick parameters - the first of our input components with more coming soon
- [VSCode migration script](https://docs.evidence.dev/guides/usql-migration-guide): to migrate legacy projects to USQL
- [Browser SQL Engine](https://duckdb.org/2021/10/29/duckdb-wasm.html):  this enables the user facing filtering, and allows you to write queries with friendly DuckDB SQL syntax

## Universal SQL Guides
- **New docs site** for Universal SQL is live at [docs.evidence.dev](https://docs.evidence.dev)
- **Legacy docs site accessible** at [legacy.docs.evidence.dev](https://legacy.docs.evidence.dev)
- [**Migration guide**](https://docs.evidence.dev/guides/usql-migration-guide) - to assist with migrating your existing legacy Evidence project, and change deprecated syntax


## Deprecated
- **Data referencing:** `{data.my_query}` in favour of `{my_query}`
- **Legacy style filtering:** `let myvar = my_query.filter(...)` in favour of `$: myvar = my_query.filter(...)` (though you may be better off filtering in SQL)