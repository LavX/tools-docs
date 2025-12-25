# IPv6 ULA Generator

Generate RFC 4193 compliant Unique Local Addresses (ULA) for private IPv6 networks.

## 🚀 Why Use IPv6 ULA Generator?

When designing internal networks, using Unique Local Addresses (ULA) ensures that your internal traffic remains private and avoids conflicts with global unicast addresses. The **IPv6 ULA Generator** provides a quick and reliable way to generate a random /48 prefix for your site, following the best practices outlined in RFC 4193.

### Developer-Centric Features
- **RFC 4193 Compliance**: Generates prefixes in the `fd00::/8` range with a pseudo-random 40-bit Global ID.
- **Instant Generation**: A new prefix is automatically generated when you load the page.
- **One-Click Copy**: Easily copy the generated /48 prefix to your clipboard for use in configuration files or documentation.
- **Educational Insights**: Learn about the structure of ULAs and how to use them for subnetting.

## 🛠️ Key Features

- **Randomized Global ID**: Uses a 40-bit pseudo-random identifier to minimize the risk of address collisions during site mergers.
- **Subnetting Ready**: The generated /48 prefix provides 16 bits for subnetting, allowing for up to 65,536 individual /64 subnets.
- **Privacy-Focused**: All generation logic happens locally in your browser; no data is sent to any server.
- **Clear Visualization**: Displays the breakdown of the prefix and provides examples of how to use it.

## 📖 How to Use

1. **Access the Tool**: Navigate to the [IPv6 ULA Generator](https://tools.lavx.hu/tools/ipv6-ula-generator) page.
2. **View Generated Prefix**: A random ULA prefix (e.g., `fdxx:xxxx:xxxx::/48`) is displayed immediately.
3. **Generate New**: If you need a different prefix, click the **"Generate New ULA Prefix"** button.
4. **Copy to Clipboard**: Click **"Copy Prefix"** to save the result.
5. **Review Details**: Check the "ULA Details" section to understand the prefix structure and see an example of a full address on the first subnet.

## 🔍 Technical Details

- **Prefix Range**: `fd00::/8` (L-bit set to 1).
- **Global ID**: 40 bits of pseudo-random data.
- **Subnet ID**: 16 bits (defaults to `0000` in the displayed prefix).
- **Interface ID**: 64 bits (typically used for host addressing).

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/ipv6-ula-generator](https://tools.lavx.hu/tools/ipv6-ula-generator)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: networking, ipv6, ula, rfc4193, address-generator, private-networking
