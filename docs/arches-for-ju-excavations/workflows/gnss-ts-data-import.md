## GNSS/Total Station Data Import (Context Footprints)

This workflow allows you to import footprint and coordinate measurements from GNSS or Total Station devices and attach them directly to Context or Trench resources in your database. 

---

### Step 1: Select Measurement Type

The first step is to determine exactly what type of resource you are importing measurements for. You will be presented with four option cards.

*   **Make a Selection:** Click on the card that matches the data you wish to import:
    *   **Import Context Measurements:** For standard Context records.
    *   **Import (O) Context Measurements:** For (O) Context records.
    *   **Import Trench Measurements:** For standard Trench records.
    *   **Import (O) Trench Measurements:** For (O) Trench records.
*   **Confirmation:** The card you click will highlight with a blue border and background to indicate your selection. Your choice here determines which records you can search for in the next step.

> **[IMAGE PLACEHOLDER: Step 1 Select Measurement Type]**
> *Highlight suggestion: Highlight the grid of four option cards, specifically drawing a box around the active/selected card (showing the blue border and background).*

---

### Step 2: Select Resource

Now that you have defined the type of record, you must find and select the specific target resource in the database. 

*   **Search for a Resource:** Use the **"Search for a Context resource..."** input bar to filter the records by name. The list will only display resources that match the category you chose in Step 1.
*   **Select a Resource:** The matching records are displayed as clickable cards. Click on the card representing the specific Context or Trench you want to attach the measurements to.
*   **Confirm Selection:** The chosen card will highlight with a blue border and a checkmark. 

> **[IMAGE PLACEHOLDER: Step 2 Select Resource]**
> *Highlight suggestion: Draw a box around the search bar and highlight the selected Context/Trench resource card.*

---

### Step 3: Select Coordinate Reference System (CRS) Type

In this step, you must define the coordinate format of the measurements you are about to import. You will see two option cards:

*   **Coordinates are in Local CRS:** Select this if your imported measurements are based on a custom local grid established for your specific excavation site.
*   **Coordinates are in WGS84 CRS:** Select this if your imported measurements use the standard global coordinate system (WGS84).
*   **Make a Selection:** Click the card that corresponds to your data. The selected card will highlight, and the workflow will direct you to the appropriate next steps based on this choice.

> **[IMAGE PLACEHOLDER: Step 3 Select CRS Type]**
> *Highlight suggestion: Highlight the two CRS option cards ("Local CRS" and "WGS84 CRS"), showing one of them in its active/selected state.*

### Step 4: CRS Definition / Coordinate Entry

The interface for this step changes entirely depending on the coordinate system type you selected in Step 3. 

#### If you chose "Coordinates are in Local CRS" (Step 3)
Because your measurements use a custom grid, you must now define or select that grid (Coordinate Reference System) so the system knows how to place the footprint on a real-world map. You control this using the toggle switch at the top.

*   **Option A: Select Existing (Toggle Left):** If the Local CRS for this trench/site has already been added to the database, use the search bar to find and select it from the list of cards.
*   **Option B: Create New (Toggle Right):** If this is a new local grid, toggle the switch to the right. A form will appear allowing you to define the new CRS by inputting its Origin coordinates (Local X/Y and Global Long/Lat) and Direction coordinates. 
*   **Proceed:** Once selected or created, you will move to the next step to enter your actual coordinate data.

> **[IMAGE PLACEHOLDER: Step 4 Local CRS - Toggle and Search/Create]**
> *Highlight suggestion: Draw a box around the "Select Existing / Create New" toggle switch and highlight the active area below it (either the search bar or the creation form).*

#### If you chose "Coordinates are in WGS84 CRS" (Step 3)
Because your measurements are already in a standard global format, you bypass CRS creation and go straight to entering your GNSS/Total Station coordinate data.

