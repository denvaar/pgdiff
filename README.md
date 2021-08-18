# pgdiff

Compare what data changed in your Postgres database between two points in time.

### Usage

Start/end a capture

```
$ PGDIFF_CONNECTION_STRING=postgresql://user:password@host:port/db_name pgdiff <key>
```

Delete all diffs

```
$ pgdiff -d
```

### Examples

```
$ pgdiff abcd
```

Time goes by, rows are inserted/updated. Now run the command again with the same database name and key params to see what data changed:


<img width="600" alt="Screen Shot 2021-08-13 at 4 45 55 PM" src="https://user-images.githubusercontent.com/10538978/129424921-918176f3-6a4a-4a23-b240-44f926f27ae4.png">


