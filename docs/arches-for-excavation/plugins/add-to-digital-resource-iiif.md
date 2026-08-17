## Add To Existing Digital Resource IIIF

This workflow allows you to append additional image files (such as new GeoTIFFs or standard photos) to an IIIF digital resource that already exists in your database. It updates the existing resource's manifest with new canvases rather than creating a brand new record.

---

### Step 1: Select Existing IIIF Resource

First, you need to identify which existing IIIF resource you want to add new files to.

*   **Search for a Resource:** Use the **"Search IIIF resources..."** input bar to find the specific digital resource.
*   **Select a Resource:** The available IIIF resources will be displayed as clickable cards. Click on the card of the resource you wish to update. 
*   **Confirm Selection:** The chosen card will highlight to indicate it is selected.

> **[IMAGE PLACEHOLDER: Step 1 Select Existing Resource]**
> *Highlight suggestion: Draw a box around the "Search IIIF resources..." bar and highlight the selected resource card.*

---

### Step 2: Append Files

In this step, you will select the type of files you are uploading, add them to the queue, and process them into the existing IIIF manifest.

*   **Select Upload Mode:** Choose the appropriate radio button for your file types:
    *   **GeoTIFF (DEM/Ortho):** Select this if you are uploading spatial GeoTIFF files. 
    *   **Photo (JPG/PNG):** Select this if you are uploading standard image files. *(Note: This mode uses the IIIF Image API without DEM processing).*
*   **Upload Files:** In the dashed dropzone area, drag and drop your files or click the **"Choose file…"** button to select them from your computer.
*   **Manage Selected Files (Queue):** Once files are added, they appear in a "Selected files" table below the dropzone.
    *   **Is DEM / Ortho Toggle:** If you selected the *GeoTIFF* upload mode, you will see a toggle button in the "Is DEM" column. Click this button to classify each file as either a **DEM** (blue button) or an **Ortho** (grey button).
    *   **Remove:** If you added a file by mistake, click the red **"Remove"** button next to it.
*   **Start Upload:** Once your queue is ready and properly classified, click the green **"Start Upload"** button.
*   **Processing:** A progress bar will appear showing that the system is processing the files. Wait until you see the green **"Success!"** message confirming the files have been processed and appended to the existing manifest.

> **[IMAGE PLACEHOLDER: Step 2 Append Files]**
> *Highlight suggestion: Highlight the "Upload mode" radio buttons, the dashed Dropzone area, the DEM/Ortho toggle button inside the "Selected files" table, and the green "Start Upload" button.*