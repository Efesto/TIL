---
id: 36980f07-8cf8-4d7f-bdf9-e02a1b3d2503
title: Db
desc: ''
updated: 1624631889577
created: 1618398335905
stub: true
---

https://rakyll.medium.com/things-i-wished-more-developers-knew-about-databases-2d0178464f78

- Autoincrementing ids can be a problem
  - May be necessary a global lock between db nodes
  - Sequential Ids may create hotspots with certain partitioning algorithms
  - Primary key should be a meaningful value