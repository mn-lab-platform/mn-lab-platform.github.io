## Annotate Digital Resource 3D

This workflow allows you to manage annotations on existing 3D models within your database. The process branches into different paths depending on whether you want to create a brand new annotation or edit an existing one.

---

### Step 1: Select Resource

The first step is to select the 3D model or digital resource that you wish to annotate.

*   **Search for a Resource:** Use the **"Search resources..."** input bar at the top of the screen to filter your available models by name.
*   **Select a Model:** Click on the card representing the 3D resource you want to work with.
*   **Confirm Selection:** Once clicked, the resource card will highlight to indicate your selection.

> **[IMAGE PLACEHOLDER: Step 1 Resource Selection]**
> *Highlight suggestion: Draw a box around the "Search resources..." bar and highlight a selected 3D resource card.*

---

### Step 2: Select Process

After choosing your 3D model, you must decide what action you want to perform on it. You will be presented with two large option cards. 

*   **Add a New Annotation:** Select this option if you want to draw and configure a brand new spatial annotation on the 3D model.
*   **Edit Existing Annotations:** Select this option if you need to modify or update an annotation that has already been created for this model.
*   **Confirmation:** The card you click will highlight with a blue border and background. Your choice here will determine the steps you see next.

> **[IMAGE PLACEHOLDER: Step 2 Process Selection]**
> *Highlight suggestion: Highlight the two process selection cards ("Add a New Annotation" and "Edit Existing Annotations"), showing one of them in its active/selected state.*

### Step 3: Manage 3D Model Annotations

In this step, your selected 3D model is loaded into an interactive 3D viewer. The tools available to you will depend on the process you selected in Step 2.

*   **Loading Data:** The system will briefly display a "Loading 3D models..." message while it fetches the model and any associated spatial data. You can click and drag to rotate the 3D model, and scroll to zoom in and out.

#### If you chose "Add a New Annotation"
*   **Drawing Tools:** Use the drawing tools menu located within the viewer window to draw a new polygon shape directly onto the 3D model's surface.
*   **Proceeding:** Once you have completed drawing the boundaries of your new annotation, the spatial data is captured, and the workflow will automatically move you to the next step to configure its details.

> **[IMAGE PLACEHOLDER: Step 3 Add Annotation]**
> *Highlight suggestion: Highlight the main 3D viewer window, and specifically draw a box around the drawing tools menu used to initiate the polygon drawing process.*

#### If you chose "Edit Existing Annotations"
*   **Selection Tool:** To modify an existing annotation, you must first activate the custom selection tool. Click the specific selection button in the viewer's toolbar. 
*   **Editing Properties:** With the tool active, click on any existing annotation on the 3D model. This will allow you to update its specific details, including the **Name**, **Description**, and **Color**. 
*   **Deleting:** You also have the option to completely remove an annotation using the delete function (the system will display a "Deleting annotation..." status message).
*   **Saving:** When you modify an existing annotation's properties, you will see a "Saving changes..." message as the database updates. Once saved, you will proceed to the next step.

> **[IMAGE PLACEHOLDER: Step 3 Edit Annotation]**
> *Highlight suggestion: Draw a prominent box or arrow pointing to the specific "special custom cesium viewer tool" button used for selecting existing annotations. If possible, also show the edit panel where the user changes the name, description, and color.*

### Step 4: Define the Annotation Object / Summary

What you see in this step depends entirely on whether you chose to add a new annotation or edit an existing one in Step 2. 

#### If you chose "Edit Existing Annotations" (Workflow Complete)
If you just finished editing an existing annotation in the 3D viewer, this step acts as your final confirmation screen. 
*   **Success Message:** You will see a message stating: *"Annotation process completed successfully. You can safely delete the workflow, your changes are saved!"* 
*   **Next Steps:** Since your edits are instantly saved to the database, you have completed the process and can safely exit the workflow.

> **[IMAGE PLACEHOLDER: Step 4 Edit Summary]**
> *Highlight suggestion: Highlight the success message text indicating that the process is complete and the changes are saved.*

#### If you chose "Add a New Annotation"
If you just finished drawing a new polygon shape on the 3D model, you must now provide its identifying details before continuing. 

*   **Annotation Name:** Type a clear name for your new annotation in this text field.
*   **Annotation Description:** Provide any relevant details or context about the annotated area in this text box.
*   **Annotation Color:** Click the square color swatch to open the color picker. Choose the color that will represent this specific annotation on the 3D model.
*   **Proceeding:** Fill out the form and proceed to the next step to determine how this new annotation will be classified in the system.

> **[IMAGE PLACEHOLDER: Step 4 Annotation Form]**
> *Highlight suggestion: Draw a box around the entire form, specifically pointing out the text inputs for Name/Description and the interactive Color square.*

