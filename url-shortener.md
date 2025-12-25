# URL Shortener

Create shortened URLs with comprehensive analytics tracking, QR code generation, password protection, and expiration dates. Manage your links with both authenticated and anonymous account options.

## 🚀 Why Use URL Shortener?

Transform long, unwieldy URLs into short, memorable links while gaining powerful insights into user engagement. **URL Shortener** provides enterprise-grade features with a developer-friendly interface, allowing you to focus on what matters most—your content.

### Key Benefits
- **Comprehensive Analytics**: Track clicks, user behavior, geographic distribution, device types, and referral sources
- **Advanced Security**: Password protection, expiration dates, and rate limiting for spam prevention
- **Flexible Account Options**: Both authenticated and anonymous account support with local storage
- **Privacy-First Design**: IP hashing and optional analytics collection protect user privacy

## 🛠️ Key Features

- **Smart URL Creation**: Automatic random slug generation or custom slugs (3-20 characters, alphanumeric with dashes)
- **Security Controls**: Password protection with bcrypt hashing and optional expiration dates
- **Detailed Analytics**: Geographic tracking, device detection, browser/OS identification, referral analysis
- **QR Code Integration**: Automatic QR code generation with download functionality
- **Rate Limiting**: Protection against abuse (10 URLs per hour per IP)
- **Metadata Extraction**: Basic favicon and title extraction based on target hostname
- **Export Capabilities**: Click analytics data export to CSV format

## 📖 How to Use

### Creating a Short URL

1. **Access the Tool**: Navigate to the [URL Shortener](https://tools.lavx.hu/tools/url-shortener) page
2. **Enter Your URL**: Paste the long URL you want to shorten in the URL input field
3. **Configure Options**: 
   - **Custom Slug**: Choose a memorable short link instead of random characters
   - **Password Protection**: Set a password (minimum 8 characters) for secure links
   - **Expiration Date**: Set an automatic deactivation date for temporary links
4. **Create Link**: Click "Create Short URL" to generate your shortened link
5. **Share or Manage**: Copy the short URL, generate QR codes, or access detailed analytics

### Managing Your URLs

**For Authenticated Users**:
- All created URLs are automatically saved to your account
- Access the **"My URLs"** page to view, manage, and delete your links
- Analytics are permanently enabled with full tracking capabilities

**For Anonymous Users**:
- Created URLs are stored locally in your browser (up to 50 recent URLs)
- Analytics are disabled for privacy protection
- URLs remain accessible as long as the browser's local storage persists

### Analytics Dashboard

Click on the **"Analytics"** button to access comprehensive tracking data:
- **Overview**: Total clicks, geographic distribution, device types, top referrers
- **Temporal Analysis**: Clicks over time with daily breakdown charts
- **Geographic Tracking**: Top countries clicking your links
- **Technology Insights**: Device types, browsers, operating systems
- **Traffic Sources**: Referrer analysis and direct traffic tracking
- **Detailed Click Log**: Individual click records with timestamp and metadata

## 🔗 Tool URLs

- **Main Tool**: [https://tools.lavx.hu/tools/url-shortener](https://tools.lavx.hu/tools/url-shortener)
- **My URLs**: [https://tools.lavx.hu/tools/url-shortener/my-urls](https://tools.lavx.hu/tools/url-shortener/my-urls) *(requires authentication)*

## 📋 Technical Specifications

### URL Validation
- Supported protocols: HTTP, HTTPS
- Open redirect protection: Blocks localhost, private IP ranges (RFC 1918), and link-local addresses
- URL format validation with international domain name support

### Slug Requirements
- **Random Slugs**: 6-character alphanumeric strings
- **Custom Slugs**: 3-20 characters, alphanumeric with single dashes (cannot start/end with dash)
- **Uniqueness**: Automatic conflict detection and resolution

### Security Features
- **Password Protection**: bcrypt hashing with salt
- **Rate Limiting**: 10 URLs per hour per IP address
- **Input Validation**: XSS and SQL injection prevention
- **Privacy Protection**: IP address hashing for analytics aggregation

### Analytics Collection
- Geographic location tracking (country, city level)
- Device type detection (desktop, mobile, tablet)
- Browser and operating system identification
- Referrer tracking for traffic source analysis
- Click timestamp recording with UTC normalization

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: web, analytics, url-shortening, link-management, qr-codes, digital-marketing, analytics-tracking

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).