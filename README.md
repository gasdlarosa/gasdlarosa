<div align="center">
Hi there, I'm Gaspar dela Rosa 👋
Python Developer focused on building intuitive desktop applications and intelligent automation tools.
<img src="https://img.shields.io/badge/Email-d14836?style=for-the-badge&logo=gmail&logoColor=white" />
</div>
🛠️ Core Technologies
<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/Tkinter-2C5985?style=for-the-badge&logo=python&logoColor=white" alt="Tkinter"/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
<img src="https://img.shields.io/badge/Transformers-FFD700?style=for-the-badge&logo=hugging-face&logoColor=black" alt="Transformers"/>
<img src="https://img.shields.io/badge/PRAW-FF4500?style=for-the-badge&logo=reddit&logoColor=white" alt="PRAW"/>
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV"/>
<img src="https://img.shields.io/badge/Pillow-92447A?style=for-the-badge&logo=pillow&logoColor=white" alt="Pillow"/>
<img src="https://img.shields.io/badge/Ultralytics-2A3DA4?style=for-the-badge&logo=yolo&logoColor=white" alt="Ultralytics YOLO"/>
<img src="https://img.shields.io/badge/ONNX-00594C?style=for-the-badge&logo=onnx&logoColor=white" alt="ONNX Runtime"/>
<img src="https://img.shields.io/badge/FFmpeg-007800?style=for-the-badge&logo=ffmpeg&logoColor=white" alt="FFmpeg"/>
<img src="https://img.shields.io/badge/PyMuPDF-A41D1A?style=for-the-badge&logo=pypi&logoColor=white" alt="PyMuPDF"/>
<img src="https://img.shields.io/badge/Ghostscript-000000?style=for-the-badge&logo=ghostscript&logoColor=white" alt="Ghostscript"/>
<img src="https://img.shields.io/badge/FontTools-4C4C4C?style=for-the-badge&logo=pypi&logoColor=white" alt="FontTools"/>
</p>
🚀 Showcase Projects
The source code for these applications is kept in private repositories.
<br>
<details>
<summary><strong>🔞 Reddit NSFW Extractor &nbsp;-&nbsp; Downloads and automatically classifies media from any subreddit.</strong></summary>
<br>
A desktop GUI application built with Python and Tkinter for downloading and automatically classifying media (images, gifs, videos) from any subreddit. It features two powerful extraction modes, session management, and intelligent sorting of content into NSFW and SFW folders.
<div align="center">
<img src="" width="800">
<!-- Note: Replace with an actual screenshot of the application -->
</div>
Key Features:
AI-Powered NSFW Classification: Utilizes a Transformers model to automatically sort downloaded images into nsfw and sfw folders.
Two Powerful Extraction Modes: A standard mode for a set number of posts and a time-based mode to bypass Reddit's 1000-post API limit.
Comprehensive Media Support: Downloads images, GIFs, and videos from Reddit, Imgur, RedGifs, and Gfycat.
Session & History Management: Save and load sessions, and maintain a download history to prevent duplicate downloads.
Automatic Video/Audio Merging: Uses FFmpeg to merge separate video and audio streams from Reddit-hosted videos.
</details>
<details>
<summary><strong>📷 AI Image Extractor &nbsp;-&nbsp; Automatically crops portraits from scanned documents.</strong></summary>
<br>
An intelligent desktop utility that uses a YOLOv8 model to automatically detect, de-skew, and extract perfectly cropped portrait photos from scanned documents (.pdf, .docx) and images.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/image-extractor-screenshot.png" width="800">
</div>
Key Features:
AI-Powered Smart Cropping: Utilizes a YOLOv8 model to calculate the ideal crop with proper headroom.
Automatic De-skew & Straighten: Corrects the perspective of skewed photos using OpenCV.
Multi-Format Support: Processes images, PDFs, and Word documents to find all embedded photos.
Intelligent Filenaming: Suggests logical filenames based on the original source document.
</details>
<details>
<summary><strong>🔐 Password Cracker &nbsp;-&nbsp; Versatile password recovery tool for compressed archives.</strong></summary>
<br>
A comprehensive desktop application for recovering lost passwords from ZIP, RAR, and 7z archives. Features multiple attack methods including dictionary attacks using SecLists wordlists, mask attacks for known patterns, and hybrid combinations with real-time progress monitoring.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/password-cracker-screenshot.png" width="800">
</div>
Key Features:
Multiple Attack Modes: SecLists integration, mask attacks, combination attacks, and custom wordlists.
Advanced Options: Keyword filtering, leet speak transformations, and hybrid enhancements.
Session Management: Save and load attack configurations for repeated use.
Detailed Reporting: Generate comprehensive reports with attack statistics and password strength analysis.
</details>
<details>
<summary><strong>✒️ AI Signature Editor &nbsp;-&nbsp; Desktop app to extract, recolor, and resize signatures from images.</strong></summary>
<br>
An intuitive desktop application that processes signature images using an AI-powered background removal model. This tool allows users to quickly extract a signature, recolor it, resize it to specific dimensions, and save it as a transparent PNG for use in digital documents.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/e-signature-app-screenshot.png" width="800">
</div>
Key Features:
AI Background Removal: Utilizes a Deep Image Segmentation model (.onnx) for accurate extraction.
Live Side-by-Side Preview: Instantly view changes as you edit.
Full Customization: Recolor signatures with a color picker and resize to exact dimensions.
Batch Processing: Automate the editing of multiple signature images at once.
</details>
<details>
<summary><strong>📄 PDF Processor &nbsp;-&nbsp; A comprehensive toolkit for all PDF processing needs.</strong></summary>
<br>
A robust desktop utility for all common PDF tasks, powered by the Ghostscript and PyMuPDF engines. It provides a simple user interface to compress, merge, split, convert, and manage PDF files efficiently.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/pdf-processor-screenshot.png" width="800">
</div>
Key Features:
Versatile Toolkit: Compress, merge, split, convert, lock, unlock, and watermark PDFs.
High-Quality Engine: Powered by Ghostscript for reliable and efficient processing.
Advanced Functionality: Includes page organization, image extraction, and metadata editing.
Intuitive GUI: A clean and simple interface built for speed and ease of use.
</details>
<details>
<summary><strong>✨ AI Background Remover &nbsp;-&nbsp; One-click background removal for any image.</strong></summary>
<br>
A simple, fast, and functional desktop application that removes the background from images with a single click. Built with Python and Tkinter, it leverages a powerful AI model for high-quality, clean results.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/background-remover-screenshot.png" width="800">
</div>
Key Features:
One-Click Removal: Load an image and click one button to remove the background.
Simple & Fast UI: A clean, compact interface designed for an efficient workflow.
Live Previews: Instantly see the original and the processed image side-by-side.
GUI Logging: View simple, real-time progress updates in the log panel.
</details>
<details>
<summary><strong>🔠 Font Renamer Utility &nbsp;-&nbsp; A tool to make font variations appear as distinct families.</strong></summary>
<br>
A robust desktop tool that solves the problem of font variations (e.g., "Bold," "Narrow") being grouped under a single parent family in operating systems. It intelligently modifies font metadata to force each variation to appear as its own top-level font family.
<div align="center">
<img src="https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/font-renamer-screenshot.png" width="800">
</div>
Key Features:
Batch Processing: Process entire folders of .ttf and .otf fonts at once.
Intelligent Renaming: Automatically modifies all necessary name table entries for maximum compatibility.
Detailed Reporting: Review a full report of all metadata changes before saving.
Automatic Backups: Creates timestamped backups of original font files for safety.
</details>
📫 Get In Touch
I'm always open to discussing new projects or collaboration opportunities. Feel free to reach out.
Email: gasdlarosa@gmail.com
