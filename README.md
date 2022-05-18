# Docker NGINX Reverse Proxy

Simple Docker and NGINX HTTP reverse proxy example deploying 4 docker service

## Link logical domain name to the IP address of the server

- localhost
- security.localhost
- weather.localhost

www.domain.com
security.domain.com
weather.domain.com

### Locally

```hosts
127.0.0.1		localhost	
127.0.0.1		security.localhost
127.0.0.1		weather.localhost
```

### VPS

Add a `A` and `CNAME` to your dns manager

```txt
IN A 45.79.250.133
```

```txt
security IN A 0.0.0.0
```

```txt
weather IN A 0.0.0.0
```
