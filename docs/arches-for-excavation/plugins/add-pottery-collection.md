## Add Pottery Collection

This workflow allows you to upload a spreadsheet (CSV or XLSX) containing pottery data and automatically generate a Pottery Collection resource, linking it directly to a specific Context resource in your database.

---

### Step 1: Select Context

The first step requires you to identify the specific Context resource that the uploaded pottery collection belongs to.

*   **Search for a Context:** Use the **"Search for an (O) Context resource..."** input bar at the top to filter the available records.
*   **Select a Context:** The matching resources will be displayed as clickable cards. Click on the card representing the correct Context.
*   **Confirm Selection:** The selected card will highlight with a blue border to indicate it is active.

> **[IMAGE PLACEHOLDER: Step 1 Select Context]**
> *Highlight suggestion: Draw a box around the search bar and highlight the selected Context resource card.*

---

### Step 2: Pottery Collection File

In this step, you will upload your data file, review a preview of the tabular data, and initiate the import process to generate the records all on the same screen.

*   **Verify Context:** At the top of the screen, a blue information box will display the **Related Context** and **Context number** you selected in Step 1. Ensure this is correct before proceeding.
*   **Upload File:** Click the **"Choose CSV/XLSX"** button to browse your computer and select the spreadsheet containing your pottery data.
*   **Review File Metadata:** Once selected, the system will display statistics about your file, including the number of **Rows**, **Columns**, **Format**, and **File size**.
*   **Data Preview:** Scroll down to the **"Preview"** section to see a table displaying the headers and initial rows of your spreadsheet. Verify that the columns align correctly.
*   **Import Data:** If the preview looks correct, click the blue **"Prepare import data"** button to process the file and generate the records.
*   **Review Import Results:** Immediately after processing, an **"Import result"** panel will appear below the button. 
    *   **Statistics:** Review the summary blocks to see exactly how many records were **Created**, **Updated**, or **Skipped**.
    *   **Errors:** If the system encountered issues with specific rows, they will be listed under the **"Errors"** section with the exact row number.
    *   **Prepared Data:** Review the tables generated from your file, categorized by their attributes (Type, Diagnostic, Undiagnostic, etc.).
    *   **Missing Concepts:** If your spreadsheet contained terminology not recognized by the system's dictionaries, they will be listed at the bottom so you can address them later.

> **[IMAGE PLACEHOLDER: Step 2 Upload, Preview, and Results]**
> *Highlight suggestion: Highlight the "Choose CSV/XLSX" button, the Data Preview table, the "Prepare import data" button, and the "Import result" panel containing the generated statistics and tables.*