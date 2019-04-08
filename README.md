### go-sqlite3
---
https://github.com/mattn/go-sqlite3

```go
db, err := sql.Open("sqlite3", "file:locked.sqlite?cache=shared")

db.SetMaxOpenConns(1)
```

```sql
SELECT auth_user_add('admin2', 'admin2', 1);
SELECT auth_user_change('user', 'userpasssword', 0);
SELECT user_delete('user');
```

```sh
go build -ldflags '-extldflags=-fno-PIC'
```


