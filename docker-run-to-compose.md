# Docker Run to Compose

Convert your `docker run` commands into clean, valid Docker Compose YAML files instantly.

## 🚀 Why Use Docker Run to Compose?

Transitioning from manual container management to orchestrated services can be tedious. **Docker Run to Compose** automates this process, allowing you to transform complex CLI commands into maintainable configuration files in seconds.

### Developer-Centric Features
- **Smart Command Detection**: Automatically detects if you've pasted a full command or just the arguments, prepending `docker run` where necessary.
- **Real-time Conversion**: Powered by the `composerize` library with a 500ms debounce for a smooth, responsive experience.
- **Instant Feedback**: Immediate error reporting for invalid commands or unsupported Docker options.
- **One-Click Copy**: Quickly copy the generated YAML to your clipboard for use in your `docker-compose.yml`.

## 🛠️ Key Features

- **Heuristic Parsing**: Handles various input styles, including commands starting with `run` or just the flag arguments.
- **Client-Side Processing**: Your commands are processed entirely in your browser, ensuring privacy and speed.
- **Clean Output**: Generates standard Docker Compose format that is ready for production or development environments.
- **User-Friendly Interface**: Simple, focused design with clear input and output areas.

## 📖 How to Use

1. **Access the Tool**: Navigate to the [Docker Run to Compose](https://tools.lavx.hu/tools/docker-run-to-compose) page.
2. **Input Your Command**: Paste your `docker run` command (e.g., `docker run -d -p 8080:80 nginx`) into the input area.
3. **Automatic Conversion**: The tool will automatically convert the command as you type (after a short delay).
4. **Review Output**: Check the generated `docker-compose.yml` content in the output section.
5. **Copy Results**: Click the **Copy YAML** button to save the configuration to your clipboard.

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/docker-run-to-compose](https://tools.lavx.hu/tools/docker-run-to-compose)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: docker, docker-compose, devops, containerization, infrastructure-as-code
