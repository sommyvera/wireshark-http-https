# Command Reference

## Identify Interfaces

```bash
ip address
```

## Start HTTP Capture

```bash
sudo tcpdump -i enp0s3 -s 0 -w httpdump.pcap
```

## Start HTTPS Capture

```bash
sudo tcpdump -i enp0s3 -s 0 -w httpsdump.pcap
```

## Stop Capture

```text
CTRL+C
```

## Wireshark HTTP Filter

```text
http
```

## Wireshark HTTPS/TCP Port 443 Filter

```text
tcp.port==443
```

## Useful tcpdump Option Summary

| Option | Purpose |
|---|---|
| `-i` | Select the capture interface |
| `-s 0` | Capture the full packet snapshot using the default maximum snap length |
| `-w` | Write captured packets to a file |

## Important

Replace `enp0s3` with the actual interface shown on your system.