### Step 5: Select Annotation Type

*(Note: You will only see this step if you are creating a new annotation).* 

After defining the details of your new annotation, you must decide how it should be stored in the database. You will be presented with two option cards to choose from:

*   **Create Plain Annotation:** Select this option if you simply want to add a standalone spatial note or markup to the 3D model. This creates the annotation but does not generate a separate resource record for the annotated object itself.
*   **Create Annotation and Associate with Resource:** Select this option if the area you just annotated represents a distinct physical entity (such as a specific artifact, wall, or feature) that requires its own dedicated resource record in the database. This path will allow you to link the visual annotation directly to a new conceptual record.
*   **Make a Selection:** Click on the card that fits your needs. The selected card will highlight with a blue border and background. 

> **[IMAGE PLACEHOLDER: Step 5 Annotation Type Selection]**
> *Highlight suggestion: Highlight the two option cards ("Create Plain Annotation" and "Create Annotation and Associate with Resource"), showing one of them in its active/selected state.*

### Step 6: Select Resource Type / Summary

What appears in this step depends on the choice you made in Step 5 regarding how the annotation should be stored. *Note: Before the screen appears, you may briefly see a loading message while the system saves your drawn annotation to the database.*

#### If you chose "Create Plain Annotation" (Workflow Complete)
If you opted to create a standalone annotation, this step acts as your final confirmation screen. 
*   **Success Message:** You will see a success message indicating: *"Annotation process completed successfully. You can safely delete the workflow, your changes are saved!"* 
*   **Next Steps:** The annotation is now saved to the 3D model. You have completed the process and can safely exit the workflow.

> **[IMAGE PLACEHOLDER: Step 6 Plain Annotation Summary]**
> *Highlight suggestion: Highlight the success message text indicating that the process is complete.*

#### If you chose "Create Annotation and Associate with Resource"
If you chose to link your new annotation to a dedicated resource record, you must now select the *type* of resource you want to create (e.g., a Context, an Artifact, a Physical Feature, etc.).

*   **Select a Category:** You will see a grid of option cards representing the available resource types in your database. Click on the card that best categorizes the object you just annotated.
*   **Confirmation:** The selected resource card will highlight with a blue border and a light blue background. 
*   **Proceeding:** Once your resource type is selected, proceed to the next step to fill out the specific details for this new physical resource.

> **[IMAGE PLACEHOLDER: Step 6 Resource Type Picker]**
> *Highlight suggestion: Highlight the grid of resource type cards, specifically drawing a box around one of the cards in its active/selected state (with the blue border and background).*

### Step 7: Create or Link Resource

If you chose to associate your annotation with a resource, this step allows you to define exactly what that resource is. You have the flexibility to either link the annotation to a resource that *already exists* in your database, or create a brand *new* resource record right now. 

You control this choice using the toggle switch located at the top right of the screen.

#### Option A: Select Existing (Toggle Left)
This is the default view. Use this if the object you annotated already has a corresponding record in the database.

*   **Search:** Use the **"Search resources..."** input bar to filter the existing records by name. The list only displays resources of the type you selected in the previous step.
*   **Select:** The available records are displayed as cards. Click on the card representing the correct resource. 
*   **Confirm:** The selected card will be highlighted with a blue border. 

> **[IMAGE PLACEHOLDER: Step 7 Select Existing Resource]**
> *Highlight suggestion: Draw a box around the toggle switch (showing it in the "Select Existing" position), the search bar, and highlight one of the selected resource cards.*

#### Option B: Create New (Toggle Right)
Use this if the object you annotated is entirely new and does not yet exist in the database.

*   **Toggle the Switch:** Click the toggle switch so the slider moves to the right, activating **"Create New"** mode.
*   **Data Entry:** The screen will change to display a data entry form tailored to the resource type you selected in Step 6. Fill out all required fields to define this new resource.
*   **Save:** Once the form is complete, ensure the new record is saved using the provided form controls before proceeding to the final summary step.

> **[IMAGE PLACEHOLDER: Step 7 Create New Resource]**
> *Highlight suggestion: Draw a box around the toggle switch (showing it in the "Create New" position with the blue slider) and the data entry form that appears below it.*

### Step 8: Summary

This is the final screen confirming that your new annotation has been successfully created and formally linked to the resource you selected or generated in the previous step.

*   **Confirmation:** You will see a green success checkmark and the message: **"Annotation created successfully and linked to the resource!"**
*   **Next Steps:** The entire annotation and linking process is now complete. Your changes are saved to the database. You can safely exit the workflow, or click the button on the screen to view the newly updated resource.

> **[IMAGE PLACEHOLDER: Step 8 Summary]**
> *Highlight suggestion: Highlight the success message text and, if present, the button allowing the user to view the resource.*