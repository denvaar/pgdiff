# pgdiff

Compare what data changed in your Postgres database between two points in time.

### Usage

```
$ pgdiff <db_name> <key>
```

Delete all diffs

```
$ pgdiff -d
```

### Examples

```
$ pgdiff pbin_dev xyz
```

Time goes by, rows are inserted/updated. Now run the command again with the same database name and key params to see what data changed:

<img width="500" alt="Screen Shot 2021-08-12 at 11 23 11 PM" src="https://user-images.githubusercontent.com/10538978/129308814-936939ab-81e1-48a0-a583-6ccef3f5691e.png">

