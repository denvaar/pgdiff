# pgdiff

Compare what data changed in your Postgres database between two points in time.

It works by just dumping out the tables into files in `/var/tmp/pgdiff`, so if you have a really large database, then you might have a bad time.

### Usage

Start/end a capture (use the same key a second time)

```bash
$ pgdiff postgresql://user:password@host:port/db_name -k some_key
```

Delete existing captures

```bash
# all
$ pgdiff postgresql://user:password@host:port/db_name -d

# some_key only
$ pgdiff postgresql://user:password@host:port/db_name -d -k some_key
```

Limit capture to certain tables only

```bash
# no need to use -t on the second time
$ pgdiff postgresql://user:password@host:port/db_name -k some_key -t "table_a,table_b,other table"
```

Show help info

```bash
$ pgdiff -h
```

