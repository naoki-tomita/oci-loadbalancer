# getting started

see [https://silver0480.blog.fc2.com/blog-entry-474.html](https://silver0480.blog.fc2.com/blog-entry-474.html)

```sh
$ docker compose up -d load-balancer nzxt-docs
$ docker compose run --rm certbot certonly --webroot -w /usr/share/nginx/html/ -d www.nzxt-docs.tk
# You should follow instruction.
$ docker compose down
```