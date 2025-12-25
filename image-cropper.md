# Image Cropper & Resizer

A high-performance, privacy-focused tool for cropping and resizing images directly in your browser. Process your images with professional-grade quality without uploading them to any server.

## 🚀 Why Use Image Cropper & Resizer?

The **Image Cropper & Resizer** provides a seamless way to prepare images for social media, websites, or personal use. By utilizing client-side processing, it ensures your data never leaves your device while offering advanced features typically found in desktop software.

### Key Benefits
- **Privacy First**: All image processing happens locally in your browser using the File API and Canvas. Your images are never uploaded to our servers.
- **High Quality**: Uses the [Pica](https://github.com/nodeca/pica) library for superior downscaling and interpolation, ensuring sharp results even at small sizes.
- **Flexible Workflow**: Choose between three distinct operation modes to suit your specific needs.
- **Instant Feedback**: Real-time preview of your crop area and settings.

## 🛠️ Key Features

### 1. Advanced Cropping
- **Freeform & Fixed Aspect Ratios**: Crop freely or use industry-standard presets:
  - **16:9** (Widescreen)
  - **4:3** (Standard)
  - **1:1** (Square)
  - **3:4** (Portrait)
  - **9:16** (Story/Reel)
- **Visual Interface**: Intuitive drag-and-drop crop selection powered by `react-image-crop`.
- **Precision**: Minimum crop size of 50x50 pixels to maintain image integrity.

### 2. Professional Resizing
- **Dual Modes**: 
  - **Pixels**: Enter specific width and height dimensions.
  - **Percentage**: Scale the image by a factor (e.g., 50% for half size).
- **Aspect Ratio Locking**: Toggle "Keep Aspect Ratio" to automatically sync dimensions and prevent distortion.
- **Comprehensive Presets**:
  - **Original Size**: Reset to the image's natural dimensions.
  - **Standard**: Thumbnail (100x100), Small Square (300x300), Small (640x480), Medium (1024x768), Large (1920x1080).
  - **Social Media**: Instagram Post (1080x1080), Instagram Story (1080x1920), Facebook Post (1200x630), Twitter Post (1024x512).

### 3. Operation Modes
- **Crop Then Resize**: Select a specific region and then scale that area to your desired dimensions.
- **Crop Only**: Focus purely on framing and composition without changing the resolution of the selected area.
- **Resize Only**: Scale the entire image without changing the frame.

### 4. Smart Output
- **Format Retention**: Automatically detects and maintains JPEG or PNG formats.
- **Optimized Quality**: JPEG output is optimized at 92% quality for the best balance of file size and visual clarity.
- **Transparency Support**: Full support for PNG transparency (alpha channel) during all operations.

## 📖 How to Use

1. **Upload**: Select an image from your device using the upload area.
2. **Select Operation Mode**: Choose between **Crop Then Resize**, **Crop Only**, or **Resize Only**.
3. **Adjust Crop**: If in a cropping mode, drag the handles to select your area. Use the **Crop Aspect Ratio** dropdown to lock the selection shape.
4. **Configure Resize**:
   - In **Pixels** mode, enter the width or height. Enable **Keep Aspect Ratio** to maintain proportions.
   - In **Percentage** mode, enter the scale factor.
   - Use **Resize Presets** for quick selection of common dimensions.
5. **Apply & Download**: Click **Apply Changes** to process the image, then use the **Download Processed Image** button to save the result.

## 🔗 Access the Tool

You can find the tool at the following link:
[https://tools.lavx.hu/tools/image-cropper](https://tools.lavx.hu/tools/image-cropper)

---

### 🌟 About Tools Suite

[Tools Suite](https://tools.lavx.hu) is a comprehensive collection of over 100+ free online utilities for developers, designers, and security researchers. Our mission is to provide high-quality, privacy-respecting tools that make your digital life easier.

**Related Topics**: image processing, photo editor, web graphics, social media tools, client-side processing, pica resizer, react-image-crop

Explore more tools at [tools.lavx.hu](https://tools.lavx.hu).
