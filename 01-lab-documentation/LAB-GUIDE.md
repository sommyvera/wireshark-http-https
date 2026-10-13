# Lab Guide

## Part 1 — Capture and View HTTP Traffic

### 1. Identify the Network Interface

Run:

```bash
ip address
```

Record the interface used by the workstation.

The source lab demonstrates `enp0s3`, but your interface may be different.

### 2. Start the HTTP Packet Capture

Example:

```bash
sudo tcpdump -i enp0s3 -s 0 -w httpdump.pcap
```

If your interface is different, replace `enp0s3`.

The capture is saved as:

```text
httpdump.pcap
```

### 3. Generate HTTP Traffic

Using the lab's designated HTTP test website, generate normal web traffic and perform the required login/test action.

Do not use personal credentials.

### 4. Stop tcpdump

Press:

```text
CTRL+C
```

### 5. Open the Capture in Wireshark

Open `httpdump.pcap` with Wireshark.

Apply:

```text
http
```

### 6. Inspect the HTTP POST Packet

Locate a POST request and inspect the form data section.

Record what information is visible in the capture.

Document your observation in:

`01-lab-documentation/OBSERVATIONS.md`

---

## Part 2 — Capture and View HTTPS Traffic

### 1. Start the HTTPS Capture

Example:

```bash
sudo tcpdump -i enp0s3 -s 0 -w httpsdump.pcap
```

### 2. Generate HTTPS Traffic

Visit the HTTPS test site specified by the lab.

Do not publish personal credentials or sensitive traffic.

### 3. Stop the Capture

Press:

```text
CTRL+C
```

### 4. Open the HTTPS Capture

Open:

```text
httpsdump.pcap
```

in Wireshark.

### 5. Filter Port 443 Traffic

Use:

```text
tcp.port==443
```

### 6. Inspect Application Data

Select an Application Data packet and expand the relevant TLS/secure-transport information.

Determine whether the application data is readable plaintext or encrypted.

Record the observation in:

`05-findings/HTTP-vs-HTTPS.md`

---

## Expected Learning Outcome

The key comparison is that HTTP application data can be exposed in readable form, while HTTPS protects application data through encryption.

Also remember: HTTPS provides encryption, but the presence of HTTPS alone does not prove that a website is trustworthy.
