# 👋 Hi there! I'm Gaspar dela Rosa

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

*Private repositories showcasing my work.*

<details>
<summary><strong>⬇️ TikTok Media Downloader</strong> - Download videos from TikTok user profiles ⬇️</summary>
<br>

A user-friendly desktop application built with Python and Tkinter, designed to download videos and media from TikTok user profiles. It leverages the powerful `yt-dlp` backend, offering robust download capabilities, including support for authenticated (private/restricted) accounts via cookies, configurable download quality, flexible file naming, and advanced history management with crash-proof checkpointing.

<div align="center">
  <!-- TODO: Add a screenshot for TikTok Media Downloader -->
  <img src="https://via.placeholder.com/800x400?text=TikTok+Media+Downloader+Screenshot" width="800" alt="TikTok Media Downloader Screenshot">
</div>

**Key Features:**
*   **TikTok User Profile Downloads:** Download all available videos from a specified public or private TikTok user URL.
*   **Customizable Save Location:** Easily select your preferred output directory.
*   **Intuitive UI:** Clean and responsive interface inspired by modern design principles, powered by `ttkthemes`.
*   **Download Controls:** Start, Stop, and Reset download sessions.
*   **Real-time Progress & Status:**
    *   Overall progress bar for the entire download session.
    *   Detailed real-time status updates for the currently downloading video.
    *   Informative status bar messages for application state.
    *   Integrated session log for detailed activity and error reporting.
*   **Authenticated Downloads (Cookies.txt Support):** Download from private or restricted accounts by providing your browser's session cookies. Detailed instructions are provided within the app.
*   **Advanced Settings Dialog:**
    *   **Video Quality Selection:** Choose from presets like "Best," "1080p," "720p," "Worst quality," "Audio only," or input a custom `yt-dlp` format string.
    *   **File Naming Template:** Customize how downloaded files are named using `yt-dlp` placeholders (e.g., `%(uploader)s - %(title)s (%(id)s).%(ext)s`).
    *   **Embed Metadata:** Option to embed video metadata (title, description, upload date, etc.) and thumbnails directly into the downloaded video files (requires FFmpeg).
*   **Robust Download History Management:**
    *   **Load History:** Load existing history files to automatically skip previously downloaded videos.
    *   **Automatic History Update on Load:** When you load a history file, the application automatically merges it with its current knowledge and saves the *combined* history back to the loaded file, ensuring your history file is always up-to-date and comprehensive.
    *   **Checkpoint Auto-Save:** The application automatically saves its download history every **25 successful downloads** (hardcoded for stability and crash recovery), ensuring that progress is not lost due to unexpected crashes or interruptions.
    *   **Manual Save History:** Manually save the current session's download history to a JSON file.
*   **Download Session Report:** Get a clear summary of total videos found, successfully downloaded, skipped, and failed videos after each session.
*   **Open Output Folder:** Convenient prompt to open the download directory after a successful session.
*   **Logs Management:** Copy or clear the session log directly from the UI.
*   **Help & Info Sections:** In-app guides for usage, cookie setup, dependencies, and developer information.

**Getting Started:**

**Prerequisites:**
*   Python 3.8 or newer
*   `pip` (Python package installer)

**Installation:**
1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/your-username/tiktok-media-downloader.git
    cd tiktok-media-downloader
    ```
    *(Note: Replace `your-username` with the actual GitHub username if you fork the project.)*

2.  **Install Dependencies:**
    It's recommended to use a virtual environment.
    ```bash
    python -m venv venv
    # On Windows:
    venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate

    pip install -r requirements.txt
    ```
    If `requirements.txt` is not provided, manually install:
    ```bash
    pip install yt-dlp tk ttkthemes
    # Note: Tkinter is usually included with Python, but for some Linux distributions,
    # you might need to install it separately (e.g., `sudo apt-get install python3-tk`).
    ```
    `yt-dlp` itself handles FFmpeg installation on first use if not already present, but for robust metadata embedding and format conversion, having FFmpeg pre-installed and in your system's PATH is recommended.

**Running the Application:**

After installation and activating your virtual environment:

```bash
python main.py
</details>
<details>
<summary><strong>📷 AI Image Extractor</strong> - Crop portraits from scanned documents 📷</summary>
<br>
Automatically detects, de-skews, and crops portrait photos from scanned documents.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/image-extractor-screenshot.png" width="800">
</div>
Key Features:
AI Smart Cropping: YOLOv8 for optimal head room.
Automatic De-skew: OpenCV for perspective correction.
Multi-Format Support: Handles PDFs, Word docs, and images.
Intelligent Filenaming: Suggests names based on source.
</details>
<details>
<summary><strong>🔐 Password Cracker</strong> - Recover passwords from compressed archives 🔐</summary>
<br>
Comprehensive tool for password recovery from ZIP, RAR, and 7z archives.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/password-cracker-screenshot.png" width="800">
</div>
Key Features:
Multiple Attack Modes: SecLists, mask, hybrid, custom.
Advanced Options: Leet speak, keyword filtering.
Session Management: Save and load configurations.
Detailed Reporting: Statistics and password strength analysis.
</details>
<details>
<summary><strong>✒️ AI Signature Editor</strong> - Extract, recolor, and resize signatures ✒️</summary>
<br>
Extracts signatures, recolors them, and resizes them for digital documents.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/e-signature-app-screenshot.png" width="800">
</div>
Key Features:
AI Background Removal: Accurate extraction with Deep Image Segmentation.
Live Preview: View changes instantly.
Full Customization: Recolor and resize.
Batch Processing: Automate multiple images.
</details>
<details>
<summary><strong>📄 PDF Processor</strong> - Toolkit for PDF processing needs 📄</summary>
<br>
Compress, merge, split, convert, and manage PDFs.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/pdf-processor-screenshot.png" width="800">
</div>
Key Features:
Versatile Toolkit: Compress, merge, split, convert, and more.
High-Quality Engine: Powered by Ghostscript.
Advanced Functionality: Page organization, image extraction.
Intuitive GUI: Simple and fast.
</details>
<details>
<summary><strong>✨ AI Background Remover</strong> - One-click background removal ✨</summary>
<br>
Removes image backgrounds with a single click.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/background-remover-screenshot.png" width="800">
</div>
Key Features:
One-Click Removal:
Simple & Fast UI:
Live Previews:
GUI Logging:
</details>
<details>
<summary><strong>🔠 Font Renamer Utility</strong> - Make font variations distinct 🔠</summary>
<br>
Modifies font metadata so that font variations (e.g., Bold, Narrow) appear as distinct font families.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/font-renamer-screenshot.png" width="800">
</div>
Key Features:
Batch Processing: Process folders of fonts.
Intelligent Renaming:
Detailed Reporting:
Automatic Backups:
</details>
📧 Get In Touch
I'm open to discussing projects and collaborations! Let's connect.
![alt text](https://img.shields.io/badge/Email-d14836?style=flat-square&logo=gmail&logoColor=white)
code
Code
Use Arrow Up and Arrow Down to select a turn, Enter to jump to it, and Escape to return to the chat.
Start typing a prompt

Run
Ctrl
1




65536
0.95
