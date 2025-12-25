# IOC Defanger

Safely format and neutralize malicious Indicators of Compromise (IOCs) such as URLs, IP addresses, and domains for secure reporting, documentation, and sharing.

## 🚀 Why Use IOC Defanger?

In cybersecurity operations and threat intelligence, sharing raw malicious links or IP addresses can lead to accidental clicks, automated link-following by security tools, or unintended infections. **IOC Defanger** is a specialized utility for security professionals to neutralize these threats by converting them into a non-clickable, "defanged" format. It also provides "refanging" capabilities to restore the original indicators when technical analysis is required.

### Security & Privacy
- **Client-Side Processing**: All transformations are performed locally in your browser. Your IOCs are never transmitted to or stored on any server.
- **Privacy First**: We do not log, track, or store any data processed through this tool.
- **Instant Execution**: High-performance, regex-based processing provides immediate results for single or bulk indicators.

## 🛠️ Key Features

- **Automated Defanging**: Neutralizes URLs and IP addresses using industry-standard security formatting.
- **Indicator Refanging**: Reverses common defanging patterns to restore original IOCs for use in sandboxes or analysis tools.
- **Bulk Processing Support**: Handles multi-line input in a dedicated text area, allowing you to process large lists of indicators simultaneously.
- **One-Click Copy**: Integrated clipboard support for quickly moving results into reports or tickets.
- **Session Reset**: Quickly clear the input workspace with a dedicated "Clear" button.
- **Optimized UI**: A clean, dark-themed interface with a holographic aesthetic, designed for high-visibility and focus during security workflows.

## 📖 Technical Logic

### Defanging Process
The tool applies the following transformations to the input text:
- **Protocol Neutralization**: Detects `http://` and `https://` (case-insensitive) and converts them to `hxxp://` and `hxxps://` respectively. The resulting protocol is always normalized to lowercase.
- **Dot Masking**: Replaces every period (`.`) with a bracketed dot `[.]`. This prevents email clients, chat platforms, and browsers from interpreting the text as a clickable hyperlink.

### Refanging Process
The tool reverses common defanging patterns to restore the original indicator:
- **Protocol Restoration**: Detects `hxxp://` and `hxxps://` (case-insensitive) and restores them to `http://` and `https://`. The resulting protocol is normalized to lowercase.
- **Dot Restoration**: Replaces both bracketed dots `[.]` and parenthesized dots `(.)` with a standard period (`.`).

## 📖 How to Use

1. **Input Your Data**: Paste your URLs, IP addresses, or domains into the **Input Indicators** text area.
2. **Select Action**:
   - Click **Defang** to neutralize the indicators.
   - Click **Refang** to restore defanged indicators to their original state.
3. **Review Results**: The processed output is displayed in the **Result** section in a clear, monospaced format.
4. **Export**: Use the **Copy** button to save the output to your clipboard, or **Clear** to reset the input field.

## 🔗 Access the Tool

You can access the IOC Defanger directly at:
[https://tools.lavx.hu/tools/ioc-defanger](https://tools.lavx.hu/tools/ioc-defanger)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that streamline your digital workflow.

**Related Topics**: security, blue-team, threat-intelligence, ioc, defanger, refanger, malware-analysis, osint, cybersecurity-tools

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).
