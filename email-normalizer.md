# Email Normalizer

The **Email Normalizer** is a specialized utility designed to convert email addresses into their canonical (standardized) format. This tool is essential for developers and data analysts who need to deduplicate user lists, link accounts, or ensure consistent data storage.

## 🚀 Why Use Email Normalizer?

Email providers often have unique rules for how they handle addresses. For example, Gmail ignores dots and allows "plus-tagging" (sub-addressing). Without normalization, `john.doe@gmail.com` and `johndoe+news@gmail.com` might be treated as two different users, even though they point to the same inbox.

### Key Benefits
- **Deduplication**: Identify duplicate accounts that use different variations of the same email.
- **Data Integrity**: Ensure all email addresses in your database follow a consistent format.
- **Privacy-Focused**: All processing happens locally in your browser; your email data is never sent to our servers.

## 🛠️ Normalization Logic & Rules

The tool applies a set of sophisticated rules based on common email provider behaviors and RFC standards:

### General Rules
- **Domain Lowercasing**: All domain parts (after the `@`) are converted to lowercase, as domains are case-insensitive.
- **Sub-addressing (Plus Aliases)**: For most providers, everything after a `+` symbol in the local part is removed (e.g., `user+extra@domain.com` becomes `user@domain.com`).
- **Local Part Lowercasing**: For most providers (except Gmail), the local part is converted to lowercase to ensure a canonical form.

### Provider-Specific Rules

| Provider | Domain Standardization | Specific Logic |
| :--- | :--- | :--- |
| **Gmail / Googlemail** | `gmail.com` | Removes all dots (`.`) from the local part. Standardizes `googlemail.com` to `gmail.com`. |
| **Outlook / Hotmail** | Original Domain | Removes plus aliases. Supports `outlook.com`, `hotmail.com`, `live.com`, and `msn.com`. |
| **Yahoo** | `yahoo.com` | Removes plus aliases. Standardizes `ymail.com` and `rocketmail.com` to `yahoo.com`. |
| **iCloud** | `icloud.com` | Removes plus aliases. Standardizes `me.com` and `mac.com` to `icloud.com`. |

## 📖 How to Use

1. **Enter Email**: Type or paste the email address you want to normalize into the input field.
2. **Instant Feedback**: The tool validates the format and displays the normalized version immediately.
3. **Copy Result**: Click the **"Copy Normalized"** button to copy the result to your clipboard.

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/email-normalizer](https://tools.lavx.hu/tools/email-normalizer)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: email-security, data-cleaning, devops-tools, canonical-email, deduplication
