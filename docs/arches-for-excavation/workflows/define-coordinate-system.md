This workflow allows you to create a new Local Coordinate System (CRS) in the database. You will define the system by specifying two key components: an origin point (using both local X/Y coordinates and real-world longitude/latitude) and a direction point (using real-world longitude/latitude). 

---

### Step 1: Create Local Coordinate System

This workflow consists of a single form that requires you to input the parameters for your new coordinate system. 

*   **General Information:** 
    *   **Name:** Enter a clear, identifiable name for your coordinate system (Required).
    *   **Description:** Provide any additional context or details about this coordinate system (Optional).
*   **Origin Point Details:**
    *   **Origin Local X & Y:** Enter the local numerical X and Y coordinates for your origin point (Required).
    *   **Origin Longitude & Latitude:** Enter the real-world global coordinates (Longitude and Latitude) that correspond to your origin point (Required).
*   **Direction Point Details:**
    *   **Direction Longitude & Latitude:** Enter the real-world global coordinates (Longitude and Latitude) to establish the orientation/direction of the local grid (Required).
*   **Submit:** Once all required fields are filled out, click the green **"Create CRS"** button at the bottom of the form to save the new coordinate system to the database.

> **[IMAGE PLACEHOLDER: CRS Creation Form]**
> *Highlight suggestion: Draw a box encompassing the entire form, potentially adding small arrows pointing to the required numeric fields (Local X/Y, Origin Lon/Lat, Direction Lon/Lat) and the green "Create CRS" button at the bottom.*