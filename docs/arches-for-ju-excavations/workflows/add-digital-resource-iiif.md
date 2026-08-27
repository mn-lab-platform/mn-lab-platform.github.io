## Add Digital Resource IIIF

This workflow allows you to upload image files (such as GeoTIFFs or standard photos) to generate a brand new IIIF Digital Resource, and simultaneously link it to an existing parent resource in your database. 

---

### Step 1: Select Resource

The first step is to choose the existing parent resource to which your new IIIF image will be linked.

*   **Search for a Resource:** Use the **"Search resources..."** input bar to filter existing records by name.
*   **Select a Resource:** The available resources are displayed as clickable cards. Click on the card of the target resource.
*   **Confirm Selection:** The chosen card will highlight to indicate it has been selected.

> **[IMAGE PLACEHOLDER: Step 1 Select Resource]**
> *Highlight suggestion: Draw a box around the search bar and highlight the selected resource card.*

---

### Step 2: Add IIIF Image

In this step, you will define the new digital resource, upload your files, and process them.

*   **Resource Name:** Enter a name for the new IIIF resource in the **"Resource name"** text field. This name is used to organize your files within the folder structure.
*   **Select Upload Mode:** Choose how your files should be processed using the radio buttons:
    *   **GeoTIFF (DEM/Ortho):** Select this for spatial GeoTIFF files. 
    *   **Photo (JPG/PNG):** Select this for standard photos that use the IIIF Image API without DEM processing.
*   **Upload Files:** Drag and drop your image files into the dashed dropzone area, or click the **"Choose file…"** button.
*   **Manage Selected Files:** Uploaded files will populate the **"Selected files"** table below. 
    *   **Classify DEM/Ortho:** If you are in GeoTIFF mode, click the toggle button in the "Is DEM" column to classify each file as a **DEM** (blue button) or **Ortho** (grey button).
    *   **Remove:** Click the red **"Remove"** button if you need to delete a file from the queue.
*   **Start Upload:** Once the queue is properly set, click the green **"Start Upload"** button.
*   **Processing:** A progress bar will appear. Wait until you receive the green **"Success!"** message confirming that the files have been processed and the new manifest has been created.

> **[IMAGE PLACEHOLDER: Step 2 Add IIIF Image]**
> *Highlight suggestion: Highlight the "Resource name" input field, the "Upload mode" radio buttons, the dropzone area, the DEM/Ortho toggle button inside the file table, and the green "Start Upload" button.*