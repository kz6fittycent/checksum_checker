# Checksum Checker

A simple GUI application to verify and generate checksums for files on Linux.

## Features
- Verify file checksums using various algorithms (e.g., md5, sha256).
- Generate checksums for local files.
- User-friendly interface with algorithm dropdown and file browser.
- Color-coded output (green for success, red for failure).
- Icons for visual feedback (checkmark for success, stop sign for errors).
- Option to check another file or exit.

## Installation

   `sudo snap install checksum_checker`

## Build and run locally
1. Clone or download the repository.
2. Navigate to the project directory.
3. Run `pip install -r requirements.txt` to install PyQt6.
4. Launch the application with `python3 checksum_checker_gui.py`.

## Requirements
- Python 3.x
- Install dependencies with: `pip install -r requirements.txt`

## Usage
1. Select or enter a file path using the "Browse" button.
2. Choose an algorithm from the dropdown menu.
3. For verification, enter an expected checksum and click "Verify Checksum".
4. To generate a checksum, click "Generate Checksum".
5. View the result in the output area.
6. Click "Check Another File" to reset or "Exit" to close.

## License
[MIT License]
