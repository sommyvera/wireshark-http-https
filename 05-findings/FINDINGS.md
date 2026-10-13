# Findings

## HTTP Findings

HTTP traffic does not provide the same application-data confidentiality as HTTPS.

During this exercise, Wireshark was used to inspect HTTP traffic and examine the POST request/form data.

### Evidence

See:

- `03-screenshots/03-http-filter.png`
- `03-screenshots/04-http-post-analysis.png`

## HTTPS Findings

HTTPS uses encryption to protect application data in transit.

The exercise uses Wireshark to inspect traffic associated with TCP port 443 and examine encrypted application data.

### Evidence

See:

- `03-screenshots/06-https-filter.png`
- `03-screenshots/07-encrypted-application-data.png`

## Security Interpretation

The practical difference demonstrated by this lab is the visibility of application-layer information.

HTTP can expose application information in a readable form, while HTTPS protects the application data through encryption.

However, HTTPS should not automatically be interpreted as proof that a website is trustworthy. A malicious or compromised website can also use HTTPS.
