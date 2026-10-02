# ✂️ Photo Cropper

A lightweight, privacy-focused, browser-based photo cropping and framing tool designed for preparing participant photos, profile pictures, avatars, and website cards to exact aspect ratios without cutting off subjects or degrading quality.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-success)

---

## 🌟 Why Photo Cropper?

When publishing profile pictures or competition submissions to a website, images often arrive in inconsistent orientations and sizes. A fixed aspect ratio (such as portrait `6:7` or `4:5`) is often required:
- **Cropping wide images**: You cut out the sides.
- **Cropping tall images**: You cut out the top and bottom.
- **Extreme close-ups / Zoomed-in faces**: Cropping directly would cut off faces abruptly.

**Photo Cropper** solves this by letting you:
1. Frame the subject centered inside your target aspect ratio box.
2. Shrink or reposition the photo inside the frame and automatically fill empty border space using colors sampled directly from the photo's background.
3. Resize the final output to web-friendly dimensions (e.g., `600×700` px) and export optimized JPEG/PNG images with controlled file sizes.

---

## ✨ Features

- **Custom Aspect Ratios**: Default `6:7` portrait ratio, fully editable to any custom ratio (e.g. `1:1`, `4:5`, `16:9`, `3:4`), with a one-click ratio swap button (`⇄`).
- **Flexible Fit & Fill Modes**:
  - **Fill Mode**: Scales the image so it covers the entire target box (crop excess).
  - **Fit Mode**: Scales the entire image within the box and pads the remaining space with the chosen background color.
- **Smart Background Fill**:
  - **Auto-Detect**: Automatically samples corner pixels of your photo to choose a seamless matching background color.
  - **Eyedropper Tool (`💧`)**: Click anywhere on the image canvas to pick an exact color.
  - **Color Picker**: Choose any hex color manually.
- **Precision Zoom & Pan Controls**:
  - Drag to reposition with mouse or touch.
  - Smooth log-scale zoom slider (`5%` to `500%`).
  - Direct numeric zoom percentage input for pixel-precise scaling.
  - Fine 5% zoom buttons (`+` / `−`) and mouse wheel zoom.
  - Keyboard arrow keys for fine 1px / 10px nudging.
- **Target Resolution & Size Presets**:
  - Quick output width presets (`300px`, `600px`, `900px`, or `Max` native resolution).
  - Automatically calculates target height based on the selected aspect ratio.
- **Format & Quality Control**:
  - Export as **PNG** or **JPEG**.
  - Adjustable JPEG quality slider (default `85%`) to avoid file size bloat.
  - Real-time output dimension indicator and download file size readout.
- **100% Client-Side & Private**: Runs entirely in your local browser using HTML5 Canvas. No images or data are ever transmitted to any server.
- **Zero Build / Zero Dependencies**: Pure HTML, CSS, and vanilla JavaScript in a single self-contained file.

---

## 🚀 Quick Start

### Option 1: Open Directly in Browser
No installation, node, or web server required!

1. Clone or download this repository:
   ```bash
   git clone https://github.com/saharsh-agrawal/photo-cropper.git
   ```
2. Double-click `index.html` (or open it with Chrome, Firefox, Edge, Safari, etc.).

### Option 2: Run with a Local Static Server (Optional)
If you prefer running via a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js npx
npx serve .
```
Then visit `http://localhost:8000` in your browser.

---

## ⌨️ Controls & Shortcuts

| Action | Shortcut / Gesture |
|---|---|
| **Upload Photo** | Click **📂 Upload**, drag & drop a file, or paste from clipboard (`Ctrl + V`) |
| **Move Image** | Click and drag on canvas, or touch drag |
| **Nudge Position** | `Arrow Keys` (1 px) or `Shift + Arrow Keys` (10 px) |
| **Zoom In / Out** | Mouse wheel, zoom slider, type zoom %, or `+` / `−` keys |
| **Reset to Default Fill** | `0` key or click `↺` |
| **Save / Download** | `Ctrl + S` / `Cmd + S` or click **💾 Save** |

---

## 🛠️ Supported Image Formats

Accepts any format supported by modern browsers:
- JPEG / JPG
- PNG
- WebP
- GIF
- BMP / SVG

---

## 🔒 Privacy & Security

All image rendering, manipulation, color sampling, and file generation occur locally in memory via the browser's Canvas API. Your pictures never leave your device.

---

## 🤝 Contributing

Contributions, feature suggestions, and bug reports are welcome! Please check out [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to get started.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
