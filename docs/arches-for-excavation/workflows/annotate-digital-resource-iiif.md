## Annotate Digital Resource IIIF

This workflow allows you to open an existing IIIF image (like an orthomap) in an interactive viewer, draw spatial annotations on it, and save those annotations either as simple spatial notes or link them directly to a separate database resource.

---

### Step 1: Select Resource

The first step is to choose the existing IIIF resource you want to annotate.

*   **Search for a Resource:** Use the **"Search resources..."** input bar at the top to find your target image. Look for the placeholder text *"— Select which ortomap to annotate —"*.
*   **Select a Resource:** The available resources are displayed as clickable cards. Click on the card of the image you wish to use. 
*   **Confirm Selection:** The chosen card will highlight to indicate it is selected. 

> **[IMAGE PLACEHOLDER: Step 1 Select IIIF Resource]**
> *Highlight suggestion: Draw a box around the search bar and highlight the selected resource card.*

---

### Step 2: Add Annotation to IIIF

Once your resource is selected, the workflow loads the IIIF map viewer. Note: A "Loading manifest…" message will appear briefly. 

*   **Draw an Annotation:** Use the drawing tools provided within the map viewer to outline your feature of interest on the image. 
*   **Add Metadata:** As soon as you finish drawing a shape, a **"New annotation"** modal will pop up. 
    *   **Title:** Enter a name for the annotation (e.g., "Crack on the north wall").
    *   **Description:** Add optional context, notes, or interpretations.
    *   **Color:** Click the color swatch to assign a specific color to this drawing.
    *   Click the green **"Add annotation"** button to temporarily store this drawing.
*   **Track Pending Annotations:** At the bottom of the viewer, the system tracks unsaved drawings (e.g., *"Nowe adnotacje oczekują: 1"* / New annotations pending). You must add at least one annotation to unlock the saving process.

> **[IMAGE PLACEHOLDER: Step 2 Viewer and Metadata Modal]**
> *Highlight suggestion: Highlight the drawing tools on the map viewer, the status text tracking pending annotations at the bottom, and the "New annotation" popup form.*

---

### Finalize and Save Annotations

Once you are ready to save your pending annotations, trigger the save action from the viewer toolbar. This will open the **"Finalize output"** modal.

*   **Review Batch:** The modal displays a summary of the host resource and a list of all the pending annotations you just drew, including their color previews.
*   **Select Save Mode:** Use the **"Save mode"** dropdown to determine how these annotations are stored:
    *   **Annotation only:** Saves the drawings purely as spatial annotations on the image.
    *   **Link annotations to another resource:** Select this if the annotated area represents a specific physical entity that needs its own record.
*   **If Linking (Optional):** If you chose to link to another resource, a new section will appear:
    *   **Select resource type:** Choose the graph/category from the dropdown.
    *   **Target resource:** Search for and select an existing resource record, or use the provided creator panel below to instantly generate a new record to link to.
*   **Save:** Click the green **"Save annotations"** button at the bottom right. A loading spinner will appear, followed by a green success message once the database is updated.

> **[IMAGE PLACEHOLDER: Step 3 Finalize Output Modal]**
> *Highlight suggestion: Highlight the "Save mode" dropdown, the list of annotations in the batch, and the "Save annotations" button.*