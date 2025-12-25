# Homoglyph Generator

The **Homoglyph Generator** is a specialized security utility designed to generate look-alike domains using ASCII substitution, Unicode homoglyphs (IDN homographs), and common typosquatting techniques. It is an essential tool for phishing research, defensive monitoring, and security awareness testing.

## 🚀 Why Use Homoglyph Generator?

In modern cybersecurity, attackers often use deceptive domains to trick users into visiting malicious websites. The Homoglyph Generator helps security professionals proactively identify these potential threats by generating variations of a target domain, allowing for better monitoring and user training.

### Security & Privacy
- **Client-Side Execution**: All generation logic runs entirely in your browser. Your target domains are never transmitted to our servers.
- **Privacy-First**: We do not log, store, or track any input domains or generated results.
- **Ethical Use**: Built specifically for OSINT, red teaming, and defensive security research.

## 🛠️ Key Features

- **Multi-Technique Generation**: Combines ASCII substitution, Unicode homoglyphs, and typosquatting for comprehensive coverage.
- **Instant Results**: Generates dozens of variations in milliseconds directly in the browser.
- **Categorized Output**: Variations are clearly labeled by type (ASCII, Unicode, or Typo) with detailed descriptions of the modification.
- **Efficient Export**: Copy individual domains or the entire list to your clipboard with a single click.
- **Visual Indicators**: Uses distinct icons and color-coding to differentiate between generation methods.

## 📖 How to Use

1.  **Input Target Domain**: Enter the domain you wish to analyze (e.g., `google.com`) into the search field.
    *   *Note: The tool mutates the first segment of the domain (the part before the first dot). For `sub.example.com`, it will mutate `sub`.*
2.  **Generate Variations**: Click the **Generate** button to execute the mutation logic.
3.  **Analyze Results**: Review the generated list, which is categorized into:
    *   **ASCII**: Visual substitutions using standard ASCII characters.
    *   **Unicode**: IDN homographs using look-alike characters from non-Latin scripts (primarily Cyrillic).
    *   **Typo**: Simulated human typing errors like omissions, doublings, and swaps.
4.  **Export Data**: Use the copy icons to save individual domains or the **Copy All** button for the full list.

## ⚙️ Generation Logic

The tool processes the input by converting it to lowercase, trimming whitespace, and splitting it at the first dot. The prefix (the part before the dot) is mutated, while the remainder (TLD and subsequent segments) remains unchanged.

### 1. ASCII Substitution
Performs single-character replacements with visually similar standard ASCII characters. The tool iterates through the prefix and generates a new domain for each possible substitution:
- `a` → `4`, `@`
- `b` → `8`
- `e` → `3`
- `g` → `9`, `q`
- `i` → `1`, `l`
- `l` → `1`, `I`
- `o` → `0`
- `s` → `5`, `$`
- `t` → `7`
- `z` → `2`

### 2. Unicode Homoglyphs
Utilizes Cyrillic characters that are visually indistinguishable from Latin characters in most modern fonts.
- **Full Mask**: Generates a version where *every* compatible character in the prefix is replaced with its Cyrillic counterpart.
- **Single Replacement**: Generates versions where only one compatible character is replaced at a time.

**Supported Mappings:**
- `a` → `а` (Cyrillic small letter a)
- `c` → `с` (Cyrillic small letter es)
- `e` → `е` (Cyrillic small letter ie)
- `o` → `о` (Cyrillic small letter o)
- `p` → `р` (Cyrillic small letter er)
- `x` → `х` (Cyrillic small letter ha)
- `y` → `у` (Cyrillic small letter u)
- `i` → `і` (Cyrillic small letter Byelorussian-Ukrainian i)
- `j` → `ј` (Cyrillic small letter je)

### 3. Typosquatting
Simulates common human typing errors:
- **Omission**: Removing a single character from the prefix (e.g., `goole.com`).
- **Doubling**: Repeating a character in the prefix (e.g., `gooogle.com`).
- **Swapping**: Interchanging two adjacent characters in the prefix (e.g., `googel.com`).

## 🔗 Access the Tool

The Homoglyph Generator is available at:
[https://tools.lavx.hu/tools/homoglyph-generator](https://tools.lavx.hu/tools/homoglyph-generator)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of free online utilities for developers, designers, and security researchers. We focus on providing high-quality, privacy-respecting tools to streamline your workflow.

**Related Topics**: osint, security, phishing, domain-monitoring, typosquatting, idn-homograph, cybersecurity-tools
