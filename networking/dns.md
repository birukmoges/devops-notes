# DNS

## What is DNS?

DNS (Domain Name System) translates domain names into IP addresses.

Example:

```text
google.com
        ↓
142.250.xxx.xxx
```

## Useful Commands

View DNS servers

```bash
cat /etc/resolv.conf
```

DNS lookup

```bash
dig google.com
```

or

```bash
nslookup google.com
```

## Troubleshooting

If

```bash
ping 8.8.8.8
```

works but

```bash
ping google.com
```

fails, the problem is likely DNS.

## Key Points

- Humans remember names.
- Computers communicate using IP addresses.