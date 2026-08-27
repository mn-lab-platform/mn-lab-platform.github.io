## Interactive Map Viewer

This plugin provides a fully interactive MapLibre-based environment directly within Arches. Unlike standard step-by-step data entry workflows, this is a continuous workspace where you can search your database for resources, plot them on a map as distinct layers, customize their appearance, and save your workspace or export it to PDF.

---

### Adding Resource Layers

To begin visualizing data, you need to pull resources from your database and add them to the map as layers. 

*   **Open the Search Panel:** Click the **"Add Layer"** button to open the Resource Search flyout (the button text will change to "Close Flyout" while it is open).
*   **Search for Resources:** Use the main search bar to look up specific records.
    *   *Advanced Search:* Check the **"Advanced search"** box to paste a specific Arches search URL directly. (If the URL is invalid, the input box will turn red with the warning *"Please enter a valid search URL"*).
*   **Filter and Select:** 
    *   Use the **Type dropdown** to filter the search results by specific resource models.
    *   Once filtered by type, you can use the **"Select All"** button to quickly grab all matching records.
    *   Check the **"Selected only"** box to review exactly which resources you have queued up.
*   **Create the Layer:** Once you have selected at least one resource, the **"Create Layer"** button at the bottom of the panel will become active. Click it to generate the layer and close the flyout.

> **[IMAGE PLACEHOLDER: Add Layer Flyout]**
> *Highlight suggestion: Draw a box around the "Add Layer" button, the search input area, the Type filter dropdown, and the "Create Layer" button.*

---

### Managing the Layer Menu

Once you have added layers to your map, they will appear in the main layer menu panel. Here, you can control how they stack and interact with one another.

*   **Visibility:** Toggle the checkbox next to any layer's name to instantly show or hide it on the map.
*   **Reordering:** The order of the layers in the menu dictates how they stack on the map (top layers cover bottom layers). You can reorder them by dragging and dropping them, or by using the **"Move Layer Up"** and **"Move Layer Down"** arrow buttons.
*   **Save & Load Workspaces:** You don't have to rebuild your map from scratch every time.
    *   **Save:** Click the **"Save Layers to File"** button to download a file containing your current layer setup.
    *   **Load:** Click the **"Load Layers from File"** button to upload a previously saved workspace file. *(Note: If you upload the wrong file type, you will receive an "Invalid file format" or "Error reading file" warning).*

> **[IMAGE PLACEHOLDER: Layer Menu Options]**
> *Highlight suggestion: Highlight the layer visibility checkboxes, the Move Up/Down arrows, and the "Save Layers to File" / "Load Layers from File" buttons.*

---

### Layer Settings & Styling

You can customize the appearance of any individual layer to make your map easier to read and analyze.

*   **Open Settings:** Click directly on a layer's name in the menu to open the **"Map Layer Settings"** flyout.
*   **General Settings:** 
    *   **Layer Name:** Rename the layer for your own organizational purposes.
    *   **Opacity:** Use the slider to make the layer more transparent (useful for comparing overlapping layers).
*   **Styling (Colors & Fills):** Depending on the type of geometry (Point, Line, or Polygon), you can use the color pickers to adjust the **Label Color**, **Point Color**, and **Line Color**. Polygons also feature a hatch fill button to cycle through different patterns.
*   **Labels:**
    *   **Label Property:** Select which database property should be used to label the features on the map.
    *   **Custom Label:** If you prefer, type a custom label to override the property data.
*   **Apply Changes:** Once you alter a setting, the blue **"Apply Changes"** button becomes active. Click it to push your visual updates to the map.
*   **Delete Layer:** Click the **"Delete"** button to completely remove the layer from your workspace. A confirmation pop-up will ask: *"Are you sure you want to delete the layer [Name]?"*

> **[IMAGE PLACEHOLDER: Map Layer Settings Flyout]**
> *Highlight suggestion: Draw a box around the Layer Name input, Opacity slider, the Color picker inputs, and the "Apply Changes" button.*

---

### Exporting Your Map

Once your map is styled exactly how you need it, you can export the current view to share or print.

*   **PDF Export:** Trigger the PDF export function. You will see a global loading overlay appear over the map while the system processes the heavy graphics and generates your document. Once the overlay disappears, your download will begin. 

> **[IMAGE PLACEHOLDER: PDF Export & Loading Overlay]**
> *Highlight suggestion: Highlight the PDF export button and provide a screenshot showing the semi-transparent busy overlay covering the map during processing.*