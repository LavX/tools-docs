# Username Recon

Check username availability across 35+ platforms simultaneously including GitHub, GitLab, social media, and content platforms.

## 🚀 Why Use Username Recon?

Username Recon is a powerful OSINT (Open Source Intelligence) tool that helps you discover where a username is already registered across multiple online platforms. Whether you're performing digital footprint analysis, investigating potential threats, or managing your brand identity, this tool provides comprehensive and fast results.

### Comprehensive Platform Coverage
- **Code & Development**: GitHub, GitLab, Dev.to, Bitbucket, NPM, Docker Hub
- **Social Media**: Twitter, Instagram, TikTok, LinkedIn, Reddit, Facebook, Snapchat
- **Content Platforms**: Medium, YouTube, Twitch, Vimeo, SoundCloud, Spotify
- **Creative & Design**: Behance, Dribbble, Pinterest
- **Gaming & Community**: Steam, Discord, Telegram
- **Professional**: Stack Overflow, Quora, Kaggle

## 🛠️ Key Features

- **Parallel Processing**: Check 35+ platforms simultaneously for instant results
- **Real-time Status Updates**: Watch live as each platform is checked
- **Smart API Integration**: Uses platform-specific APIs for GitLab and Dev.to for enhanced reliability
- **Web Scraping Technology**: Utilizes Playwright to bypass restrictions and check platforms that don't offer APIs
- **Visual Results**: Color-coded indicators show taken (red), available (green), checking (blue), and error (yellow) states
- **Direct Links**: Click through to taken profiles directly from results
- **Error Handling**: Graceful handling of network issues and platform-specific edge cases

## 📖 How to Use

1. **Access the Tool**: Navigate to the [Username Recon](https://tools.lavx.hu/tools/username-recon) page
2. **Enter Username**: Type the username you want to check in the input field
3. **Start Search**: Click the "Search" button or press Enter
4. **View Results**: Watch as results populate in real-time showing which platforms have the username registered
5. **Navigate Profiles**: Click the external link icon next to taken usernames to visit the profile directly

### Result States
- **Taken** (Red): Username is already registered on that platform
- **Available** (Green): Username appears to be available for registration
- **Error** (Yellow): Unable to check this platform (network issues, rate limiting, etc.)
- **Checking** (Blue): Platform is currently being checked

## 🔧 Technical Implementation

- **Client-Side Interface**: Built with React and Next.js for responsive user experience
- **Server-Side Processing**: Uses Playwright for reliable web scraping and API calls
- **Privacy-First**: Checks are performed server-side without storing or logging usernames
- **Parallel Execution**: All platform checks run simultaneously using Promise.all for optimal performance
- **Smart Platform Detection**: Handles platform-specific quirks like Wikipedia soft 404s

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/username-recon](https://tools.lavx.hu/tools/username-recon)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100 free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: osint, social-media, username, reconnaissance, digital-forensics, brand-monitoring

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).