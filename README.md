# Hi there, I'm Gaspar dela Rosa 👋

I'm a Python Developer specializing in building practical desktop applications and backend automation tools. My focus is on creating intuitive, user-friendly software that solves real-world challenges, from processing documents to integrating AI models for intelligent tasks.



---

## 🚀 Showcase Projects

Here are a few of my recent projects. The source code for these applications is kept in private repositories.

### ✒️ AI Signature Editor

> An intuitive desktop application designed to process signature images using an AI-powered background removal model. This tool allows users to quickly extract a signature from its background, recolor it, resize it to specific dimensions, and save it as a transparent PNG, perfect for digital documents.

![AI Signature Editor Screenshot](https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/e-signature-app-screenshot.png)

#### Key Features
-   **AI-Powered Background Removal:** Utilizes a Deep Image Segmentation model (`.onnx`) for accurate background extraction.
-   **Live Preview:** See the original and processed images side-by-side in real-time.
-   **Custom Colorization:** Recolor signatures to any color using a simple color picker.
-   **Precise Resizing:** Define exact output dimensions with an option to maintain aspect ratio.
-   **Batch Processing:** Process multiple signature images in a single operation.

#### Tech Stack
<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Tkinter-2C5985?style=for-the-badge&logo=python&logoColor=white" alt="Tkinter"/>
  <img src="https://img.shields.io/badge/ONNX-00594C?style=for-the-badge&logo=onnx&logoColor=white" alt="ONNX Runtime"/>
  <img src="https://img.shields.io/badge/Pillow-92447A?style=for-the-badge&logo=pillow&logoColor=white" alt="Pillow"/>
</p>

---

### 📄 PDF Processor

> A comprehensive toolkit for all PDF needs, powered by Ghostscript and Python. It can compress, merge, split, and convert PDF files through a simple user interface.

![PDF Processor Screenshot](https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/pdf-processor-screenshot.png)

#### Key Features
-   **Versatile Toolkit:** Compress, merge, split, convert, lock, unlock, and watermark PDFs.
-   **Efficient Processing:** Powered by the robust Ghostscript engine for high-quality results.
-   **User-Friendly GUI:** A simple and intuitive interface built with Tkinter.
-   **Extensive Functionality:** Includes page organization, image extraction, metadata editing, and more.

#### Tech Stack
<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Tkinter-2C5985?style=for-the-badge&logo=python&logoColor=white" alt="Tkinter"/>
  <img src="https://img.shields.io/badge/PyMuPDF-A41D1A?style=for-the-badge&logo=pypi&logoColor=white" alt="PyMuPDF"/>
  <img src="https://img.shields.io/badge/Ghostscript-000000?style=for-the-badge&logo=ghostscript&logoColor=white" alt="Ghostscript"/>
</p>

---

# ✨ AI Background Remover Utility

> A simple, fast, and functional desktop application that removes the background from images with a single click. Built with Python and Tkinter, it leverages the powerful `transparent-background` library for high-quality, AI-powered image segmentation.

![Background_Remover_Screenshot](https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/background-remover-screenshot.png)

---

## ✨ Features

-   **One-Click Removal:** Load an image and click one button to remove the background.
-   **Simple Interface:** A clean, compact, and functional UI designed for speed and ease of use.
-   **Live Previews:** See the original and the processed image side-by-side.
-   **Fast Workflow:** Includes "Save As..." and "Clear" buttons for efficient processing.
-   **GUI Logging:** View simple, real-time progress in the log panel.
-   **Organized File Logs:** Generates a new log file for each day in the `logs` directory.
-   **Dynamic Window Sizing:** Automatically adjusts to your screen for a comfortable fit.

---

## 🛠️ Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Tkinter-2C5985?style=for-the-badge&logo=python&logoColor=white" alt="Tkinter"/>
  <img src="https://img.shields.io/badge/Pillow-92447A?style=for-the-badge&logo=pillow&logoColor=white" alt="Pillow"/>
  <img src="https://img.shields.io/badge/transparent--background-000000?style=for-the-badge&logo=pypi&logoColor=white" alt="transparent-background"/>
</p>

---

## 🚀 Getting Started

Follow these steps to run the application on your local machine.

### Prerequisites

-   You must have **Python 3.8 or newer** installed on your system.
-   **Git** must be installed to clone the repository.

# Font Renamer Utility

<div align="center">

