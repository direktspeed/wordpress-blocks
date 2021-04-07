# Load when ESM is supported
- To know which scripts should be included in the page we need access to a special version of the post or we create a extra database table.
- We could also try to load url based the JS via PHP that would return a 200 empty or the desired script we should cache that aggressiv.
  - implement cache reset. slows down one reqest.
- We can also load a js file with url parameters that could do the needed operations. via reading comments or reading template tags.


# Later add support for SYSTEMJS
if the browser does not support ESM we should try to load that via SYSTEMJS or stealjs
