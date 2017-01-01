# jerrybendy/nginx-http2

A nginx build with nginx-ct and last openssl. Most use of enable http2.

## Usage

```shell
docker pull jerrybendy/nginx-http2
```

You should overwrite the main `nginx.conf` by yourselves. It postioned `/usr/local/nginx/conf/nginx.conf`.

```shell
docker run --name nginx -d  \
    -p 80:80 -p 443:443 \
    -v /path/to/my/nginx.conf:/usr/local/nginx/conf/nginx.conf \
    jerrybendy/nginx-http2
```

## History

### v1.1.0

* Update `nginx` to version 1.11.8
* Update `nginx-ct` to version 1.3.2
* Add `http_stub_status_module` module