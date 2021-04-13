---
id: c83358fb-678a-40c9-a0c8-5e6f2234b822
title: Gotchas
desc: ''
updated: 1618307916492
created: 1618307908767
---

- Mysql uses empty strings and meaningless values for default null columns
- MySql changes decimal input according to the set precision (eg 2,0 precision with 100 becomes 99)
- In Mysql, `1/0 == null`
- Mysql truncates string input longer than max length
- Invalid dates like `31st of february == 0000-00-00`
- String in decimal `== 0`