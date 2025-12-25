# JWT Builder

Create and sign JSON Web Tokens (JWT) with various algorithms directly in your browser.

## 🚀 Why Use JWT Builder?

The **JWT Builder** is a specialized tool for developers and security professionals to quickly generate signed tokens for testing, debugging, and prototyping. It provides a clean interface to configure headers, payloads, and signing keys without needing to write custom code or use command-line utilities.

### Security First
- **Client-Side Processing**: All token generation and signing happen locally in your browser using the `jose` library. Your secrets and payloads are never sent to our servers.
- **No Data Logging**: We do not store or log any of the data you input into the tool.
- **Standard Compliant**: Built using industry-standard cryptographic algorithms and the robust `jose` library.

## 🛠️ Key Features

- **Comprehensive Algorithm Support**:
    - **HMAC (Symmetric)**: HS256, HS384, and HS512.
    - **RSA (Asymmetric)**: RS256, RS384, and RS512.
    - **ECDSA (Asymmetric)**: ES256, ES384, and ES512.
- **JSON Configuration**: Dedicated input areas for Header and Payload with full JSON support.
- **Automatic Key Generation**: For RSA and ECDSA algorithms, the tool automatically generates a temporary, ephemeral key pair for signing.
- **Algorithm Enforcement**: The tool automatically sets the `alg` parameter in the protected header based on your selection, ensuring the token is valid for the chosen algorithm.
- **Instant Generation**: Generates the JWT immediately upon clicking the button.
- **One-Click Copy**: Easily copy the generated token to your clipboard.
- **Integration**: Direct link to the JWT Verifier to test and validate your generated tokens (best suited for HMAC algorithms).

## 📖 How to Use

1. **Select Algorithm**: Choose your desired signing algorithm from the dropdown menu.
2. **Provide Secret/Key**:
    - For **HMAC (HS)** algorithms, enter your secret key in the "Secret Key" field. The tool treats this as a UTF-8 string.
    - For **RSA (RS)** or **ECDSA (ES)** algorithms, the tool generates a temporary key pair for each generation. *Note: Manual private key input for RS/ES is currently not supported, and the generated public key is not displayed.*
3. **Configure Header**: Edit the JSON Header in the provided textarea. Note that the `alg` field will be overridden by the algorithm selected in the dropdown.
4. **Configure Payload**: Edit the JSON Payload with the claims you want to include (e.g., `sub`, `name`, `iat`).
5. **Generate**: Click the **Generate JWT** button. The tool will validate your JSON, apply the selected algorithm, and sign the token.
6. **Copy Result**: Use the **Copy Token** button to copy the resulting JWT string.

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/jwt-builder](https://tools.lavx.hu/tools/jwt-builder)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: jwt, json web token, authentication, security, hmac, rsa, ecdsa, developer tools, jose library

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).
