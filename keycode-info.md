# Keycode Info

Identify JavaScript key codes and event properties for keyboard events in real-time.

## 🚀 Why Use Keycode Info?

When developing web applications, handling keyboard interactions requires precise knowledge of how browsers report key presses. **Keycode Info** provides an instant, visual way to inspect every property of a `keydown` event, helping you write accurate event listeners and keyboard shortcuts.

## 🛠️ Key Features

- **Real-Time Capture**: Instantly displays event data as you press keys.
- **Comprehensive Event Data**: View `key`, `code`, `keyCode`, `which`, and more.
- **Modifier Detection**: Tracks the status of Alt, Ctrl, Meta (Cmd/Win), and Shift keys.
- **Location Awareness**: Distinguishes between standard keys, left/right modifiers, and Numpad keys.
- **Repeat Detection**: Identifies if a key is being held down.
- **Smart Prevention**: Automatically prevents default browser actions (like scrolling with Space or Arrow keys) while the tool is active, ensuring a smooth testing experience.
- **Privacy-Focused**: All event processing happens entirely in your browser; no keystrokes are sent to any server.

## 📖 How to Use

1. **Access the Tool**: Navigate to the [Keycode Info](https://tools.lavx.hu/tools/keycode-info) page.
2. **Activate Capture**: Click on the central "listening area" to focus the tool.
3. **Press a Key**: Hit any key or key combination on your keyboard.
4. **Inspect Properties**: Review the detailed breakdown of the event properties displayed below the capture area.
5. **Switch Keys**: Simply press another key to update the information instantly.

## 🔍 Event Properties Explained

- **event.key**: The value of the key (e.g., `a`, `Enter`, `ArrowUp`).
- **event.code**: The physical key code representing the key's position on the keyboard (e.g., `KeyA`, `Numpad5`).
- **event.keyCode / event.which**: Legacy numerical codes (deprecated but still widely used in older codebases).
- **Location**: Indicates the specific area of the keyboard (Standard, Left, Right, or Numpad).
- **Modifiers**: Boolean values indicating if Alt, Ctrl, Meta, or Shift were active during the event.
- **Repeat**: Indicates if the key is being held down, triggering multiple events.

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/keycode-info](https://tools.lavx.hu/tools/keycode-info)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: javascript, keyboard-events, web-development, debugging, keycodes

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).
