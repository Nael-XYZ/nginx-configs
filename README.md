# Nginx Configs 🌐

Production Nginx configs for common patterns.

## Templates

- **reverse-proxy.conf**: Backend proxying with load balancing
- **rate-limit.conf**: Request rate limiting with burst
- **ssl-hardening.conf**: TLS 1.3, OCSP, HSTS
- **cache.conf**: Static asset caching
- **security-headers.conf**: CSP, X-Frame-Options, etc.

## Quick Start

```bash
cp templates/reverse-proxy.conf /etc/nginx/sites-available/myapp
ln -s /etc/nginx/sites-available/myapp /etc/nginx/sites-enabled/
nginx -t && systemctl reload nginx
```

## License

MIT