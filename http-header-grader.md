# HTTP Header Grader

Evaluate website security headers and identify vulnerabilities. The **HTTP Header Grader** analyzes response headers against security best practices to provide a comprehensive security grade and detailed improvement recommendations.

## 🚀 Why Use HTTP Header Grader?

In the realm of cybersecurity, **HTTP Header Grader** provides a critical service for web developers and security professionals. It helps ensure that your web applications are protected against common attacks like XSS, Clickjacking, and MIME-type sniffing by validating the presence and configuration of essential security headers.

### Security & Privacy
- **Dual Analysis Modes**: Analyze live websites via URL or paste raw headers for manual inspection.
- **Server-Side Fetching**: URL analysis uses a secure server-side action to fetch headers, bypassing browser CORS restrictions while keeping your IP private from the target.
- **Privacy-First**: Analysis logic runs entirely in your browser. We do not log your URLs, headers, or analysis results.
- **Instant Feedback**: Get a clear security grade (A-F) and a point-based score out of 100.

## 🛠️ Key Features

- **Live URL Scanning**: Automatically fetch headers from any public URL using a server-side `HEAD` request with a custom User-Agent (`SecurityHeaderGrader/1.0`).
- **Raw Header Analysis**: Paste headers directly from browser developer tools, proxy logs, or `curl` output.
- **Comprehensive Security Checks**:
    - **HSTS (Strict-Transport-Security)**: Ensures the site is only accessed over HTTPS. (-20 points if missing)
    - **CSP (Content-Security-Policy)**: Detects missing policies (-25 points) or unsafe directives like `unsafe-inline` and `unsafe-eval` (-10 points).
    - **Clickjacking Protection**: Validates `X-Frame-Options` or the modern CSP `frame-ancestors` directive. (-15 points if both are missing)
    - **MIME Sniffing**: Verifies the `X-Content-Type-Options: nosniff` header is present. (-10 points if missing)
    - **Referrer Policy**: Checks for a defined policy to control how much referrer information is shared. (-5 points if missing)
    - **Permissions Policy**: Identifies if `Permissions-Policy` (or the legacy `Feature-Policy`) is used to restrict browser features. (Informational)
    - **Information Leakage**: Flags the exposure of server versions or technology stacks in `Server` or `X-Powered-By` headers. (-5 points if present)
- **Detailed Reporting**: Each check includes a status (Pass, Fail, Warning, Info), specific point deductions, and a clear explanation of the security implications.

## 📖 How to Use

1. **Access the Tool**: Navigate to the [HTTP Header Grader](https://tools.lavx.hu/tools/http-header-grader) page.
2. **Choose Mode**:
    - **URL**: Enter a target URL (e.g., `https://example.com`) to fetch headers automatically.
    - **Raw Headers**: Paste the full header block from an HTTP response.
3. **Analyze**: Click the **Analyze Headers** button.
4. **Review Results**:
    - Check your **Security Grade**:
        - **A**: 90 - 100 points
        - **B**: 80 - 89 points
        - **C**: 70 - 79 points
        - **D**: 60 - 69 points
        - **F**: Below 60 points
    - Examine the **Detailed Report** to see which headers passed and where improvements are needed.
    - View the actual header values associated with each check for debugging.

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/http-header-grader](https://tools.lavx.hu/tools/http-header-grader)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: security headers, HSTS, CSP, web security audit, clickjacking protection, XSS defense, pentesting tools.

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).
