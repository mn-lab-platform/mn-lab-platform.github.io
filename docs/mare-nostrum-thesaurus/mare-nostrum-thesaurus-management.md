# Mare Nostrum LAB thesaurus - Management

This section is dedicated to explain all specific procedures which allow searching, modifying and deleting information from the Mare Nostrum LAB thesaurus.

---

## Browsing Dictionaries

### Available Data

The Mare Nostrum LAB thesaurus project offers the following data dictionaries (click to explore):

- [**pottery types - amphorae**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_types_-_amphorae_Dictionary) - Mediterranean amphora types

- [**pottery types - lamps**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_types_-_lamps_Dictionary) - Mediterranean lamp types

- [**pottery types - table ware**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_types_-_table_ware_Dictionary) - Mediterranean table ware types

- [**pottery - morphology**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_-_morphology_Dictionary) - geometric characteristics of fragments

- [**pottery - vessel form**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_-_vessel_form_Dictionary) - general morphological categories

- [**pottery - vessel part**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_-_vessel_part_Dictionary) - preserved component part of a vessel

- [**pottery - sub-category**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_-_sub-category_Dictionary) - detailed product specification (primarily refers to the ceramic fabric/paste, which sometimes implies a specific repertoire of vessel types)

- [**pottery - state of preservation**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_-_state_of_preservation_Dictionary) - state of preservation of a found fragment

