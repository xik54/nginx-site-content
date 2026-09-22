# Nginx 网站内容

这是私有仓库 `xik54/nginx-site-content` 的内容。它保存网站静态文件和 Nginx 站点模板；VPS 上的 `nginx-vps-installer` 使用只读 Deploy Key 每 5 分钟拉取一次，并在 `nginx -t` 成功后发布。

目录约定：

```text
nginx/
  site.conf.template  # Nginx server 块；__SITE_DOMAIN__ 和 __WEB_ROOT__ 由安装器替换
site/
  index.html          # 网站静态文件根目录
```

不要提交 `.env`、TLS 私钥、数据库、上传文件、日志或任何密钥。
