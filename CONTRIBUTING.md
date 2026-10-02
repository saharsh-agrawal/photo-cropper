# Contributing to Photo Cropper

Thank you for your interest in contributing to **Photo Cropper**! 🎉

This project is built using vanilla HTML, CSS, and JavaScript with zero external libraries or build dependencies. The goal is to keep it fast, lightweight, and completely accessible without requiring complex build chains.

---

## 💡 How Can You Contribute?

You can contribute in several ways:
- **Reporting Bugs**: Found an issue with touch controls, image rendering, or aspect ratio math? Open a GitHub issue describing the bug, steps to reproduce, and your browser/OS version.
- **Suggesting Enhancements**: Ideas for handy presets, keyboard shortcuts, or UI improvements are welcome!
- **Submitting Pull Requests**: Implement a bug fix or feature.

---

## 🛠️ Development Guidelines

1. **Keep it Dependency-Free**:
   - Do not introduce external libraries (e.g. npm dependencies, bundlers, frontend frameworks, or CDN scripts) unless there is a strong justification and consensus.
   - The app should remain runnable simply by opening `index.html` in any modern web browser.

2. **Maintain Clean Code**:
   - Write clear, modern, and readable JavaScript.
   - Keep styling responsive and consistent with the dark theme palette.
   - Preserve comments explaining non-trivial coordinate math or canvas scaling logic.

3. **Privacy First**:
   - Never add telemetry, network tracking, or cloud uploading of user images. All operations must remain strictly client-side.

---

## 🚀 Submitting a Pull Request

1. **Fork** the repository and create your feature branch:
   ```bash
   git checkout -b feature/my-new-feature
   ```
2. **Make your changes** in `index.html` or documentation.
3. **Test thoroughly** across desktop and mobile browsers:
   - File upload (file picker, drag & drop, paste from clipboard).
   - Zooming (mouse wheel, slider, keyboard, +/- buttons).
   - Dragging / repositioning.
   - Fill color auto-detection and eyedropper.
   - Exporting in PNG and JPEG at different dimensions.
4. **Commit** your changes with clear, descriptive commit messages:
   ```bash
   git commit -m "Add feature: ..."
   ```
5. **Push** to your branch:
   ```bash
   git push origin feature/my-new-feature
   ```
6. **Open a Pull Request** against the `main` branch.

---

## 📜 Code of Conduct

Please treat everyone with respect, kindness, and constructive feedback.