- [**pottery - surface treatment**](https://thesaurus.mn.cenagis.edu.pl/wiki/Pottery_-_surface_treatment_Dictionary) - type of exterior wall finishing

- [**provenance**](https://thesaurus.mn.cenagis.edu.pl/wiki/ProvenanceDictionary) - hierarchical dictionary of vessel production sites

- [**chronology**](https://thesaurus.mn.cenagis.edu.pl/wiki/ChronologyDictionary) - hierarchical timeframes

- [**Harris matrix relationships**](https://thesaurus.mn.cenagis.edu.pl/wiki/HarrisMatrixRelationshipsDictionary) - stratigraphic relationships according to the Harris matrix (describing chronological and spatial links between stratigraphic units)

- [**trench parameters**](https://thesaurus.mn.cenagis.edu.pl/wiki/TrenchParametersDictionary) - parameters defining the physical, material, and methodological characteristics of an archaeological trench. This includes:

    - **archaeological remains** - types of recovered artifacts and materials

    - **context characterization** - physical properties of the excavated layer, including its origin, soil color, grain size, and soil density

    - **excavation procedures** - methods applied during the excavation of the trench

- [**visual item metadata**](https://thesaurus.mn.cenagis.edu.pl/wiki/VisualItemMetadataDictionary) - visual object metadata, regarding drawing and image

- [**linguistic object metadata**](https://thesaurus.mn.cenagis.edu.pl/wiki/LinguisticObjectMetadataDictionary) - textual and linguistic attributes assigned to an object

---

### Searching for a Specific Value

1. If you know the specific record you are looking for, enter it in the dedicated panel located at the top of the interface.

    ![Specific Record](mare-nostrum-thesaurus-management/specific-record.png)

2. Clicking on an item redirects you to its content, displaying all defined properties.

    ![Specific Record Page](mare-nostrum-thesaurus-management/specific-record-page.png)

---

### Displaying and Searching Hierarchical Data

???+ note "Dictionaries structure"
    Each dictionary is represented by a drop-down list that can be opened by clicking the corresponding link name or by clicking the corresponding dictionary name in the [Available Data](#available-data) subsection.

1. Select a [dictionary](#available-data) of interest.

    ![Select a dictionary of interest](mare-nostrum-thesaurus-management/select-dictionary-from-thesaurus.png)

1. After selecting, an expandable view of the object hierarchy linked to the parent item is displayed (e.g., vessel part).

    ![Expandable view](mare-nostrum-thesaurus-management/drop-down-list.png)

1. To display a specific dictionary value, click on the blue **"Q"** identifier followed by a corresponding number.

    ![Inspect item](mare-nostrum-thesaurus-management/inspect-item.png)

---

## Modifying Dictionaries

### Manually Adding a New Item

???+ note "Log in before adding"
    Adding a new item requires [logging in](account-management.md/#logging-in-to-the-account) first.

1. Select the **"New item"** option from the Main page.

    ![New item option](mare-nostrum-thesaurus-management/new-item-button.png)

1. Enter the Label and Description. If aliases exist, they should also be provided here. Complete the process by clicking the **"Create"** button.

    ???+ note "Language"
        Pay close attention to the Language field while adding an item, as an unintentional change may result in incorrect value assignment.

    ![Create a new Item](mare-nostrum-thesaurus-management/label-description-aliases.png)

1. After creating the item, its page will appear on the screen, allowing you to verify the accuracy of the entered data and perform potential edits by clicking the **"edit"** button.

    ![Edit a new item](mare-nostrum-thesaurus-management/edit-new-item.png)

1. If the label, description, and aliases are correct, you typically need to define statements pointing to the properties (P) of the item. This is done using the **"add statements"** button.

    ![Add statement to the item](mare-nostrum-thesaurus-management/add-statement-new-item.png)

1. To add a new statement, follow steps below:
    
    - 1 - Enter the appropriate property by its name.
    
    - 2 - Provide the value representing the given feature.
        
        ???+ note "Matching types"
            Ensure that the added value type matches the property type.

    - *2a (optional) - Add a **"reference"** indicating the source of the information. Suggested property: [described at url (P29)](https://thesaurus.mn.cenagis.edu.pl/wiki/Property:P29).*
    - *2b (optional) - Assign a value to the selected property.* 
        
        ???+ note "Matching types"
            Ensure that the added value type matches the property type.

    - 3 - Save the statement for the item.

    ![Add statement elements](mare-nostrum-thesaurus-management/add-statement-elements.png)

1. After saving the statement, you can assign another value to it (**"add value"**) or create a new statement poining to the item (**"add statement"**).

    ![Further connections](mare-nostrum-thesaurus-management/add-value-add-statement.png)

---

### Editing an Existing Item

1. [Browse dictionaries](#browsing-dictionaries) for the item of interest (e.g., R'as al Basit).

1. Click the **"edit"** button with pencil icon.

    ???+ note "Log in before editing"
        Editing an item requires [logging in](account-management.md/#logging-in-to-the-account) first.

    ![Press edit button](mare-nostrum-thesaurus-management/press-edit-button.png)

1. Modify contents and press **"save"** after completing the change.
    
    ![Modify contents](mare-nostrum-thesaurus-management/modify-contents.png)

1. Wait for changes to be saved which is indicated by the reappearance of the **"edit"** button.

    ![Wait for change to be saved](mare-nostrum-thesaurus-management/wait-for-change-save.png)

---

### Deleting an Item

???+ note "Retrievable Data Loss"
    This action is not permanent, and the data can be undeleted.

???+ note "Log in before deleting"
    Deleting an item requires [logging in](account-management.md/#logging-in-to-the-account) first.

1. [Browse dictionaries](#browsing-dictionaries) to find the item you want to delete.

2. (optional) Make sure that the **"Tools"** pane is displayed on the right side of the selected page. If not, find the **"Tools"** menu in the upper-right corner of the main content area, expand it, and select the **"move to sidebar"** option.

    ![Expand tools pane](mare-nostrum-thesaurus-management/expand-tools-pane.png)

3. In the **"Actions"** section of the **"Tools"** pane, select **"Delete"**.

    ![Delete item button](mare-nostrum-thesaurus-management/delete-item-button.png)

4. If needed, select a deletion reason from the dropdown menu and provide additional details in the text field (if not, leave the default values). Then, click **"Delete page"** to remove the item from the Thesaurus.

    ![Delete page](mare-nostrum-thesaurus-management/delete-page.png)

5. After deletion, a confirmation message will be displayed.

    ![Confirmation message](mare-nostrum-thesaurus-management/deletion-confirmation.png)

## Downloading Content

1. [Search dictionary](#displaying-and-searching-hierarchical-data) to find items of interest.

2. Select the checkboxes next to them.

    ???+ note
        To select all values, check the parent item.

    ![Select checkboxes](mare-nostrum-thesaurus-management/select-checkboxes.png)

3. Move to the top of the page and click **"Download selected as Arches format"**.

    ???+ note
        As a result, a `selected_dictionary_name.rdf` file will be downloaded. You can import it to Arches.

    ![Download selected as Arches format](mare-nostrum-thesaurus-management/download-selected-as-arches-format.png)