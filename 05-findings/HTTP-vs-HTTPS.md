# HTTP vs HTTPS

| Feature | HTTP | HTTPS |
|---|---|---|
| Encryption | No application-data encryption | Encrypts application data |
| Typical port | 80 | 443 |
| Wireshark visibility | Application information may be readable | Application data is protected/encrypted |
| Security benefit | Limited confidentiality | Improves confidentiality and integrity in transit |
| Practical lab filter | `http` | `tcp.port==443` |

## Key Lesson

The purpose of this exercise is not simply to memorize ports. It is to understand what packet analysis reveals about network communications and why encryption matters.

## Important Security Note

HTTPS does not automatically mean a website is trustworthy. Always consider the website, certificate, domain, application behavior, and other security indicators.
