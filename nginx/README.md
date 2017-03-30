# Pain points - NGINX
# location pointing to subdirectory
``` nginx
location /{path}/ {
    rewrite /{path}/(.*) /$1 break;
    root /{path on server}/
    ...
    break;
}
```
