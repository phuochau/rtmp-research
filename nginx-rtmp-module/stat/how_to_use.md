Go to `nginx.conf`, find `http/server` and add these lines:

```
location /stat {
      rtmp_stat all;
      rtmp_stat_stylesheet stat.xsl;
  }

  location /stat.xsl {
        root html;
  }
```
