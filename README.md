# Zoom Update Script

This script automates the process of checking, downloading, and updating Zoom to its latest version on Linux.

## Overview

The script performs the following tasks:
1. Checks for the latest Zoom `.deb` package.
2. Compares the currently installed Zoom version with the latest available version.
3. Updates Zoom if a new version is found.

## Prerequisites

- **Operating System**: Linux (Debian-based distributions like Ubuntu)
- **Dependencies**: `wget`, `dpkg`

## How to Use

1. Place this script in your preferred directory.
2. Make the script executable:
   ```bash
   chmod +x update_zoom.sh
   ```
3. Run the script:
   ```bash
   ./update_zoom.sh
   ```

The script will check if a new version of Zoom is available. If an update is found, it will download and install the latest `.deb` package.

## Explanation of Script Components

- **Download and Check Version**: Downloads the latest `.deb` file from Zoom’s server.
- **Version Comparison**: Uses `dpkg` to compare the currently installed Zoom version with the downloaded version.
- **Automatic Update**: If a new version is available, the script installs it using `sudo dpkg -i`.

## Notes

- **Permissions**: The script requires `sudo` privileges to install the new version of Zoom.
- **Download Directory**: By default, the script saves the Zoom `.deb` file in `~/Downloads/Install/Software`. Update this path if needed.

## License

This script is licensed under the [MIT License](LICENSE).

--- 

This README provides clear instructions and explanations for anyone looking to use or understand your Zoom update script.