# OTP Generator (TOTP)

Generate Time-based One-Time Passwords (TOTP) using shared secret keys for two-factor authentication and security auditing.

## 🚀 Why Use OTP Generator?

The **OTP Generator** is an essential tool for cybersecurity professionals, developers, and anyone working with two-factor authentication systems. It provides real-time TOTP generation for testing, debugging, and security analysis of authentication systems.

### Security First
- **Client-Side Processing**: All OTP generation occurs locally in your browser using industry-standard cryptographic libraries
- **No Data Logging**: Secret keys and generated codes never leave your device
- **Open Standards**: Implements RFC 6238 TOTP specification using the `otplib` library
- **Time Synchronization**: Automatically synchronizes with your device's time for accurate code generation

## 🛠️ Key Features

- **Real-Time Generation**: Generates TOTP codes with live countdown timer showing remaining validity period
- **Configurable Parameters**: Customizable digits (6-8), time periods (1+ seconds), and hashing algorithms (SHA1/256/512)
- **Base32 Secret Validation**: Validates and formats Base32 encoded secret keys with real-time error feedback
- **Visual Progress Bar**: Shows remaining time until code expiration with visual countdown
- **Copy Functionality**: One-click copy for generated OTP codes
- **Auto-Refresh**: Automatically generates new codes when the time period expires

## 📖 How to Use

1. **Access the Tool**: Navigate to the [OTP Generator](https://tools.lavx.hu/tools/otp-generator) page
2. **Enter Secret Key**: Input your Base32 encoded secret key in the "Secret Key" field (e.g., `JBSWY3DPEHPK3PXP`)
3. **Configure Settings**: Adjust the number of digits (6 or 8), time period (usually 30 seconds), and hashing algorithm
4. **Generate OTP**: The tool automatically generates TOTP codes based on current time and your secret
5. **Monitor Expiration**: Watch the countdown timer and progress bar to see when the current code expires
6. **Copy Results**: Click "Copy OTP" to save the generated code to your clipboard

## 🔧 Technical Specifications

### Supported Parameters
- **Digits**: 6 or 8 digit codes
- **Time Period**: 1-300+ seconds (commonly 30 seconds)
- **Algorithms**: SHA1, SHA256, SHA512
- **Secret Format**: Base32 encoded strings

### Validation Features
- **Base32 Validation**: Ensures secret keys contain only valid Base32 characters (A-Z, 2-7, = for padding)
- **Time Remaining Calculation**: Uses `totp.timeRemaining()` to show seconds left for current code
- **Auto-Correction**: Automatically formats secret keys by removing spaces and converting to uppercase
- **Real-Time Error Handling**: Provides immediate feedback for invalid secret keys or generation errors

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/otp-generator](https://tools.lavx.hu/tools/otp-generator)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: security, generator, otp, totp, authentication, 2fa, mfa, cryptography, rfc6238

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).