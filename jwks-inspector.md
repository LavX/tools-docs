# JWKS Inspector

Fetch and inspect JSON Web Key Sets (JWKS) from public endpoints to analyze public key metadata and facilitate JWT signature verification.

## 🚀 Why Use JWKS Inspector?

In modern authentication systems like OAuth 2.0 and OpenID Connect, **JWKS Inspector** is an essential tool for developers and security researchers. It allows you to easily retrieve and examine the public keys used by identity providers to sign JSON Web Tokens (JWTs).

### Security & Privacy
- **Client-Side Fetching**: The tool fetches and processes JWKS data directly in your browser.
- **No Data Logging**: We do not store the URLs you enter or the key data retrieved.
- **Standard Compliant**: Built using the industry-standard `jose` library for accurate parsing and validation.

## 🛠️ Key Features

- **Live Fetching**: Retrieve JWKS data from any publicly accessible HTTPS endpoint.
- **Key Listing**: View a summary of all keys in the set, including Key ID (`kid`), Key Type (`kty`), Algorithm (`alg`), and Usage (`use`).
- **Detailed Inspection**:
    - **RSA Keys**: View Modulus (`n`) and Exponent (`e`).
    - **EC Keys**: View Curve (`crv`) and Coordinates (`x`, `y`).
- **JSON Export**: Copy the full JSON representation of any individual key for use in your own applications or configuration files.
- **Pre-configured Examples**: Quickly test with common endpoints from Google, Microsoft, and Auth0.

## 📖 How to Use

1. **Enter JWKS URL**: Provide the endpoint URL (e.g., `https://www.googleapis.com/oauth2/v3/certs`).
2. **Fetch Keys**: Click the **Fetch JWKS** button to retrieve the key set.
3. **Select a Key**: Click on any key in the list to view its full technical details.
4. **Analyze Metadata**: Review the cryptographic parameters and intended usage of the selected key.
5. **Copy Key**: Use the **Copy Key** button to copy the key's JSON structure to your clipboard.

## 🔗 Common JWKS Endpoints

- **Google**: `https://www.googleapis.com/oauth2/v3/certs`
- **Microsoft**: `https://login.microsoftonline.com/common/discovery/keys`
- **Auth0**: `https://your-domain.auth0.com/.well-known/jwks.json`

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of free online utilities for developers and security researchers. Our mission is to provide high-quality, privacy-respecting tools that simplify complex technical tasks.

**Related Topics**: JWT, OAuth 2.0, OpenID Connect, Cryptography, Web Security

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).
