---

## 🚀 Featured Projects

<details>
<summary><strong>⬇️ 4K YT Downloader (with Authentication)</strong> - Download YouTube content with role-based authentication ⬇️</summary>
<br>

A modern, cross-platform GUI application built with Python and CustomTkinter for downloading YouTube content. It utilizes `yt-dlp` for core downloading and `ffmpeg` for media processing, and features an integrated role-based authentication system.

This version is simplified for ease of use, focusing on producing universally compatible media files.

## Features

*   **Role-Based Authentication:** Secure login for Administrator and Operator roles using `bcrypt` and an embedded SQLite database.
*   **Intuitive & Simple GUI:** Built with CustomTkinter (CTK) for a modern aesthetic. The interface is streamlined for a simple workflow.
*   **One-Click Downloads:**
    *   **Video:** Downloads the highest available quality and automatically converts it into a universally compatible **MP4 (H.264/AAC)** file.
    *   **Audio:** Downloads the best audio available and converts it to **MP3**.
*   **Playlist Support:** Automatically detects playlists and downloads all items sequentially.
*   **Progress Tracking:** Real-time download and post-processing status.
*   **User Management (Admin Only):** Administrators can register and delete Operator accounts.
*   **Logging:** In-app log viewer for troubleshooting.

## Prerequisites

To run this application, you need Python and several packages, as well as the external utility `FFmpeg`.

1.  **Python 3.x:** Download and install from [python.org](https://www.python.org/downloads/).
2.  **FFmpeg:** This is **critical** for converting and merging video/audio.
    *   Download from [ffmpeg.org](https://ffmpeg.org/download.html).
    *   **Installation:** You must ensure the `ffmpeg` executable is accessible from your system's PATH.

## Installation and Setup

1.  **Clone the Repository (Optional) or Save Files:**
    Create a project folder and save all the provided `.py` files inside it. Create subfolders `processing` and `utils` and place the respective files inside them.

2.  **Install Required Python Packages:**
    Open a terminal or command prompt in your project folder and run:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Run the Application:**
    ```bash
    python main.py
    ```

2.  **Initial Administrator Setup:**
    *   On the first run, the database is created. The administrator account is created upon the first login attempt.
    *   Select the **Administrator** role.
    *   Enter the fixed PIN: **`116898`**
    *   The application will create the administrator account and log you in.

3.  **Administrator Actions:**
    *   Once logged in, the Administrator can access **File -> Account Registration** to create new **Operator** users.
    *   Use **File -> User Management** to view and delete existing Operator accounts.

4.  **Operator Login:**
    *   Select the **Operator** role.
    *   Enter the username and PIN created by the administrator.

5.  **Downloading Content:**
    *   Paste a YouTube URL into the entry field.
    *   Click **Fetch**.
    *   Once the video/playlist information appears, click either **Download Video (MP4)** or **Download Audio (MP3)**.

</details>

<details>
<summary><strong>⚙️ Windows Component Registrar (DLL & OCX)</strong> - Smart batch script for registering COM components ⚙️</summary>
<br>

A robust and user-friendly batch script for automatically registering COM components (`.dll` and `.ocx` files) on Windows. It intelligently handles administrator privileges and 32/64-bit compatibility issues, making it a reliable tool for developers, IT professionals, and power users.

## Overview

Registering legacy DLL and OCX components on modern Windows systems can be a tedious and error-prone task. This script automates the entire process. It ensures that the correct registration tools are used, handles required permissions gracefully, and provides a clear summary of its actions.

## Key Features

-   **✅ Automatic Administrator Elevation**: The script detects if it's running without administrative privileges and will automatically prompt for elevation via the User Account Control (UAC) dialog.
-   **⚙️ Smart 32/64-bit Compatibility**: On 64-bit versions of Windows, it automatically uses the 32-bit version of `regsvr32.exe` from the `SysWOW64` directory. This is crucial for ensuring compatibility with older 32-bit components.
-   **🔍 Pre-registration Check**: To improve efficiency and prevent unnecessary operations, the script first checks the Windows Registry to see if a component is already registered.
-   **📂 Batch Processing**: Simply drop all your `.dll` and `.ocx` files into the `components` subfolder, and the script will process them all in one go.
-   **📊 Detailed Summary Report**: After execution, a final report is displayed, showing how many components were successfully registered, how many were already registered, and how many failed.
-   **📜 User-Friendly Instructions**: The script starts by displaying clear, concise instructions, ensuring the user understands the prerequisites and process before any action is taken.

## Prerequisites

-   Windows Vista or newer (due to the UAC elevation method).
-   The `.dll` and `.ocx` files you wish to register.

## How to Use

1.  **Download:** Clone this repository or download the `register_components.bat` file.

2.  **Create the Directory Structure:**
    -   Place the `register_components.bat` file in a folder of your choice.
    -   In that same folder, create a new subfolder and name it exactly `components`.

3.  **Add Components:**
    -   Copy all the `.dll` and `.ocx` files that you need to register into the newly created `components` folder.

    Your folder structure should look like this:

    ```
    └── MyProject/
        ├── register_components.bat
        └── components/
            ├── component1.dll
            ├── component2.ocx
            ├── another.dll
            └── ...
    ```

4.  **Run the Script:**
    -   Double-click the `register_components.bat` file.
    -   A command prompt window will appear with instructions. Press any key to continue.

5.  **Approve UAC Prompt:**
    -   A **User Account Control (UAC)** prompt will appear asking for administrator privileges. You **MUST** click "Yes" for the script to function correctly.
    -   The script will then proceed to register all the components and will display the final summary when finished.

## Understanding the Output

The script provides real-time feedback as it processes each file. The final summary is broken down into three categories:

-   **Successfully Registered**: The number of new components that were registered without errors.
-   **Already Registered**: The number of components that were skipped because they were already present in the Windows Registry.
-   **Failed to Register**: The number of components that could not be registered. This can happen if a file is not a valid COM component, is corrupt, or is missing its own dependencies.

## Troubleshooting

If a component fails to register, consider the following:

-   **Missing Dependencies**: The `.dll` or `.ocx` may depend on other libraries that are not present on the system. Use a tool like "Dependency Walker" to check for missing dependencies.
-   **Corrupt File**: The component file itself may be corrupted or incomplete. Try re-downloading or obtaining a fresh copy.
-   **Not a Registrable Component**: Not all `.dll` files are COM components and therefore cannot be registered with `regsvr32.exe`. The file must export the `DllRegisterServer` function.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Disclaimer

This script modifies the Windows Registry. While it is designed to be safe, you should always use it with care. The author is not responsible for any damage to your system. Always ensure you have backups of important data.
</details>

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
