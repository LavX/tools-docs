# SSH Key Generator

Generate secure SSH key pairs (Ed25519 or RSA) client-side with OpenSSH-compatible public key format.

## 🚀 Why Use SSH Key Generator?

This tool provides a secure, privacy-focused solution for generating SSH key pairs directly in your browser. Whether you're setting up secure server access, configuring Git repositories, or managing multiple systems, this generator offers the security and convenience you need.

### Security First
- **Client-Side Processing**: All key generation happens locally in your browser using the Web Crypto API
- **No Data Transmission**: Your private keys never leave your device
- **No Data Logging**: No inputs or generated keys are stored or transmitted
- **Modern Cryptography**: Uses industry-standard Ed25519 and RSA algorithms

## 🛠️ Key Features

- **Dual Key Support**: Generate both Ed25519 (recommended) and RSA key pairs
- **Configurable RSA Key Sizes**: Choose between 2048-bit or 4096-bit RSA keys
- **OpenSSH Format**: Public keys are formatted for immediate use in `authorized_keys` files
- **Multiple Private Key Formats**: Export private keys as both JWK (JSON Web Key) and PEM (PKCS#8) formats
- **Custom Comments**: Add custom comments to your public keys for identification
- **One-Click Downloads**: Download both public and private keys instantly
- **Copy to Clipboard**: Quick copy functionality for public keys

## 📖 How to Use

1. **Access the Tool**: Navigate to the [SSH Key Generator](https://tools.lavx.hu/tools/ssh-key-generator) page
2. **Select Key Type**: Choose between Ed25519 (recommended) or RSA key type
3. **Configure RSA Options**: If selecting RSA, choose between 2048 or 4096-bit key size
4. **Add Comment**: Optionally add a comment to identify your key (e.g., user@hostname)
5. **Generate Keys**: Click "Generate SSH Key Pair" to create your key pair
6. **Download Keys**: Use the download buttons to save your public key (`.pub`) and private key (`.pem` or `.jwk`)
7. **Install Public Key**: Add the public key content to your server's `~/.ssh/authorized_keys` file

## 🔧 Key Format Details

### Ed25519 Keys
- **Public Key**: `ssh-ed25519 <base64_data> [comment]`
- **Private Key**: Available in PEM (PKCS#8) and JWK formats
- **Security**: Modern, fast, and secure elliptic curve cryptography

### RSA Keys
- **Public Key**: `ssh-rsa <base64_data> [comment]`
- **Private Key**: Available in PEM (PKCS#8) and JWK formats
- **Key Sizes**: 2048-bit or 4096-bit options

### Private Key Conversion
If you need to convert the downloaded PEM (PKCS#8) private key to the native OpenSSH format, you can use the following command:
```bash
ssh-keygen -i -f key.pem -m PKCS8
```

## ⚠️ Important Security Notes

- **Private Key Protection**: Your private key should be kept secure and never shared
- **Browser Compatibility**: Ensure your browser supports the Web Crypto API for Ed25519 keys
- **Key Backup**: Download and securely store your private key immediately after generation
- **Server Configuration**: Copy only the public key content to your server's `authorized_keys` file

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/ssh-key-generator](https://tools.lavx.hu/tools/ssh-key-generator)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, system administrators, and security professionals. Our mission is to provide high-quality, privacy-respecting tools that make your digital infrastructure management easier.

**Related Topics**: ssh, cryptography, security, key-generation, devops, system-administration

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).