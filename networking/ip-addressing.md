# IP Addressing

## What is an IP address?

An IP (Internet Protocol) address is a unique identifier assigned to a device on a network. It allows devices to communicate with each other.

Example:

```text
192.168.1.10
```

## Types

- Private IP – Used inside local networks
- Public IP – Accessible from the Internet
- Loopback (`127.0.0.1`) – Refers to the local machine

## Useful Commands

Show IP addresses

```bash
ip a
```

Show only IPv4 addresses

```bash
ip -4 addr
```

Show network interfaces

```bash
ip link
```

Show your public IP

```bash
curl ifconfig.me
```

## Key Points

- Every network device needs an IP address.
- Devices on the same subnet can communicate directly.
- Public IPs are assigned by an ISP.

- A subnet is a smaller network created by dividing a larger network.
- Larger CIDR = smaller network.
- Smaller CIDR = more available hosts.