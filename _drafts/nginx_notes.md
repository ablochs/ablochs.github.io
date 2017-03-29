```
location ~ "^/dir/(?<var1>\d{4})-(?<var2>.*?)/(?<var3>.*?)/(?<var4>.*?)/(?<var5>.*?)$" {
    proxy_pass http://api:8001/web/$var1-$var2/$var3/$var4/$var5;
}
```

