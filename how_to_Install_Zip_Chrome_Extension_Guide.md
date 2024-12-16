## Guide to Loading CaptchaSonic Chrome and Firefox Extensions

---
[![How to Load Extensions from zip on Chrome](https://img.youtube.com/vi/yVvvA8kaIuk/0.jpg)](https://www.youtube.com/watch?v=yVvvA8kaIuk)


## Table of Contents

1. [Loading Extensions in Google Chrome](#loading-extensions-in-google-chrome)
2. [Loading Extensions in Mozilla Firefox](#loading-extensions-in-mozilla-firefox)

---

## Loading Extensions in Google Chrome

Follow these steps to load a Chrome extension from your local files:

### Step 1: Open Chrome’s Extensions Page

- Open Google Chrome and navigate to the Extensions page.
- You can do this by typing `chrome://extensions` in the address bar and pressing Enter.

![Step 1 Image Placeholder](image_placeholder_1)

### Step 2: Enable Developer Mode

- At the top right of the Extensions page, toggle the "Developer mode" switch to ON.

![Step 2 Image Placeholder](image_placeholder_2)

### Step 3: Load Unpacked Extension

- Click the **Load unpacked** button.
- A file dialog will appear, prompting you to select a folder.
- Navigate to the folder containing the extension you want to load.

![Step 3 Image Placeholder](image_placeholder_3)

### Step 4: Select the Extension Folder

- Select the folder that contains your extension files. Ensure the folder contains the `manifest.json` file, which is required for the extension to load correctly.

![Step 4 Image Placeholder](image_placeholder_4)

### Step 5: The Extension Is Now Loaded

- After selecting the folder, the extension will be loaded, and you should see it listed on the Extensions page in Chrome.

![Step 5 Image Placeholder](image_placeholder_5)

---

## Loading Extensions in Mozilla Firefox

Follow these steps to load a Firefox extension from your local files:

### Step 1: Open Firefox’s Add-ons Manager

- Open Mozilla Firefox and click on the three horizontal lines (hamburger menu) in the upper-right corner.
- Select **Add-ons and themes** to open the Add-ons Manager.

![Step 1 Image Placeholder](image_placeholder_6)

### Step 2: Open the Extensions Section

- In the Add-ons Manager, select the **Extensions** tab from the left sidebar.

![Step 2 Image Placeholder](image_placeholder_7)

### Step 3: Enable Developer Mode

- Scroll down and click on **"More"** (three dots) on the upper-right corner of the Extensions section.
- From the dropdown, select **"Install Add-on From File"**.



![Step 3 Image Placeholder](image_placeholder_8)

### Step 4: Select the Extension File

- A file dialog will appear. Locate and select the `.xpi` file for your extension.
- Alternatively, if you're testing a folder-based extension, you can use the Firefox Developer Tools to load it manually.

![Step 4 Image Placeholder](image_placeholder_9)

### Step 5: The Extension Is Now Loaded

- After installation, the extension will appear in the list of installed extensions and should be ready to use.

![Step 5 Image Placeholder](image_placeholder_10)

---

## Troubleshooting

### Chrome

- **"Manifest file is missing" error:** Ensure that the folder you selected contains the `manifest.json` file. Without it, Chrome cannot load the extension.
- **Extension doesn't work as expected:** Try reloading the extension by clicking the refresh icon on the Extensions page.

### Firefox

- **"This add-on could not be installed because it appears to be corrupt":** Ensure that the `.xpi` file is valid. If you're loading an unpacked extension, ensure that it is properly packaged before trying again.
- **Extension doesn't appear after installation:** Try restarting Firefox or clearing cache data.

---

## Conclusion

Loading extensions manually in Chrome and Firefox is a great way to test new features or troubleshoot your own extensions. With the steps outlined above, you should be able to load any unpacked or locally stored extension in both browsers.

For further assistance or if you encounter issues, feel free to consult the official documentation for [Chrome Extensions](https://developer.chrome.com/docs/extensions/) and [Firefox Add-ons](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons).
