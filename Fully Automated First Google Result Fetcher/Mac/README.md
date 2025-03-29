## Project - URL Finder Script  



### 1. Download & Install  
- Download the application from this Google Drive link:  
  [Download URL Finder Script](https://drive.google.com/file/d/1KBZtivp806hT2y3uFfhFOyPYrdydGgY0/view?usp=sharing)  
- Double-click the downloaded `.zip` file to unzip it.  
- Move the **"URL Finder Script.app"** to your **Applications** folder or desired location.  

### 2. First-Time Setup (Important Security Steps)  
1. Locate **"URL Finder Script.app"** in Finder.  
2. Right-click (or **Control + Click**) on the app.  
3. Select **"Open"** from the menu.  
4. When you see the security warning:  
   *"URL Finder Script.app cannot be opened because it is from an unidentified developer."*  
   - Click **"Open"** again to bypass this restriction.  

### 3. Additional Permissions  
- The app may request permissions for:  
  - File access (for reading/writing Excel files)  
  - Network access (for Google searches)  
- Click **"Allow"** when prompted.  
- After completing these steps, the app should run normally.  
- You can now open it by double-clicking in the future.  

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
- Each search takes **3-5 seconds** (intentionally slowed to avoid Google’s anti-bot measures).  
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
