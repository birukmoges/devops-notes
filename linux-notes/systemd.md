# systemd

systemd manages services on Linux.

Check status

```bash
systemctl status nginx
```

Start

```bash
systemctl start nginx
```

Stop

```bash
systemctl stop nginx
```

Restart

```bash
systemctl restart nginx
```

Enable at boot

```bash
systemctl enable nginx
```

Disable

```bash
systemctl disable nginx
```

Reload configuration

```bash
systemctl reload nginx
```

List running services

```bash
systemctl list-units --type=service
```

Troubleshooting

If nginx won't start:

```bash
systemctl status nginx

journalctl -u nginx

nginx -t
```

Typical workflow

1. Edit configuration
2. Test configuration
3. Reload service

```bash
nginx -t

systemctl reload nginx
```