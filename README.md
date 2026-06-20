# OCR PDF to Word Converter

A Windows GUI application that converts scanned PDFs into editable Word (.docx) documents using EasyOCR.

![screenshot](screenshot.png)

## Features

- Select any PDF file via a simple GUI
- Converts PDF pages to images using Poppler
- Performs OCR with EasyOCR (English)
- Saves output as a formatted Word document (.docx)
- Progress bar and status updates
- Standalone executable available (no Python required)

## Downloads

Pre-built Windows executables are available on the [Releases](https://github.com/YOUR_USERNAME/YOUR_REPO/releases) page. Just download, unzip, and run `ocr_gui_app.exe`.

## Requirements (for running from source)

- Python 3.8+
- [Poppler for Windows](https://github.com/oschwartz10612/poppler-windows/releases) (included in the `poppler/` folder)

## Installation (from source)

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO

# Create a virtual environment (optional but recommended)
python -m venv venv
.\venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the app
python ocr_gui_app.py
```

## Building the executable

```bash
pip install pyinstaller
pyinstaller ocr_gui_app.spec
```

The standalone executable will be in `dist/ocr_gui_app/`.

## How to use

1. Click **Upload PDF** to select a scanned PDF
2. Click **Select Save Location** to choose where to save the .docx
3. Click **Start OCR** to begin conversion
4. Wait for the progress bar to complete

## License

This project is licensed under the **GNU General Public License v3.0**. See [LICENSE](LICENSE).

The included Poppler binaries are GPL-licensed (see `poppler/README-poppler.txt`).