*   **Input Coordinates:** Paste your raw coordinate data directly into the large text area. The system expects a specific format (usually line-by-line coordinates). 
*   **Reorder X and Y (Tool):** If your GNSS device exports coordinates as Y,X (Latitude, Longitude) instead of X,Y, click the **top circular button** (with the reorder/swap arrows) on the right side of the screen to quickly swap the columns in your text area.
*   **Ignore Last Line (Tool):** If your imported data ends with an invalid line (like a summary string or an empty space that causes a validation error), click the **bottom circular button** (with the skip icon) to instruct the system to ignore the final line of text.
*   **Validation:** The system will validate your text. If there is a formatting issue, an error message will appear at the top. Once valid, you can proceed.

> **[IMAGE PLACEHOLDER: Step 4 WGS84 - Coordinate Entry]**
> *Highlight suggestion: Highlight the large coordinate input text area, and specifically draw boxes around the two circular tool buttons on the right side ("Reorder X and Y" and "Ignore last line").*

### Step 5: Coordinate Entry / Map Display

The interface for this step continues to adapt based on the coordinate system type you selected in Step 3. 

#### If you chose "Coordinates are in Local CRS" (Step 3)
In the previous step, you defined your custom coordinate grid. Now, you must enter the actual GNSS/Total Station coordinate data that aligns with that grid.

*   **Input Coordinates:** Paste your raw local coordinate data directly into the large text area. Ensure it follows a standard line-by-line format. 
*   **Reorder X and Y (Tool):** If your device exported the coordinates in the wrong order, click the **top circular button** (with the reorder/swap arrows) on the right side of the screen to instantly swap the X and Y columns.
*   **Ignore Last Line (Tool):** If your imported data ends with an invalid string or empty space that causes an error, click the **bottom circular button** (with the skip icon) to instruct the system to ignore the final line of text.
*   **Validation:** The system validates your text formatting in real-time. If there is an issue, a red error message will appear. Once the data is valid, you can proceed to the next step.

> **[IMAGE PLACEHOLDER: Step 5 Local CRS - Coordinate Entry]**
> *Highlight suggestion: Highlight the large coordinate input text area and draw boxes around the two circular tool buttons on the right side ("Reorder X and Y" and "Ignore last line").*

#### If you chose "Coordinates are in WGS84 CRS" (Step 3)
Because you already entered your global coordinates in the previous step, the system will now project them onto a real-world map for visual verification.

*   **Map Verification:** Review the interactive map viewer to ensure your coordinates accurately represent the physical footprint. The system will automatically connect your points (drawing a line for 2 points, or a blue polygon for 3 or more points).
*   **Inspect Points:** Click on any of the blue markers to open a detailed popup. This displays the point's label, Longitude (Lng), Latitude (Lat), and Elevation (Z).
*   **Change Basemap:** To better contextualize the footprint, use the layer control panel located in the **top-right corner** of the map. You can click on the different options to switch between available basemaps (e.g., standard map view vs. satellite imagery).

> **[IMAGE PLACEHOLDER: Step 5 WGS84 - Map Display]**
> *Highlight suggestion: Draw a box around the plotted polygon/points on the map, highlight an open marker popup, and draw a box around the basemap switcher control panel in the top-right corner.*

### Step 6: Map Verification / Verify and Save

Because the order of operations changes based on the coordinate system you selected in Step 3, this step will display one of two screens depending on your path.

#### If you chose "Coordinates are in Local CRS" (Step 3)
In the previous step, you entered your raw local coordinates. Now, the system has used the Coordinate Reference System you defined to project those points onto a global map for visual verification.

*   **Map Verification:** Review the interactive map viewer to ensure your footprint is accurately placed in the real world. The system automatically connects your points.
*   **Inspect Points:** Click on any of the blue markers to open a detailed popup displaying the point's label and converted Longitude (Lng), Latitude (Lat), and Elevation (Z).
*   **Change Basemap:** Use the layer control panel located in the **top-right corner** of the map to switch between available basemaps (e.g., standard map view vs. satellite imagery) to better verify the placement.
*   **Proceed:** Once you have visually verified the footprint, proceed to the next step to finalize the save.