[![Python Version](https://img.shields.io/badge/python-3.6%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

A robust desktop tool to modify font metadata, ensuring every font variation appears as a distinct, top-level family in your OS and design software.

</div>

---

<div align="center">

*Replace this GIF with a screen recording of your application's workflow: Load -> Process -> View Details -> Save*
![Font Renamer Utility Demo](https://raw.githubusercontent.com/gasdlarosa/gasdlarosa/main/font-renamer-screenshot.png)

</div>

## The Problem

Operating systems like Windows often group font variations (e.g., `Arial Narrow`, `Arial Bold`) under a single parent family (`Arial`). While logical, this hides variations within style menus, making it cumbersome for designers, developers, and typographers who want to see every font as a distinct, easily accessible family.

This utility solves that problem by intelligently batch-processing your fonts and rewriting their metadata to force them to appear as standalone families.

## ✨ Key Features

*   🚀 **Batch Processing:** Load and process dozens of TrueType (`.ttf`) and OpenType (`.otf`) fonts in a single operation.
*   ⚙️ **Intelligent Renaming:** Automatically modifies all necessary name table entries for maximum compatibility across different operating systems and applications.
*   📊 **Detailed Reporting:** Review a comprehensive before-and-after report of all proposed metadata changes before committing to save the files.
*   ⏱️ **Real-time Feedback:** A live log panel, progress bar, and Estimated Time Remaining (ETR) calculator keep you informed during processing.
*   💾 **Automatic Backups:** For peace of mind, the utility automatically creates a timestamped backup of every original font file before processing.
*   🎨 **Modern UI:** A clean, responsive, and intuitive interface built with Tkinter's modern `ttk` themed widgets.

## 🚀 Getting Started

Get the application running on your local machine in two simple steps.

### Prerequisites

*   Python 3.6 or newer
*   The `fonttools` Python library

### Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/font-renamer-utility.git
    cd font-renamer-utility
    ```

2.  **Install dependencies:**
    The application relies on the `fonttools` library. Install it using pip:
    ```sh
    pip install fonttools
    ```

## 📖 Usage Guide

1.  **Launch the Application:**
    Run the `main.py` script from your terminal:
    ```sh
    python main.py
    ```

2.  **Load Fonts:**
    Click **`Load Font(s)`**. You can select multiple `.ttf` or `.otf` files. Backups of your original files will be created automatically in a `.font_backups` folder.

3.  **Process Fonts:**
    Click **`Process All Fonts`**. The application will analyze each font and generate new metadata. The UI will display real-time progress.

4.  **Review Changes (Recommended):**
    After processing, click **`View Batch Details`**. This opens a report comparing the original and proposed names for every font, allowing you to verify the changes.

5.  **Save Modified Fonts:**
    Click **`Save All Modified Fonts`** and choose an output directory. The new font files, with sanitized names, will be saved there.

6.  **Reset:**
    Click **`Reset`** to clear the application's state and start a new batch.

<br>

<details>
<summary><strong>🔬 The Technical Details: Renaming Logic & Codebase</strong></summary>

### How the Renaming Works

The utility's core logic is designed to trick an OS into un-grouping a font variation by making it a new, standalone family.

1.  **Create a New Family Name:** It combines the original family and subfamily names. For example, a font with Family=`"Inter"` and Subfamily=`"SemiBold"` becomes the new Family=`"Inter SemiBold"`.
2.  **Standardize the New Subfamily:** It sets the font's *new* subfamily to `"Regular"`.
3.  **Update All Name IDs:** This new `"Family"` and `"Subfamily"` data is written to all relevant name IDs within the font's internal name table (`nameID` 1, 2, 4, 16, 17, 21, 22) to ensure maximum compatibility across platforms and software.

The OS now sees a new font family called `"Inter SemiBold"` that has only one style: `"Regular"`. This forces it to be listed as a top-level font family.

### Codebase Structure

The project is organized into several key modules:

-   `main.py`: The main application entry point, containing the `FontRenamerApp` class which manages the GUI, state, and threading.
-   `processing/font_processor.py`: Contains the `FontProcessor` class, which handles all the low-level font file interactions using the `fonttools` library.
-   `dialogs/font_dialogs.py`: Helper functions for creating native-looking file and directory dialogs.
-   `utils/logging_config.py`: Sets up the application's logging configuration to direct output to the GUI.

</details>

## 📄 License

Distributed under the MIT License. See `LICENSE.txt` for more information.

## 📫 Get In Touch

If you'd like to chat about my projects or potential opportunities, feel free to reach out!

-   **Email:** `gasdlarosa@gmail.com`

