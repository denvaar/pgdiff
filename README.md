# pgdiff

Compare what data changed in your Postgres database between two points in time.

### Usage

```
$ pgdiff <db_name> <key>
```

### Examples

```
$ pgdiff pbin_dev xyz
```

Time goes by, the rows are inserted/updated, run the command again with the same database name and key:
