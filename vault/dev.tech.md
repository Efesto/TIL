---
id: d5aeb3dd-7805-46d5-87cc-170fde9fe37b
title: Technologies and tools
desc: ''
updated: 1622733844054
created: 1618398572565
stub: false
---

# MISC

[Why JWT for session is bad](http://cryto.net/~joepie91/blog/2016/06/13/stop-using-jwt-for-sessions/)
- No control server side for expiring session
- Less battle-proof implementation over secure cookies
- Less secure if Local Storage is used
- Heavier than cookie (for stateless at least)
- Not different than cookies if used just as session store