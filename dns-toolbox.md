# DNS Toolbox

A comprehensive DNS lookup and analysis suite for developers and security researchers. Perform deep DNS record inspections, analyze email security policies, and discover subdomains through wordlist brute-forcing and Certificate Transparency logs.

## 🔗 Dedicated IP Address

This tool is available at a dedicated subdomain:
- `dns.lavx.hu`

Access the tool directly at: [https://dns.lavx.hu/tools/dns-toolbox](https://dns.lavx.hu/tools/dns-toolbox)

## 🚀 Why Use DNS Toolbox?

DNS Toolbox goes beyond simple lookups by providing a unified interface for domain reconnaissance and security auditing. It combines traditional DNS queries with modern discovery techniques to give you a complete picture of a domain's infrastructure.

### Developer-Centric Features
- **Deep Inspection**: Automatically performs reverse DNS lookups and fetches GeoIP metadata for IP addresses.
- **Security Auditing**: Built-in SPF and DMARC parsers to validate email authentication policies.
- **Subdomain Reconnaissance**: Dual-mode discovery using curated wordlists and public Certificate Transparency (CT) logs.
- **Wildcard Awareness**: Intelligent wildcard detection to filter out false positives during subdomain discovery.

## 🛠️ Key Features

### 1. DNS Record Lookups
Supports all essential record types with enriched data:
- **A & AAAA**: IPv4 and IPv6 addresses with reverse hostname resolution and GeoIP metadata (City, Region, Country, ISP).
- **CNAME**: Canonical name aliases with recursive target following (up to 4 levels deep).
- **MX**: Mail exchange servers with priority levels.
- **TXT**: Text records for verification and policy data.

### 2. Email Security Analysis
- **SPF Parser**: Automatically identifies and analyzes Sender Policy Framework records.
- **DMARC Parser**: Queries and parses Domain-based Message Authentication, Reporting, and Conformance records from the `_dmarc` subdomain.

### 3. Subdomain Discovery
- **Wordlist Brute-force**: Scans a curated list of high-signal prefixes to find live hosts.
- **CT Logs Integration**: Queries public Certificate Transparency logs (via crt.sh) to find subdomains issued in SSL/TLS certificates.
- **Live Host Detection**: Automatically checks if discovered subdomains are "alive" by performing real-time DNS lookups.
- **Interesting Host Highlighting**: Flags subdomains containing keywords like `dev`, `staging`, `vpn`, `admin`, and `api`.

## 📖 How to Use

1. **Access the Tool**: Navigate to the [DNS Toolbox](https://tools.lavx.hu/tools/dns-toolbox) page.
2. **Enter Domain**: Type the domain name (e.g., `example.com`) in the input field.
3. **Configure Discovery**:
   - Toggle **Attempt subdomain discovery** for wordlist-based scanning.
   - Toggle **Certificate Transparency Logs** to find subdomains from SSL certificates.
4. **Run Lookup**: Click **Run Lookup** to start the analysis. All lookups are performed server-side to ensure accuracy and bypass browser-level DNS limitations.
5. **Analyze Results**:
   - View DNS records in the **Results Display**.
   - Check email security in the **SPF/DMARC Parser** section.
   - Explore discovered hosts in the **Subdomain Results** and **CT Logs** views.

### URL Integration
You can trigger a lookup directly via URL:
`https://tools.lavx.hu/tools/dns-toolbox?domain=example.com`

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/dns-toolbox](https://tools.lavx.hu/tools/dns-toolbox)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: networking, dns, reconnaissance, spf, dmarc, devops, osint
