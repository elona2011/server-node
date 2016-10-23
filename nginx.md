# 重启

```bash
/usr/local/nginx/sbin/nginx -s reload
```

# 配置

```bash
vi /usr/local/nginx/conf/nginx.conf
```

设置反向代理

```
upstream dip.cnsuning.com{
    server 10.37.65.66:8360 weight=1;
    server 10.37.65.68:8360 weight=1;
}
```

设置/persons走反向代理

```
location /persons {
    proxy_pass http://dip.cnsuning.com;
    proxy_redirect default;
}
```
