# Linux File Permissions and Ownership Lab

## Objective
Practice managing Linux file permissions and ownership to protect files and control user access.

## Lab Environment
- Platform: Hack The Box Academy
- Operating system: Linux
- Topics: File permissions, ownership, and access control

## Commands Practiced

### 1. View file permissions
```bash
ls -l
ls -ld cyberlab
```
`ls -l` displays file permissions and ownership. `ls -ld` shows the directory's own permissions.

### 2. Change file permissions
```bash
chmod 755 script.sh
chmod 640 secret.txt
chmod u+x attack.txt
chmod u-x attack.txt
```
`chmod` changes read, write, and execute permissions.

### 3. Change file ownership
```bash
sudo chown david:security secret.txt
```
`chown` changes the file owner to david and the group to security, when those accounts exist and the command is authorized.

### 4. Understand numeric permissions
| Number | Permission | Meaning |
|---|---|---|
| 7 | rwx | Read, write, execute |
| 6 | rw- | Read, write |
| 5 | r-x | Read, execute |
| 4 | r-- | Read only |
| 0 | --- | No permissions |

### 5. Example: Protect a sensitive file
```bash
chmod 640 secret.txt
ls -l secret.txt
```
Expected permissions: `-rw-r-----`.

## What I Learned
- How Linux manages access for owners, groups, and others.
- How to use symbolic and numeric permissions.
- How to restrict access to sensitive files.
- How file permissions support the principle of least privilege.

## Security Takeaway
Correct file permissions help prevent unauthorized access and reduce the risk of accidental changes to important data.
