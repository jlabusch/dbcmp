# dbcmp
Quick and dirty script for diffing PostgreSQL "plain" format DB dumps.

## Usage
1. Create a dump, e.g. `pg_dump --data-only mydb > now.sql`
2. Compare it to a previous dump! `dbcmp then.sql now.sql`

You probably want to edit the `skip_tables` list in `dbcmp` to exclude noisy or unimportant tables from your results.
