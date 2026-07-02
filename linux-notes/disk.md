# Disk Troubleshooting

Check disk usage

```bash
df -h
```

Find largest directories

```bash
du -sh *

du -sh /var/*
```

Find large files

```bash
find / -size +500M
```

Clean apt cache

```bash
apt clean
```

Remove old logs

```bash
journalctl --vacuum-time=7d
```