---
id: ec4e2203-affb-46b5-9933-5a6bc03210e0
title: Postgresql
desc: ''
updated: 1622208033167
created: 1618307316347
---

![[dev.tech.db.mysql.gotchas]]

## Cool feats
- [Lateral Queries](https://www.postgresql.org/docs/13/queries-table-expressions.html#QUERIES-LATERAL)
- [Materialized views](https://www.postgresql.org/docs/9.3/rules-materializedviews.html)
- [Concurency control MVCC-based](https://www.postgresql.org/docs/current/mvcc-intro.html)
- [Window functions](https://www.postgresql.org/docs/13/tutorial-window.html)
- [Generated columns](https://www.postgresql.org/docs/12/ddl-generated-columns.html) (postgresql 12)
  - **Caveat** you cannot convert a generated column to a normal one, needs drop and recreate
- [Table partitioning](https://www.postgresql.org/docs/13/ddl-partitioning.html)
  - Cool for big table, rule of thumb when the table doesn't fit in memory
  - **Caveat** is not possible to turn a normal table in a partitioned table and reverse, but an existing table can be a paritioned table
- [Foreign data](https://www.postgresql.org/docs/13/ddl-foreign-data.html)
  - This sounds cool for migrating from different db technologies
- [Geometric types](https://www.postgresql.org/docs/13/datatype-geometric.html)
- [Domain types](https://www.postgresql.org/docs/13/domains.html)
- [Ordered indexes](https://www.postgresql.org/docs/13/indexes-ordering.html)
- [Partial indexes](https://www.postgresql.org/docs/13/indexes-partial.html)
  - Cool if the queries occurs mostly on a subset, doesn't replace partitioning tho
- [Listen/Notify](https://www.postgresql.org/docs/current/sql-notify.html)

## Tips and tricks

- To check the existence of some record, don't use `COUNT()`, use `EXISTS()` because [count is expensive](https://wiki.postgresql.org/wiki/Slow_Counting)
- `(split_part(uri, ':', 3))` is the way to go for searching on fields containing URIs, can be used as an index
- [Materialised](https://www.postgresql.org/docs/9.3/rules-materializedviews.html) views are the way to go for caching heavy queries involving not so often updated tables
  - The view update can be triggered on table update, introducing a slowdown or triggered by an external process like a cronjob or application
- Use the proper [index type](https://www.postgresql.org/docs/13/indexes-types.html) for your table
- If an index on text field needs to be case-insensitive, using an expressional index with `citext` (case insensitive text) is a good alternative to using `upper/lower` see https://www.postgresql.org/docs/13/indexes-expressional.html
- [Others on performance](https://wiki.postgresql.org/wiki/Performance_Optimization)