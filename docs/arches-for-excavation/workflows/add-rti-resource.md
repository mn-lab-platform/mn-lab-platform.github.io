## Add RTI Resource

This workflow allows you to upload a Reflectance Transformation Imaging (RTI) package (specifically a Relight ZIP package) and attach it to an existing resource in your database. The system will process the images, generate IIIF-compatible planes, and allow you to adjust the rotation and crop of the final RTI viewer.

---

### Step 1: Select Resource

The first step is to choose the existing parent resource to which you want to attach the new RTI asset.

*   **Search for a Resource:** Use the **"Search resources..."** input bar to find the specific record.
*   **Select a Resource:** Click on the card of the resource you wish to use. 
*   **Confirm Selection:** The chosen card will highlight to indicate it is selected as the target resource.

> **[IMAGE PLACEHOLDER: Step 1 Select Resource]**
> *Highlight suggestion: Draw a box around the search bar and highlight the selected resource card.*

---

### Step 2: Upload RTI Package

In this step, you will define the RTI asset's name and upload the required ZIP package containing your image planes and Relight metadata.

*   **RTI Name:** Enter a descriptive name for the RTI asset in the **"RTI name"** text field (e.g., "Coin RTI front side").
*   **Select Package:** Click the **"Choose File"** (or equivalent) button under **"Relight ZIP package"** to select your `.zip` file. *Note: The ZIP must contain the JPG planes and the Relight `info.json` file.*
*   **Upload:** Once the file is selected, click the blue **"Upload RTI package"** button.
*   **Processing:** The system will display a yellow warning banner stating: *"Processing ZIP, converting JPG files to COG TIFF..."*. Please wait while the system processes the heavy image files.
*   **Confirmation:** Upon successful processing, a panel titled **"Generated IIIF planes"** will appear, displaying a table of all the processed layers, their source files, and their new IIIF service URLs.

> **[IMAGE PLACEHOLDER: Step 2 Upload RTI Package]**
> *Highlight suggestion: Highlight the "RTI name" input field, the file upload input, the "Upload RTI package" button, and the "Generated IIIF planes" table at the bottom.*

---

### Step 3: Adjust RTI View

The final step allows you to fine-tune how the RTI is displayed in the viewer before saving it permanently to the database.

*   **Interactive Viewer:** The processed RTI will load in an interactive viewer on the screen.
*   **Rotation:** Use the **"Rotation"** slider located below the viewer to adjust the orientation of the image from 0° to 360°.
*   **Cropping (Optional):** If you need to crop the image bounds:
    1.  Click the **"Select crop"** button to activate cropping mode.
    2.  Draw your desired crop box directly over the image in the viewer (the coordinates will appear below the buttons).
    3.  Click the blue **"Apply crop to rasters"** button to crop the underlying files.
    4.  *If you make a mistake, click "Clear crop selection" to reset.*
*   **Save Settings:** Once the rotation and crop are set to your liking, click the blue **"Save settings"** button at the bottom of the screen to finalize the workflow.

> **[IMAGE PLACEHOLDER: Step 3 Adjust RTI View]**
> *Highlight suggestion: Highlight the Rotation slider, the row of crop-related buttons ("Select crop", "Apply crop to rasters"), and the final "Save settings" button.*