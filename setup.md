# AssetVault API documentation

### Setup and dev guide

##### 1 - Clone repo

##### 2 - Install Docsify

```bash
npm i docsify-cli -g
```

##### 3 - Run host

```bash
docsify serve .
```

##### 4 - Deploy

Nginx config:

```nginx
server {
  listen 80;
  server_name  your.domain.com;

  location / {
    alias /path/to/repo;
    index index.html;
  }
}
```

For other options check [deploy docs](https://docsify.js.org/#/deploy)
