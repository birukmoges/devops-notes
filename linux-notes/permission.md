# Linux Permissions

## Overview

Linux controls access to files using three permission groups:

- Owner
- Group
- Others

Permissions include:

- Read (r)
- Write (w)
- Execute (x)

Example :
```bash
-rwxr-xr--
```
Meaning :

Owner

- Read
- Write
- Execute

Group

- Read
- Execute

Others

- Read only

Numeric Values

| Permission | Value |
|------------|-------|
| r | 4 |
| w | 2 |
| x | 1 |

Examples

755

Owner:

rwx

Group:

r-x

Others:

r-x

644

Owner:

rw-

Group:

r--

Others:

r--

Useful Commands

```bash
chmod 755 file.sh

chmod +x script.sh

chmod -R 755 project/

chown ubuntu:ubuntu file.txt
```

Real Example

Deploying a shell script:

```bash
chmod +x deploy.sh

./deploy.sh
```

Common Mistakes

❌ Using 777 on production.

Instead:

Use the minimum permissions necessary.

Summary

- Use 755 for executables.
- Use 644 for most files.
- Avoid 777.