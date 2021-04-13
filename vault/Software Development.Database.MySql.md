---
id: 459e4c5e-c58e-49d1-883e-60665b5358d6
title: MySql
desc: ''
updated: 1618306933275
created: 1618306673397
---

# MySql

## Some gotchas of using MySql that don't happen with [Postgresql]

- Mysql uses empty strings and meaningless values for default null columns
- MySql changes decimal input according to the set precision (eg 2,0 precision with 100 becomes 99)
- In Mysql, `1/0 == null`
- Mysql truncates string input longer than max length
- Invalid dates like `31st of february == 0000-00-00`
- String in decimal `== 0`
