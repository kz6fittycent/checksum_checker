[![🧪 Snap Builds](https://github.com/kz6fittycent/checksum_checker/actions/workflows/test-snap-can-build.yml/badge.svg)](https://github.com/kz6fittycent/checksum_checker/actions/workflows/test-snap-can-build.yml)

# Checksum Checker

A simple GUI application to verify and generate checksums for files on Linux.

## Features
- Verify file checksums using various algorithms (e.g., md5, sha256).
- Generate checksums for local files.
- User-friendly interface with algorithm dropdown and file browser.
- Color-coded output (green for success, red for failure).
- Icons for visual feedback (checkmark for success, stop sign for errors).
- Option to check another file or exit.

## Preferred Installation Methods

### Checksum Checker is also distributed as a `.deb` package for Ubuntu-based distributions. Follow these steps to install:

1. **Download the Package**  
   Download the latest `.deb` file from the [releases page](https://github.com/kz6fittycent/checksum_checker/releases).

2. **Install the Package**  
   Install the `.deb` file using the following commands:
   ```bash
   sudo dpkg -i checksumchecker_1.0-1_all.deb
   sudo apt-get install -f
   ```
   - The `apt-get install -f` command resolves any missing dependencies.

3. **Dependencies**  
   - On Ubuntu 24.04, `python3-pyqt6 (>= 6.9.1)` is available in the default repositories and should install automatically.
   - On Ubuntu 22.04: `pip3 install PyQt6==6.9.1`


4. **Launch the Application**  
   - From the terminal: `checksum_checker`
   - Or find "Checksum Checker" in your application menu.

For issues or feedback, please visit [https://github.com/kz6fittycent/checksum_checker/issues](https://github.com/kz6fittycent/checksum_checker/issues).

### A snap is coming soon!

To install the snap:

   `sudo snap install checksum_checker`

([Don't have snapd installed?](https://snapcraft.io/docs/core/install))

## Build and run locally
1. Clone or download the repository.
2. Navigate to the project directory.
3. Run `pip install -r requirements.txt` to install PyQt6.
4. Launch the application with `python3 checksum_checker`.
5. Set the script as executable with: `chmod +x checksum_checker`
6. Move it to a location to be reused often (e.g. `/usr/local/bin`)

## Requirements
- Python 3.x
- Install dependencies with: `pip install -r requirements.txt`
- If using the snap, just ensure you have `snapd` [installed](https://snapcraft.io/docs/core/install). 

## Usage
1. Select or enter a file path using the "Browse" button.
2. Choose an algorithm from the dropdown menu.
3. For verification, enter an expected checksum and click "Verify Checksum".
4. To generate a checksum, click "Generate Checksum".
5. View the result in the output area.
6. Click "Check Another File" to reset or "Exit" to close.

![image](https://github.com/user-attachments/assets/f9ac9539-7ed6-4edd-8170-a88861646fd4)

![image](https://github.com/user-attachments/assets/c1f01d26-2010-4314-ae83-805bec80916a)

![image](https://github.com/user-attachments/assets/b75a13d1-1bda-4137-8fa3-808f930ba658)



## Credits

This was an experiment with [Grok3](https://grok.com/) that went quite well. I am still working on the snap, but Grok3 created the application itself based on my prompts. Grok also helped with the `.deb`.

## License
[MIT License](https://github.com/kz6fittycent/checksum_checker/blob/main/LICENSE)
