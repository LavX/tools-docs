# Certificate Toolkit (PEM/CSR)

A comprehensive browser-based toolkit for inspecting, validating, and generating TLS certificates, private keys, certificate signing requests (CSRs), and OpenSSL configurations. All processing happens locally in your browser for maximum privacy and security.

## 🚀 Why Use Certificate Toolkit (PEM/CSR)?

This tool provides cybersecurity professionals, DevOps engineers, and system administrators with a complete solution for certificate management workflows. Whether you're debugging certificate issues, validating certificate chains, or generating new certificates, this toolkit offers precision and reliability.

### Security First
- **Client-Side Processing**: Your sensitive cryptographic data never leaves your browser
- **No Data Logging**: We don't store or transmit your keys, certificates, or configurations
- **Open Standards**: Built using industry-standard algorithms and the forge.js library

## 🛠️ Key Features

### Inspect & Decode
- **Certificate Analysis**: Parse X.509 certificates to extract subject, issuer, validity periods, serial numbers, SHA-256 fingerprints
- **Private Key Inspection**: Examine private key type (RSA/EC), key size, encryption status
- **CSR Validation**: Verify certificate signing requests including signature validation
- **OpenSSL Config Parser**: Parse .cnf files to extract distinguished names and Subject Alternative Names (SANs)
- **Multi-format Support**: Automatic DER-to-PEM conversion for certificates and CSRs

### Validate Relationships
- **Public Key Matching**: Verify that private keys match certificates and CSRs (RSA supported)
- **Certificate Chain Verification**: Validate certificates against provided CA chains using local trust stores
- **Configuration Consistency**: Check that CNs and SANs align between certificates, CSRs, and OpenSSL configs
- **Expiration Monitoring**: Track certificate validity periods with visual risk indicators and day-remaining counters

### Generate Cryptographic Assets
- **RSA Key Generation**: Generate 2048, 3072, or 4096-bit RSA key pairs in-browser
- **Certificate Signing Requests**: Create CSRs with custom subjects and SANs
- **Self-Signed Certificates**: Generate self-signed certificates (up to 825 days validity)
- **Export Options**: Download generated assets as PEM files or copy to clipboard

## 📖 How to Use

### Inspect Certificates & Keys
1. **Navigate to the Tool**: Go to the [Certificate Toolkit](https://tools.lavx.hu/tools/tls-certificate-decoder) page
2. **Upload or Paste Content**:
   - Certificates: Paste PEM content or upload .crt/.cer/.pem files (supports DER auto-conversion)
   - Private Keys: Paste PEM content or upload .key/.pem files (supports legacy PKCS#1 encrypted keys)
   - CSRs: Paste PEM content or upload .csr/.pem files (supports DER auto-conversion)
   - OpenSSL Configs: Paste .cnf content or upload configuration files
3. **Decode Instantly**: Click "Decode & Check" to parse and validate all content
4. **Review Results**: Examine decoded information and validation results

### Validate Relationships
- The tool automatically checks relationships between uploaded content:
  - Private key ↔ Certificate public key matching
  - Private key ↔ CSR public key matching
  - Certificate/CSR CN alignment with OpenSSL config
  - SAN coverage validation
  - Certificate chain verification (when CA certificates are provided)

### Generate New Assets
1. **Switch to Generate Tab**: Click the "Generate" tab
2. **Configure Subject**: Fill in distinguished name fields (CN, O, OU, C, ST, L)
3. **Set SANs**: Add DNS names and IP addresses for Subject Alternative Names
4. **Choose Key Parameters**: Select key size (2048/3072/4096 bits) and optional validity period
5. **Select Generation Options**: Choose to generate CSR, self-signed certificate, or both
6. **Generate**: Click "Generate in browser" to create cryptographic assets
7. **Export Results**: Use copy buttons or download generated PEM files

### Advanced Features
- **Batch CA Processing**: Upload multiple CA certificates for chain validation
- **File Format Auto-Detection**: Best-effort DER-to-PEM wrapping for binary certificates and CSRs
- **Encrypted Key Support**: Passphrase decryption for legacy PKCS#1 RSA keys
- **CNF Prefill**: Auto-populate generator fields from parsed OpenSSL configurations

## 🔗 Access the Tool

**Tool Link**: [https://tools.lavx.hu/tools/tls-certificate-decoder](https://tools.lavx.hu/tools/tls-certificate-decoder)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: cybersecurity, certificate management, TLS/SSL, PKI, DevOps, certificate authority, public key infrastructure, cryptography

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).