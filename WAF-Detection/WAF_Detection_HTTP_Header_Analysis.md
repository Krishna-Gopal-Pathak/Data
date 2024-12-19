
## WAF Detection and HTTP Header Analysis Using Curl

### Show All Response Headers:
To view all response headers from a web server, use the `-I` option with `curl`:

```bash
curl -I https://example.com
```

This command retrieves the HTTP headers without downloading the entire content of the page.

---

### Follow Redirects (e.g., from HTTP to HTTPS):
If a website redirects from HTTP to HTTPS, use the `-L` option to follow the redirects and see all response headers:

```bash
curl -I -L https://example.com
```

This shows the headers for each redirection.

---

### Get Detailed Header Information:
To get a more detailed view of both the request and response headers, use the `-v` option:

```bash
curl -v https://example.com
```

This will provide detailed information, including SSL/TLS details and the headers.
