# SSH

SSH allows secure remote access to Linux systems.

Generate key

```bash
ssh-keygen
```
creating the key in the right directoty and making sure the files have the right permission is a key : the ssh key default directory is ~/.ssh



Copy key

```bash
ssh-copy-id user@server
```

Connect

```bash
ssh user@server
```

Transfer files

```bash
scp file.txt user@server:/home/user/
```

SSH Config

~/.ssh/config

```text
Host aws-server
    HostName 54.xxx.xxx.xxx
    User ubuntu
    IdentityFile ~/.ssh/aws.pem
```

Now connect using

```bash
ssh aws-server
```

Security Tips

- Disable root login.
- Use SSH keys instead of passwords.
- Disable password authentication.