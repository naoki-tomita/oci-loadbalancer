# getting started

see [https://silver0480.blog.fc2.com/blog-entry-474.html](https://silver0480.blog.fc2.com/blog-entry-474.html)

```sh
# first time cert generation
$ cp nginx/first_nginx.conf_bk nginx/nginx.conf
$ docker compose up -d load-balancer
# check and edit docker-compose.yaml for certbot entrypoint.
$ docker compose run --rm certbot certonly --webroot -w /usr/share/nginx/html/ -d nzxt-docs.tk -d www.nzxt-docs.tk
# follow instruction
$ docker compose down
```

```sh
# serve applications
$ docker compose up -d
```
