# PGP Key Pair Generator

Generate PGP (Pretty Good Privacy) key pairs with support for both RSA and ECC (Elliptic Curve Cryptography) algorithms. Create secure public/private key pairs for encryption, decryption, and digital signatures.

## 🚀 Why Use PGP Key Pair Generator?

This tool provides a secure, client-side solution for generating PGP key pairs with customizable cryptographic parameters. Whether you're setting up secure communications, implementing digital signatures, or managing cryptographic identities, this generator offers precision and reliability.

### Security First
- **Client-Side Processing**: All key generation happens entirely in your browser using the OpenPGP.js library via Web Workers
- **No Data Logging**: No keys, passphrases, or user data are transmitted to any server
- **Industry Standards**: Supports both RSA and modern ECC algorithms with configurable parameters

## 🛠️ Key Features

- **Dual Algorithm Support**: Generate keys using RSA (2048, 3072, 4096-bit) or ECC (Ed25519, Curve25519, NIST P-256/P-384/P-521)
- **Optional Passphrase Protection**: Secure your private key with a user-defined passphrase
- **Flexible User ID Configuration**: Customize name and email address for key identity
- **Instant Results**: Download keys separately or copy to clipboard
- **Web Worker Integration**: Non-blocking key generation with background processing
- **Comprehensive Error Handling**: Clear feedback for validation and generation issues

## 📖 How to Use

1. **Access the Tool**: Navigate to the [PGP Key Pair Generator](https://tools.lavx.hu/tools/pgp-key-generator) page
2. **Configure User ID**: Enter your name and email address (required for key identity)
3. **Set Key Parameters**: Choose between RSA or ECC, select key size/curve type
4. **Optional Passphrase**: Enter a passphrase to encrypt your private key (recommended for production use)
5. **Generate Keys**: Click "Generate Key Pair" and wait for the cryptographic operation
6. **Save Results**: Download or copy your public and private keys
7. **Secure Storage**: Store your private key safely - it cannot be recovered if lost

## 🔧 Technical Specifications

### Supported Algorithms
- **RSA**: 2048-bit, 3072-bit, 4096-bit keys (default: 4096-bit)
- **ECC**: Ed25519, Curve25519, NIST P-256, P-384, P-521 (default: Ed25519)

### Key Generation Process
- Uses OpenPGP.js library for cryptographic operations
- Web Worker architecture for non-blocking generation
- 60-second timeout for large key generation (e.g., 4096-bit RSA)
- Automatic key format: ASCII-armored OpenPGP format

### Security Considerations
- Private keys can be optionally encrypted with AES-256 encryption when a passphrase is provided
- All cryptographic operations are performed client-side; no sensitive data or keys are ever sent to a server
- Generated keys are not stored by the application and must be saved manually by the user

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/pgp-key-generator](https://tools.lavx.hu/tools/pgp-key-generator)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: pgp, cryptography, key-generator, encryption, security, digital-signatures, rsa, ecc, ed25519, curve25519

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).