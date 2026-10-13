# Wireshark: Examining HTTP and HTTPS Traffic

A beginner-friendly cybersecurity portfolio project demonstrating how to capture, inspect, and compare HTTP and HTTPS traffic using `tcpdump` and Wireshark.

## Project Overview

This project is based on the lab **Using Wireshark to Examine HTTP and HTTPS Traffic**. The activity covers two main parts:

1. Capture and analyze HTTP traffic.
2. Capture and analyze HTTPS traffic.

The lab demonstrates an important security difference: HTTP traffic can expose application-layer information in readable form, while HTTPS protects application data through encryption.

## Learning Objectives

By completing this project, you will practice:

- Identifying network interfaces with `ip address`.
- Capturing traffic with `tcpdump`.
- Saving packet captures as `.pcap` files.
- Opening packet captures in Wireshark.
- Filtering HTTP traffic with `http`.
- Filtering HTTPS-related traffic with `tcp.port==443`.
- Inspecting HTTP POST/application form data.
- Inspecting HTTPS/TLS encrypted application data.
- Comparing plaintext HTTP with encrypted HTTPS.
- Documenting practical cybersecurity work on GitHub.

## Lab Environment

The source lab specifies:

- CyberOps Workstation VM
- Internet connection
- `tcpdump`
- Wireshark
- A web browser

> Adapt the network interface name to your own VM. The source lab uses `enp0s3` as an example.

## Project Workflow

```text
Identify Interface
       ↓
Start tcpdump
       ↓
Generate HTTP Traffic
       ↓
Stop Capture
       ↓
Open .pcap in Wireshark
       ↓
Filter HTTP
       ↓
Inspect POST/Form Data
       ↓
Capture HTTPS Traffic
       ↓
Filter tcp.port==443
       ↓
Inspect Application Data
       ↓
Compare HTTP vs HTTPS
       ↓
Document Findings
       ↓
Push Project to GitHub
```

## Repository Structure

```text
wireshark-http-https/
├── README.md
├── 01-lab-documentation/
│   ├── LAB-GUIDE.md
│   └── OBSERVATIONS.md
├── 02-command-reference/
│   └── COMMANDS.md
├── 03-screenshots/
│   └── README.md
├── 04-pcap-analysis/
│   └── README.md
├── 05-findings/
│   ├── FINDINGS.md
│   └── HTTP-vs-HTTPS.md
├── 06-reflection/
│   └── REFLECTION.md
├── .gitignore
└── LICENSE
```

## Important Security Note

Do **not** upload real usernames, passwords, session cookies, private tokens, personal data, or sensitive packet captures to a public GitHub repository.

The original lab uses demonstration credentials. For your portfolio, document the technique and observations without publishing credentials or sensitive traffic.

## Portfolio Evidence

Use the `03-screenshots` folder to document evidence such as:

- Network interface output
- tcpdump running
- HTTP capture opened in Wireshark
- HTTP filter and POST packet
- HTTP form data inspection
- HTTPS capture
- `tcp.port==443` filter
- TLS/Application Data packet
- Encrypted application data inspection

## Skills Demonstrated

**Networking:** packet capture, TCP/IP traffic, ports, HTTP, HTTPS, TLS

**Security:** plaintext exposure, encryption, traffic inspection, security analysis

**Tools:** Linux terminal, tcpdump, Wireshark

**Documentation:** GitHub project organization, screenshots, findings, reflection

## Source Lab

This portfolio workflow is based on the uploaded Cisco Networking Academy lab, **Lab - Using Wireshark to Examine HTTP and HTTPS Traffic**.

## Author

**Digital Eselsa**

Cybersecurity Training & Practical Labs
