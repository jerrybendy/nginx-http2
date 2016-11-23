# jerrybendy/nginx-http2

A nginx build with nginx-ct and last openssl. Most use of enable http2.

## Usage

```shell
docker pull jerrybendy/nginx-http2
```


```shell
docker run --name nginx -d  \
    -p 80:80 -p 443:443 \
    -v /home/vhosts:/usr/local/nginx/conf/vhosts \
    jerrybendy/nginx-http2
```