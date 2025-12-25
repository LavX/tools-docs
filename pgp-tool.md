# PGP Tool

Encrypt and decrypt messages using PGP (Pretty Good Privacy) with OpenPGP.js implementation. This tool provides client-side PGP operations for secure message handling.

## 🔐 What is PGP Tool?

The PGP Tool enables secure message encryption and decryption using industry-standard PGP encryption. All operations are performed entirely in your browser using Web Workers, ensuring your sensitive data remains private and local.

### Security Features
- **100% Client-Side Processing**: All encryption/decryption operations occur locally in your browser using Web Workers
- **No Data Transmission**: Your messages, keys, and results never leave your device
- **OpenPGP.js Integration**: Built on the trusted openpgp.js library for cryptographic operations
- **Web Worker Architecture**: Background processing prevents UI blocking and enhances security

## ⚙️ Core Functionality

### Encryption Mode
- Encrypt plaintext messages using recipient's public PGP key
- Support for armored PGP public keys (PEM format)
- Produces encrypted ASCII-armored output
- Input validation for proper key format

### Decryption Mode
- Decrypt encrypted messages using your private PGP key
- Support for encrypted private keys with optional passphrase
- Handles various PGP message formats

## 🚀 Key Features

- **Dual Operation Modes**: Toggle between encryption and decryption workflows
- **Error Handling**: Clear error messages for invalid keys, incorrect passphrases, or malformed data
- **Copy to Clipboard**: One-click output copying for convenience
- **Responsive Design**: Works on desktop and mobile devices
- **Loading States**: Visual feedback during operations
- **Link Integration**: Direct connection to PGP key generator tool

## 📖 How to Use

### Encrypt a Message
1. **Navigate to the Tool**: Access [PGP Tool](https://tools.lavx.hu/tools/pgp-tool)
2. **Select Encrypt Mode**: Click the "Encrypt" button in the operation selector
3. **Enter Plaintext**: Type or paste your message in the input field
4. **Add Public Key**: Paste the recipient's PGP public key in the key field
5. **Encrypt**: Click "Encrypt" to generate the encrypted message
6. **Copy Result**: Use "Copy Output" to copy the encrypted message

### Decrypt a Message
1. **Select Decrypt Mode**: Click the "Decrypt" button in the operation selector
2. **Enter Encrypted Message**: Paste the encrypted PGP message
3. **Add Private Key**: Paste your PGP private key in the key field
4. **Enter Passphrase** (Optional): If your private key is encrypted, enter the passphrase
5. **Decrypt**: Click "Decrypt" to reveal the plaintext message

### Input Requirements
- **Plaintext**: Any text content for encryption
- **Encrypted Messages**: Valid PGP ASCII-armored encrypted blocks
- **Public Keys**: Valid PGP ASCII-armored public key blocks (starting with `-----BEGIN PGP PUBLIC KEY BLOCK-----`)
- **Private Keys**: Valid PGP ASCII-armored private key blocks (starting with `-----BEGIN PGP PRIVATE KEY BLOCK-----`)
- **Passphrases**: Required only if the private key is encrypted

## 🔗 Access the Tool

Visit the PGP Tool at: [https://tools.lavx.hu/tools/pgp-tool](https://tools.lavx.hu/tools/pgp-tool)

## ➕ Additional Resources

### Generate PGP Keys
Need PGP keys? Use our [PGP Key Generator](https://tools.lavx.hu/tools/pgp-key-generator) to create key pairs.

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security professionals. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: cryptography, pgp, encryption, decryption, privacy, security, email

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).