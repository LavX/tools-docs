# SSL/TLS Checker

Comprehensive SSL/TLS certificate analysis tool that inspects certificates, chain validation, protocol support, cipher suites, and security configurations for any host.

## 🚀 Why Use SSL/TLS Checker?

This tool provides deep security insights for web administrators, developers, and security professionals. Get instant analysis of SSL/TLS configurations, certificate validity, protocol support, and potential security issues with detailed, actionable information.

### Key Security Analysis Features
- **Certificate Chain Validation**: Complete chain analysis with trust status
- **Protocol Support Testing**: TLS 1.3 and 1.2 compatibility verification
- **Cipher Suite Analysis**: Security assessment of supported ciphers
- **Hostname Validation**: Certificate hostname matching verification
- **OCSP Stapling Detection**: Certificate revocation status checking
- **Certificate Expiry Monitoring**: Days remaining until expiration

## 🛠️ Core Capabilities

### Certificate Analysis
- **Complete Certificate Chain**: Detailed chain verification from leaf to root
- **Subject Information**: CN, Organization, and alternative names
- **Issuer Details**: Certificate authority information
- **Validity Periods**: Precise valid from/to dates with ISO formatting
- **Expiration Tracking**: Days remaining with color-coded risk indicators
- **Self-Signed Detection**: Automatic identification of self-signed certificates

### Protocol Testing
- **TLS 1.3 Support**: Modern protocol compatibility verification
- **TLS 1.2 Support**: Legacy protocol testing with cipher suite sampling
- **Protocol Negotiation**: Shows actual negotiated protocol versions
- **ALPN Support**: Application-layer protocol negotiation detection

### Security Validation
- **Chain Trust**: Complete certificate chain trust verification
- **Hostname Matching**: Strict hostname validation against certificate
- **OCSP Stapling**: Real-time certificate revocation status checking
- **Authorization Errors**: Detailed error reporting for trust issues

## 📖 How to Use

1. **Enter Target Information**: Input a hostname (domain) in the provided field
2. **Specify Port**: Default is 443 for HTTPS, but you can specify custom ports (1-65535)
3. **Run Analysis**: Click "Check" to perform comprehensive SSL/TLS analysis
4. **Review Results**: Examine the detailed security report with multiple sections
5. **Interpret Findings**: Analyze the color-coded indicators for security status

### Input Parameters
- **Hostname**: Valid domain name (e.g., `example.com`)
- **Port**: Target port number (default: 443, range: 1-65535)

## 🔍 Results Interpretation

### Summary Section
- **Target Information**: Shows analyzed host:port combination
- **SNI (Server Name Indication)**: Displays server name used for handshake
- **Chain Validation**: Trust status with detailed error messages
- **Hostname Validation**: Certificate hostname match verification
- **OCSP Stapling**: Presence/absence of certificate revocation checking

### Certificate Chain Section
- **Leaf Certificate**: First certificate in the chain with detailed attributes
- **Chain Certificates**: Intermediate and root certificates with complete metadata
- **Subject Information**: CN, Organization, and detailed subject attributes
- **SAN Analysis**: All Subject Alternative Names (DNS and IP addresses)
- **Technical Details**: Serial numbers, SHA256 fingerprints, and self-signed status

### Protocols & Ciphers Section
- **Protocol Support Matrix**: TLS 1.3 and 1.2 support status
- **Cipher Information**: Negotiated cipher details for each protocol
- **ALPN Protocols**: Application-layer protocol negotiation results
- **TLS 1.2 Cipher Sampling**: Representative modern cipher suite support

## 🔗 Access the Tool

Access the SSL/TLS Checker at: [https://tools.lavx.hu/tools/ssl-tls-checker](https://tools.lavx.hu/tools/ssl-tls-checker)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: ssl, tls, certificate, security, networking, certificate-chain, cipher-suites, certificate-validation, ocsp, hostname-validation

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).