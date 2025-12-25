# JWT Verifier

Verify the signature of JSON Web Tokens (JWT) using secret or public keys. This tool ensures that your tokens are authentic and have not been tampered with.

## 🚀 Why Use JWT Verifier?

In modern web development and cybersecurity, JSON Web Tokens are a standard for securely transmitting information. The **JWT Verifier** allows you to quickly validate these tokens during development, debugging, or security audits without sending sensitive data to a server.

### Security & Privacy
- **Client-Side Processing**: All verification logic runs entirely in your browser using the `jose` library. Your JWTs and keys never leave your machine.
- **No Data Logging**: We do not store or log any tokens or keys provided to the tool.
- **Industry Standard**: Built on top of well-vetted cryptographic libraries to ensure accuracy and reliability.

## 🛠️ Key Features

- **Multi-Algorithm Support**:
  - **HMAC**: HS256, HS384, HS512 (using a shared secret).
  - **RSA**: RS256, RS384, RS512, PS256, PS384, PS512 (using a public key).
  - **Elliptic Curve (EC)**: ES256, ES384, ES512 (using a public key).
- **Automatic Detection**: The tool automatically identifies the algorithm from the JWT's protected header.
- **Payload Extraction**: Once verified, the tool displays the decoded payload in a formatted JSON view.
- **Instant Feedback**: Immediate validation results with clear success or error messages.
- **One-Click Copy**: Easily copy the verified payload to your clipboard.

## 📖 How to Use

1. **Access the Tool**: Navigate to the [JWT Verifier](https://tools.lavx.hu/tools/jwt-verifier) page.
2. **Input JWT**: Paste your full JWT token into the "JWT Token" field.
3. **Provide Key**:
   - For **HS** algorithms, enter your **Secret Key**.
   - For **RS**, **PS**, or **ES** algorithms, enter the **Public Key** (SPKI format).
4. **Verify**: Click the **Verify JWT** button.
5. **Review Results**:
   - A green checkmark indicates a valid signature.
   - A red cross indicates a failed verification with a specific error message (e.g., "signature verification failed", "JWT expired").
6. **Copy Payload**: If valid, you can view and copy the verified payload.

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/jwt-verifier](https://tools.lavx.hu/tools/jwt-verifier)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: jwt, security, validator, authentication, oauth2, openid-connect

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).
