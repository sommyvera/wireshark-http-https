# PCAP Analysis

This folder is for documenting packet-capture analysis.

## Recommended Files

During the lab you may create:

```text
httpdump.pcap
httpsdump.pcap
```

## Public GitHub Recommendation

Do not automatically publish packet captures.

PCAP files can contain:

- Credentials
- Cookies
- URLs
- IP addresses
- Hostnames
- Application data
- Other sensitive information

For a public portfolio, use screenshots and written analysis unless you have verified that the PCAP contains only safe, intentionally generated test traffic.

## Analysis Checklist

### HTTP

- [ ] Open `httpdump.pcap`
- [ ] Apply `http`
- [ ] Locate a POST request
- [ ] Inspect form data
- [ ] Record what is visible
- [ ] Take a screenshot

### HTTPS

- [ ] Open `httpsdump.pcap`
- [ ] Apply `tcp.port==443`
- [ ] Locate Application Data
- [ ] Inspect TLS/secure transport details
- [ ] Determine whether application data is readable
- [ ] Take a screenshot

## Portfolio Principle

The goal is to demonstrate that you can capture, filter, inspect, interpret, and document network traffic—not simply upload large packet files.
