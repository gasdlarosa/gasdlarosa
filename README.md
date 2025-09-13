<div align="center">

# 👋 Hi there! I'm Gas Dela Rosa  ¯\_(ツ)_/¯

**Python Developer | Desktop Applications | Automation Tools**

[![Email](https://img.shields.io/badge/Email-d14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:gasdlarosa@gmail.com)

</div>

---

## 🛠️ Core Technologies

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Tkinter-2C5985?style=for-the-badge&logo=python&logoColor=white" alt="Tkinter"/>
  <img src="https://img.shields.io/badge/PRAW-FF4500?style=for-the-badge&logo=reddit&logoColor=white" alt="PRAW"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/Transformers-FFD700?style=for-the-badge&logo=hugging-face&logoColor=black" alt="Transformers"/>
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV"/>
  <img src="https://img.shields.io/badge/Pillow-92447A?style=for-the-badge&logo=pillow&logoColor=white" alt="Pillow"/>
  <img src="https://img.shields.io/badge/FFmpeg-007800?style=for-the-badge&logo=ffmpeg&logoColor=white" alt="FFmpeg"/>
  <img src="https://img.shields.io/badge/Ultralytics-2A3DA4?style=for-the-badge&logo=yolo&logoColor=white" alt="Ultralytics YOLO"/>
  <img src="https://img.shields.io/badge/ONNX-00594C?style=for-the-badge&logo=onnx&logoColor=white" alt="ONNX Runtime"/>
  <img src="https://img.shields.io/badge/PyMuPDF-A41D1A?style=for-the-badge&logo=pypi&logoColor=white" alt="PyMuPDF"/>
  <img src="https://img.shields.io/badge/Ghostscript-000000?style=for-the-badge&logo=ghostscript&logoColor=white" alt="Ghostscript"/>
  <img src="https://img.shields.io/badge/FontTools-4C4C4C?style=for-the-badge&logo=pypi&logoColor=white" alt="FontTools"/>
</p>

---

## 🚀 Featured Projects

<details>
<summary><strong>⬇️ Reddit Media Extractor and NSFW Classifier</strong> - Extract, classify, and organize Reddit media ⬇️</summary>
<br>

A powerful and user-friendly desktop tool for extracting images and videos from Reddit, classifying them with an AI model, and organizing them into local folders. Built with Python and CustomTkinter, it leverages the Reddit API for content retrieval and a pre-trained AI model for NSFW detection.

<div align="center">
   <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/main_window.png" width="800">
      <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/nsfw_downloads.png" width="800">
         <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/sfw_downloads.png" width="800">
            <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/videos_downloads.png" width="800">

</div>

**Key Features:**
*   **CustomTkinter GUI**: Modern, responsive, and aesthetically pleasing interface.
*   **Reddit API Integration**: Connects using PRAW for efficient post fetching.
*   **Media Extraction**: Downloads images (JPG, PNG, GIF) and videos (MP4, GIFV).
*   **Smart Video Handling**: Merges audio and video streams using FFmpeg.
*   **NSFW Classification**: Employs a Hugging Face Transformers-based AI model to classify media.
*   **Automatic Organization**: Saves media into `videos`, `nsfw`, and `sfw` subdirectories.
*   **Download History**: Prevents redundant downloads by maintaining a session-specific history.
*   **Session Management**: Save and load application settings and credentials.

</details>

<details>
<summary><strong>⬇️ TikTok Media Downloader</strong> - Download videos and media from TikTok user profiles ⬇️</summary>
<br>

A user-friendly desktop application built with Python and Tkinter, designed to download videos and media from TikTok user profiles. It leverages the powerful `yt-dlp` backend.

<div align="center">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/tiktok_media_downloader.png" width="800" alt="TikTok Media Downloader Screenshot">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/tiktok_extracted_media.png" width="800" alt="TikTok Extracted Media Screenshot">
</div>

**Key Features:**
*   **Robust `yt-dlp` Backend:** Leverages `yt-dlp` for powerful download capabilities.
*   **Authenticated Downloads:** Supports private/restricted accounts via cookies.
*   **Configurable Quality:** Choose preferred video and media quality.
*   **Flexible Naming:** Customizable file naming conventions.
*   **Advanced History Management:** Crash-proof checkpointing for download history.

</details>

<details>
<summary><strong>📷 AI Image Extractor</strong> - Crop portraits from scanned documents 📷</summary>
<br>

Automatically detects, de-skews, and crops portrait photos from scanned documents.

<div align="center">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/image-extractor-screenshot.png" width="800">
</div>

**Key Features:**
*   **AI Smart Cropping:** YOLOv8 for optimal head room.
*   **Automatic De-skew:** OpenCV for perspective correction.
*   **Multi-Format Support:** Handles PDFs, Word docs, and images.
*   **Intelligent Filenaming:** Suggests names based on source.

</details>

<details>
<summary><strong>🔐 Password Cracker</strong> - Recover passwords from compressed archives 🔐</summary>
<br>

Comprehensive tool for password recovery from ZIP, RAR, and 7z archives.

<div align="center">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/password-cracker-screenshot.png" width="800">
</div>

**Key Features:**
*   **Multiple Attack Modes:** SecLists, mask, hybrid, custom.
*   **Advanced Options:** Leet speak, keyword filtering.
*   **Session Management:** Save and load configurations.
*   **Detailed Reporting:** Statistics and password strength analysis.

</details>

<details>
<summary><strong>✒️ AI Signature Editor</strong> - Extract, recolor, and resize signatures ✒️</summary>
<br>

Extracts signatures, recolors them, and resizes them for digital documents.

<div align="center">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/e-signature-app-screenshot.png" width="800">
</div>

**Key Features:**
*   **AI Background Removal:** Accurate extraction with Deep Image Segmentation.
*   **Live Preview:** View changes instantly.
*   **Full Customization:** Recolor and resize.
*   **Batch Processing:** Automate multiple images.

</details>

<details>
<summary><strong>📄 PDF Processor</strong> - Toolkit for PDF processing needs 📄</summary>
<br>

Compress, merge, split, convert, and manage PDFs.

<div align="center">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/pdf-processor-screenshot.png" width="800">
</div>

**Key Features:**
*   **Versatile Toolkit:** Compress, merge, split, convert, and more.
*   **High-Quality Engine:** Powered by Ghostscript.
*   **Advanced Functionality:** Page organization, image extraction.
*   **Intuitive GUI:** Simple and fast.

</details>

<details>
<summary><strong>✨ AI Background Remover</strong> - One-click background removal ✨</summary>
<br>

Removes image backgrounds with a single click.

<div align="center">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/background-remover-screenshot.png" width="800">
</div>

**Key Features:**
*   **One-Click Removal:**
*   **Simple & Fast UI:**
*   **Live Previews:**
*   **GUI Logging:**

</details>

<details>
<summary><strong>🔠 Font Renamer Utility</strong> - Make font variations distinct 🔠</summary>
<br>

Modifies font metadata so that font variations (e.g., Bold, Narrow) appear as distinct font families.

<div align="center">
  <img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/font-renamer-screenshot.png" width="800">
</div>

**Key Features:**
*   **Batch Processing:** Process folders of fonts.
*   **Intelligent Renaming:**
*   **Detailed Reporting:**
*   **Automatic Backups:**

</details>

---

## 📧 Get In Touch
I'm open to discussing projects and collaborations! Let's connect.

[![Email](https://img.shields.io/badge/Email-d14836?style=flat-square&logo=gmail&logoColor=white)](mailto:gasdlarosa@gmail.com) gasdlarosa@gmail.com