> **[IMAGE PLACEHOLDER: Step 6 Local CRS - Map Display]**
> *Highlight suggestion: Draw a box around the plotted polygon on the map, highlight an open marker popup, and draw a box around the basemap switcher control panel in the top-right corner.*

#### If you chose "Coordinates are in WGS84 CRS" (Step 3)
Because you already verified your WGS84 coordinates on the map in the previous step, you are now ready to review the final data package and commit it to the database.

*   **Verify Data:** The screen displays a side-by-side view of the data that will be saved to the database resource.
    *   **Left Panel (GeoJSON):** Shows the system-generated spatial code representing your footprint.
    *   **Right Panel (Plain Text):** Shows the raw coordinate data you initially pasted.
*   **Save Footprint:** If the data is correct, click the large green **"Add to Resource"** button at the bottom right of the screen. 
*   **Status:** A loading indicator will appear. Wait for the green success message confirming that the footprint has been permanently attached to your selected Context/Trench resource.

> **[IMAGE PLACEHOLDER: Step 6 WGS84 - Verify and Save]**
> *Highlight suggestion: Highlight the dual-pane view showing the GeoJSON and raw text side-by-side, and specifically point an arrow to the large green "Add to Resource" button.*

### Step 7: Verify and Save / Summary

This step concludes the process for both CRS paths, though the view differs slightly based on your initial choice in Step 3.

#### If you chose "Coordinates are in Local CRS" (Step 3)
Because you just verified the map projection in the previous step, you must now review the final data package before saving. 

*   **Verify Data:** The screen displays a side-by-side view of the data that will be saved to the database.
    *   **Left Panel (GeoJSON):** Shows the converted global spatial code representing your footprint.
    *   **Right Panel (Plain Text):** Shows the raw local coordinate data you initially pasted.
*   **Save Footprint:** If everything looks correct, click the large green **"Add to Resource"** button at the bottom right of the screen. 
*   **Proceed:** A loading indicator will appear as the database updates. Once saved, you will move to the final Summary screen.

> **[IMAGE PLACEHOLDER: Step 7 Local CRS - Verify and Save]**
> *Highlight suggestion: Highlight the dual-pane view showing the GeoJSON and raw text side-by-side, and specifically point an arrow to the large green "Add to Resource" button.*

#### If you chose "Coordinates are in WGS84 CRS" (Step 3) (Workflow Complete)
Because you already verified and saved your data in the previous step, this step acts as your final confirmation screen.

*   **Confirmation:** You will see a green checkmark and a **"Success!"** message indicating the footprint was saved. (If an error occurred during saving, a red "Incomplete" warning will display instead).
*   **View your Resource:** You can immediately inspect your updated Context or Trench record by clicking the blue **"View Resource"** button. This will open the record in a new browser tab.
*   **Finish:** The workflow is now complete and can be safely closed.

> **[IMAGE PLACEHOLDER: Step 7 WGS84 - Summary]**
> *Highlight suggestion: Highlight the green Success card and the blue "View Resource" button.*

### Step 8: Summary

*(Note: You will only reach this 8th step if you chose "Coordinates are in Local CRS" in Step 3. The WGS84 path concludes at Step 7).*

This is the final confirmation screen verifying that your local coordinates have been successfully converted, projected, and saved to your database resource.

*   **Confirmation:** You will see a green checkmark and a **"Success!"** message indicating the footprint was securely attached. (If an error occurred during the final save process, a red "Incomplete" warning will display instead).
*   **View your Resource:** Click the blue **"View Resource"** button to immediately open and inspect your newly updated Context or Trench record in a new browser tab.
*   **Finish:** The workflow is now complete and can be safely closed.

> **[IMAGE PLACEHOLDER: Step 8 Local CRS - Summary]**
> *Highlight suggestion: Highlight the green Success card, the success message, and the blue "View Resource" button.*