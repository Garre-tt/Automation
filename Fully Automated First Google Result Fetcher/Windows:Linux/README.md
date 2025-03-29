# Project - URL Finder Script

### 1. Download & Install
- Download the application files from this Google Drive link: [Download URL Finder Script](https://drive.google.com/file/d/1KBZtivp806hT2y3uFfhFOyPYrdydGgY0/view?usp=sharing)
- Double-click the downloaded `.zip` file to unzip it.
- Navigate to the extracted folder containing the script files.

### 2. Setup Python Environment
1. Ensure Python 3.12 is installed on your system.
2. Open a terminal or command prompt in the script folder.
3. Install the required dependencies by running
```pip install -r requirements.txt```

### 3. Running the Script
- Execute the script from the terminal/command prompt:
``` python url_finder.py ```

### 4. Using the App
#### Important: Before Starting
- Save and close the Excel sheet you want to process.
- Ensure your computer does not go to sleep during the process.

#### Running the Script
When you start the app, you'll need to provide:
- The Excel file you want to process.
- The header row number (example: if column names are in row 2, enter **"2"**).
- The column name containing company names.
- The column name where URLs should be added.

#### Important Notes
- The app **will not** overwrite existing URLs in filled cells.
- Each search takes **3-5 seconds** (intentionally slowed to avoid Google's anti-bot measures).
- You can use your computer normally while it runs, but:
- Do not close the application.
- Do not open the Excel file being processed.
- The app will close automatically when finished.

### 5. Limitations
- The script selects the **first URL** from Google search results.
- This means some results may be:
- Yelp listings
- Directory pages
- Social media profiles
- Instead of official company websites
- Manual verification of URLs may be required.

---
*This script was designed to automate the process of finding company URLs. Feel free to modify or extend it to suit your needs.*
