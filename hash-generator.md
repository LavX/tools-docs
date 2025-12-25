# Hash Generator

A secure, client-side utility for generating cryptographic hashes from text input or text-based files.

## 🚀 Why Use Hash Generator?

The **Hash Generator** provides a private environment for generating checksums and cryptographic fingerprints. By performing all calculations locally in your browser, the tool ensures that your data is never exposed to external servers.

### Security & Privacy
- **Client-Side Execution**: All hashing logic is executed directly in your browser.
- **Web Crypto API**: Utilizes the browser's native **Web Crypto API** for SHA-256 and SHA-512 algorithms.
- **SHA-3 Support**: Implements SHA3-256 and SHA3-512 using the `js-sha3` library.
- **Zero Data Transmission**: Your inputs and files are processed locally and are never sent to our servers.
- **Browser-Based History**: A history of your recent operations is stored in your browser's `localStorage` for easy access.

## 🛠️ Key Features

- **Supported Algorithms**:
  - **SHA-2**: SHA-256, SHA-512 (Native browser implementation via Web Crypto API)
  - **SHA-3**: SHA3-256, SHA3-512 (Library-based implementation)
  - **Legacy/Demonstration**: MD5, SHA-1 (Currently implemented as placeholders for demonstration purposes)
- **Input Methods**:
  - **Direct Text**: Enter or paste text directly into the input area.
  - **File Upload**: Load the content of local text files for hashing.
- **Operation History**: 
  - Automatically tracks the last 20 hash operations.
  - Displays timestamp, algorithm used, and a preview of the input.
  - Click any history item to reload its settings and results.
- **Clipboard Integration**: One-click "Copy Hash" functionality for quick use.
- **Responsive Design**: Optimized for seamless use across desktop and mobile devices.

## 📖 How to Use

1. **Select Algorithm**: Choose the hashing algorithm from the available options (e.g., SHA-256, SHA3-512).
2. **Input Data**: 
   - Type or paste text into the **Input Text** area.
   - Alternatively, click **Upload File** to import text from a local file.
3. **Generate**: Click the **Generate Hash** button to compute the result.
4. **Manage Results**:
   - The resulting hash is displayed in the output section.
   - Use **Copy Hash** to copy the result to your clipboard.
5. **History Management**:
   - Review previous operations in the **Hash History** section.
   - Click a history card to restore that specific input and algorithm.
   - Use **Clear History** to remove all stored records from your browser.

## 🔗 Access the Tool

Access the tool securely at:
[https://tools.lavx.hu/tools/hash-generator](https://tools.lavx.hu/tools/hash-generator)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a collection of privacy-focused utilities for developers and security professionals.

**Related Topics**: cryptography, checksum, sha256, sha512, sha3, data integrity, security tools, web crypto api.

Explore more at [tools.lavx.hu](https://tools.lavx.hu).
