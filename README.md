# Workflow Automation

Tools for reducing repetitive vendor website lookup and spreadsheet data entry: a Python batch URL finder and a Windows AutoHotkey assistant.

## Projects

| Project | Purpose | Technology |
| --- | --- | --- |
| [Batch URL Finder](Fully%20Automated%20First%20Google%20Result%20Fetcher/Windows%3ALinux/) | Search company names from Excel and fill empty URL cells | Python, pandas, openpyxl, Tkinter |
| [Quick URL Fetcher](QuickURLFetcherHotkey/) | Assist vendor research across Excel and Chrome using hotkeys | AutoHotkey v1.1, Windows Excel |
| [Mac package notes](Fully%20Automated%20First%20Google%20Result%20Fetcher/Mac/) | Existing packaged version and usage notes | macOS application bundle |

## Business problem

Vendor records can contain missing or outdated website addresses. These tools support batch collection of candidate websites and human review with faster browser-to-spreadsheet entry. The hotkey assistant was created for a Valify workflow.

## Run the Python source

Requires Python with Tkinter and a desktop display. From the repository root:

```sh
cd "Fully Automated First Google Result Fetcher/Windows:Linux"
python -m venv .venv
# Activate the environment using the command for your shell.
python -m pip install pandas==2.2.3 openpyxl==3.1.5 google==3.0.0
python fullscript.py
```

Select a copy of an Excel workbook, enter its header row number (starting at 1), and provide the company-name and destination URL column names. Save and close the workbook before running. The script saves changes to the selected file; review the resulting URLs before using them.

## Design and limitations

- Uses a search-result URL as a candidate; it does not verify that it is the official company website.
- Searches each input row, then writes URLs only where destination cells are empty.
- Adds a randomized 2–5 second delay after each lookup; network/search latency adds to total time. Search availability and rate limits can interrupt a run.
- Prototype error handling is limited, including cancellation and very small workbooks. Use a workbook copy.
- The Python reader uses the first worksheet; the writer targets the active worksheet. Use a single-sheet workbook to avoid a mismatch.
- The legacy requirements.txt includes Mac packaging dependencies. The command above installs the libraries directly imported by the script.
- Windows:Linux is a legacy directory name containing a colon, which prevents a normal Windows checkout. Run the Python source from a compatible filesystem; the folder name needs a separate migration for Windows use.

See each project folder for its existing workflow instructions. These are historical utilities; current compatibility has not been revalidated.
