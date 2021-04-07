# Security Headers
.htaccess 
```
<IfModule mod_headers.c>
Header set Strict-Transport-Security "max-age=63072000; includeSubDomains; preload"
Header set Referrer-Policy "same-origin"
Header set X-XSS-Protection "1; mode=block"
Header set x-frame-options "SAMEORIGIN"
Header set X-Content-Type-Options "nosniff"
Header set Feature-Policy "none"
Header set Content-Security-Policy "self"
</IfModule>
``` 

nginx

```
location some-location {
  add_header Strict-Transport-Security "max-age=63072000; includeSubDomains; preload" always;
  add_header Referrer-Policy "same-origin"
  add_header X-XSS-Protection "1; mode=block"
  add_header x-frame-options "SAMEORIGIN"
  add_header X-Content-Type-Options "nosniff"
  add_header Feature-Policy "none"
  add_header Content-Security-Policy "self"
}
```
