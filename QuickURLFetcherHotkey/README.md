# Automated Google Search Script

This script allows you to grab the most accurate URL for the company with only one click. Used to quickly update outdated or missing URLS in an Excel sheet. Created specifically for Valify.

## Prerequisites

### Step 1: Install AHK v1.1
To run the script, you need AutoHotkey v1.1 installed. You can download it from the following link:

[Download AutoHotkey v1.1](https://autohotkey.com/download/)

### Step 2: Download the Script
Download the `.ahk` file or copy the provided code into a new `.ahk` file using Notepad.

### Step 3: Running the Script
1. Once the script is downloaded or saved, simply double-click on the `.ahk` file to run it.
2. A tooltip will appear indicating the program is running, displaying the default hotkeys for your convenience.

## Features

This script provides the following functionality:

- **Excel Integration:**
  - Retrieves vendor data (Vendor ID, Name, Old URL, and Top Level Domain) from an Excel sheet.
  - Automatically populates the retrieved data into relevant fields in Chrome.

- **Google Chrome Integration:**
  - Automates navigation to specific tabs in Chrome.
  - Automatically opens vendor URLs and fetches relevant data.
  - Allows searching using multiple vendor-related fields (Vendor ID, Name, URL, and TLD).

## Hotkeys

### Default Hotkeys:
- `CapsLock`: Begin Search (Excel data is retrieved for processing).
- `XButton2`: Pick URL (When hovering over a URL in Chrome).
- `Middle Mouse Button (MButton)`: Get current URL from the site you're visiting.
- `XButton1`: Insert "?" into the URL field.

### Navigation in Chrome:
- `1`: Navigate to Tab 1.
- `2`: Navigate to Tab 2.
- `3`: Navigate to Tab 3.
- `4`: Navigate to Tab 4.

### Other Hotkeys:
- `Esc`: Exit the script.
- `~ (Tilde)`: Open the tutorial.
- `Ctrl + Alt + S`: Open the settings menu.
- `Shift + ~ (Tilde)`: Open the settings menu.

## Settings Configuration

The settings menu allows you to configure:

- **Target Monitor**: Select which monitor Chrome will open on.
- **Tab Number**: Select which tab Chrome should open.
- **Vendor ID Input**: Choose whether to automatically input Vendor ID in relevant fields.

### How to Access Settings:
1. Press `Ctrl + Alt + S` or `Shift + ~ (Tilde)` to open the settings menu.
2. In the settings window, you can configure the following:
   - **Monitor**: Specify the monitor number where Chrome will open.
   - **Tab Number**: Choose which tab Chrome should start on (1-4).
   - **Vendor ID**: Choose if you want to input Vendor ID automatically.

After making your changes, click **Save** to apply the settings.

## How It Works

1. **GetData**:
   - The script grabs vendor data (ID, Name, URL) from an open Excel sheet.
   - It then processes the data and performs a Google search.

2. **Search**:
   - The script searches for the vendor data in Google and performs further tasks like opening URLs and inputting the data into the relevant Chrome fields.

3. **newdata**:
   - Fetches data from Chrome, including hovering over URLs and grabbing the current URL or manually setting a "?" in the URL field.

4. **TextEnter**:
   - Automatically inputs data into the specified fields on the Chrome window.

5. **RunChrome**:
   - Opens a new Chrome window, maximizes it, and places it on the selected monitor.

## Error Handling

- If no Excel file is open, the script will show a message box asking you to open the file and go to the "New URL" field.
- If no URL is found during data extraction, a tooltip will prompt you to try again.

## Troubleshooting

1. **Excel Not Running**: The script requires an open Excel window with the vendor data. If Excel is not running, you will be prompted to open it.
2. **Chrome Window Not Found**: If the Chrome window is not active, the script will wait until it detects Chrome and proceed.

## Exit the Script

To exit the script at any time, simply press `Esc` on your keyboard.


For any questions or issues, feel free to reach out.
