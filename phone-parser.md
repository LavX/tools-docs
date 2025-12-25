# Phone Parser & Formatter

Parse, validate, format, and generate example phone numbers with support for international numbers.

## 🚀 Why Use Phone Parser & Formatter?

**Phone Parser & Formatter** is a comprehensive utility for working with international phone numbers. It leverages Google's libphonenumber-js library to provide accurate parsing, validation, formatting, and example generation capabilities for phone numbers.

### Key Benefits
- **Comprehensive Parsing**: Parse phone numbers with or without country codes
- **Real-time Validation**: Get instant validation feedback with visual indicators (green/red)
- **Multiple Formats**: Display international (+1 202 555 0123) and national formats
- **Smart Country Detection**: Automatically detect country from phone number, with fallback to multiple possible countries for ambiguous numbers
- **Privacy-Focused**: All processing happens entirely in your browser using libphonenumber-js

## 🛠️ Key Features

- **Parse & Validate**: Parse phone numbers with or without country codes
- **Format Numbers**: Automatically format as international or national format
- **As-You-Type Formatting**: Real-time formatting feedback as you type (shows preview below input)
- **Country Detection**: Automatically detect the country from phone number
- **Ambiguous Country Handling**: Shows multiple possible countries when country cannot be determined
- **Number Type Identification**: Identify if a number is mobile, landline, toll-free, voicemail, etc.
- **Example Generation**: Generate example phone numbers (best effort - may not succeed for all countries)
- **Extension Support**: Option to include extensions in generated examples
- **Copy to Clipboard**: Copy functionality for each parsed field with visual feedback

## 📖 How to Use

1. **Access the Tool**: Navigate to the [Phone Parser & Formatter](https://tools.lavx.hu/tools/phone-parser) page.
2. **Enter Phone Number**: Type or paste a phone number in the input field (e.g., +1 202 555 0123 or just 202-555-0123).
3. **Select Default Country**: Choose a default country from the dropdown if your number doesn't include an international prefix.
4. **View Results**: See parsed information including validation status (green=valid, red=invalid), country, and various formats.
5. **Generate Examples**: Use the generator section to create example numbers for specific countries (limited success rate for some countries).

### Parsing Examples
- With country code: `+1 202 555 0123`
- Without country code: `202-555-0123` (select US as default)
- International: `+44 20 7946 0958` (UK)

### Generated Information Displayed
- **Validation Status**: Green for valid, red for invalid numbers
- **Country**: Detected country and calling code (e.g., "US (+1)")
- **Possible Countries**: When ambiguous, shows "Possibly: US, CA" format
- **National Number**: The number without country code
- **International Format**: +CC NNN NNN NNNN format
- **National Format**: Local format for the country
- **Phone URI**: tel: link format (clickable phone numbers)
- **Number Type**: MOBILE, FIXED_LINE, FIXED_LINE_OR_MOBILE, TOLL_FREE, etc.

### Example Generator Limitations
The random example generator uses Faker.js's default phone number generation followed by libphonenumber-js validation. This approach:
- Works well for major countries (US, UK, etc.) but has limited success for others
- Tries up to 20 attempts per generation request
- May fail for countries with complex number formats
- Best suited for common countries like US, UK, CA, AU

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/phone-parser](https://tools.lavx.hu/tools/phone-parser)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: phone, parser, formatter, international, validation, libphonenumber

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).