# HTTP & HTTPS

## HTTP

- HyperText Transfer Protocol
- Port 80
- Data is sent in plain text

## HTTPS

- HTTP secured with TLS
- TLS (Transport Layer Security) encrypts communication between a client and a server.
It protects data from being read or modified during transmission.
- Port 443
- Data is encrypted

## Useful Commands

Request a webpage

```bash
curl https://example.com
```

View response headers

```bash
curl -I https://example.com
```

## Key Points

- Always prefer HTTPS.
- HTTPS protects data during transmission.