# Twitter Name Spotter

## Description

This browser extension processes Twitter names to find candidate names (first and last names) within tweet or profile text. If a candidate name is found in a predefined JSON list (e.g., "GEORGE SOROS"), it replaces that candidate with a formatted string (e.g., `($(George Soros)$)`). It works on both Chrome/Brave and Firefox and uses a MutationObserver to handle dynamically loaded content on Twitter.

## Features

- **Name Lookup:** Loads a JSON file containing a list of names (all in uppercase for consistency) and uses a fast lookup set.
- **Dynamic Processing:** Processes Twitter elements (using specific CSS selectors) to find and replace candidate names in real time.
- **Formatted Output:** Replaces candidate names with a formatted string `($(Candidate Name)$)`.
- **Mutation Observer:** Automatically processes new content loaded dynamically on Twitter.
- **Cross-Browser Compatibility:** Works on Chrome/Brave and Firefox.

## Warning & Important Notes

- **Manual Installation Required:**  
  If you install the extension using the provided `.crx` file (Chrome/Brave) or by loading the unpacked extension, you must enable Developer Mode in your browser’s extensions page.
  
- **Installation Restrictions:**  
  Chrome and Brave may warn users about installing extensions from outside the official Web Store. Users may need to bypass these warnings in Developer Mode.
  
- **No Automatic Updates:**  
  When distributing the extension as a `.crx` file, users will not receive automatic updates. You will need to distribute new versions, and users must reinstall the updated extension manually.
  
- **Security & Trust:**  
  Only install extensions from trusted sources. This extension is provided as open-source software for testing and personal use.

- **Testing:**  
  It is recommended to thoroughly test the extension on your browser version since updates to Twitter’s design or browser changes may affect functionality.

## Installation

### For Chrome/Brave

#### Load Unpacked (for Development or Testing)

1. **Clone or Download:**  
   Clone this repository or download the ZIP file and extract it.

2. **Open Extensions Page:**  
   Go to `chrome://extensions/` (for Chrome) or `brave://extensions/` (for Brave).

3. **Enable Developer Mode:**  
   Toggle the **Developer mode** switch in the top right corner.

4. **Load Unpacked Extension:**  
   Click on **Load unpacked** and select the folder containing the extension files (the folder with `manifest.json`, `content.js`, and `clean_official_names.json`).

5. **Test the Extension:**  
   Navigate to Twitter to see the extension in action.

#### Install Using the .crx File (Direct Distribution)

1. **Obtain the .crx File:**  
   Download the packaged `.crx` file from this repository’s releases.

2. **Open Extensions Page:**  
   Go to `chrome://extensions/` (for Chrome) or `brave://extensions/` (for Brave).

3. **Enable Developer Mode:**  
   Make sure Developer Mode is enabled.

4. **Drag and Drop the .crx File:**  
   Drag and drop the `.crx` file onto the extensions page.

5. **Follow Prompts:**  
   Accept any prompts or warnings to complete the installation.

### For Firefox

#### Load Temporary Add-on (for Testing)

1. **Clone or Download:**  
   Clone this repository or download the ZIP file and extract it.

2. **Open Firefox Debugging Page:**  
   Type `about:debugging` in the address bar.

3. **Load Temporary Add-on:**  
   Click **This Firefox** (or **Add-ons Debugging**) and then click **Load Temporary Add-on…**.  
   Select the `manifest.json` file from the extension folder.

4. **Test the Extension:**  
   Navigate to Twitter to verify that the extension works as expected.

#### Permanent Installation

1. **Package the Extension:**  
   Zip the contents of the repository (make sure that `manifest.json` is at the root of the ZIP).

## Updating the Extension

- **Chrome/Brave:**  
  If you install via the Chrome Web Store, updates will be automatic. For manually installed `.crx` files, users must reinstall the updated version.
  
- **Firefox:**  
  Updates for published add-ons on AMO are handled by Mozilla. For temporary add-ons, you must reload the extension after making changes.

## Contributing

Contributions are welcome! Please submit issues or pull requests for improvements, bug fixes, or additional features.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

For any questions, issues, or suggestions, please open an issue in this repository or contact the maintainer.

