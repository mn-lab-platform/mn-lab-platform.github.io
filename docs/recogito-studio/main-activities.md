# Main Activities

This section provides information on:

- creating a new project,
- adding a new document,
- modifying document metadata (including Dublin Core), 
- creating a group,
- annotating TEI texts or PDF documents,
- annotating IIIF, JPG or PNG images,
- installing Geotagger plugin in your project,
- using Geotagger plugin,
- enabling the Mare Nostrum LAB thesaurus plugin,
- tagging annotations from the Mare Nostrum LAB thesaurus,
- creating an assignment,
- fulfilling an assignment.

---

## Create a New Project

???+ note "User priviledges"
    To create a new project, you need to have a proper organization role, which means having a `Professor` or `Admin` role. Further information can be found [here]().

1. [Login to Recogito Studio](account-management.md/#login-to-recogito-studio).

1. Press the **"New Project"** button in the top right corner of the page.

    ![New Project button](main-activities/new-project-button.png)

1. Provide the project name and description, set projects properties, and press the **"Create"** button.

    ???+ note "Project properties - Project Visibility"
        You can select two options in Project Visibility section:

        - **Private** - project is visible only to the admin and users who join after receiving an admin invitation.
        - **Public** - any registered user can access the project by visiting the **"Public Projects"** section.

    ???+ note "Project properties - Project Type"
        You can select two options in Project Type section:

        - **Assignments** - project admins create assignments with specific documents, and team members fulfil the given tasks.
        - **Single Team** - project members can annotate any document.

    ![Create a new project](main-activities/project-creation.png)

1. Upon creation, an empty project page will be displayed. 

    ![Empty project page](main-activities/creation-success.png)

---

## Add New Document

1. [Create](#create-new-project) or open a project.

1. Press the **"Add Document"** button in the top right corner.

    ![Add Document button](main-activities/add-document-button.png)

1. Press the **"Import"** button and select a file from your device or provide a IIIF manifest.

    ![Import Document button](main-activities/import-options.png)

1. (Optional) Go to the **"All documents"** section and select documents of interest from the list of publicly available ones across the organization.

    ![All Documents section](main-activities/public-documents.png)

1. Wait for processing, which ends with a confirmation message and a new document object.

    ???+ note
        To inspect the document from the adding panel, you need to refresh the page by hand.

    ![Import ended with success](main-activities/successful-import.png)

---

## Modify Document Metadata

### Method 1

1. Open a project, click the three dots in the object representing the document, and click **"Edit document metadata"**.

    ![Edit document metadata](main-activities/edit-document-metadata.png)

1. Add or modify document's metadata and save the changes.

    ???+ note
        Here, you can also change a name of the file in the Recogito Studio.

    ![Modify metadata](main-activities/modify-metadata.png)

    ???+ note "Dublin Core"
        The metadata form always lists the 15 Dublin Core elements: Contributor, Coverage, Creator, Date, Description, Format, Identifier, Language, Publisher, Relation, Rights, Source, Subject, Title, Type. Empty values are shown as `novalue`. Extra custom fields can still be added.

    ![Dublin Core document metadata](main-activities/dublin-core-metadata.png)

---

### Method 2

1. Open a project, click the "Add Document" button, and click three vertical dots next to the document of interest.

    ![Modify metadata](main-activities/method-2.png)

1. Here you can edit document metadata (see point 2 in **[Method 1](#method-1)**), change its status, or remove it from Recogito Studio.

    ???+ note "Make Public / Make Private"
        This option allows the user to change document accessibility. If status is `Private`, only users inside a specific project can see this document. If status is `Public`, any logged-in user can access this file via the **"All Documents"** section.

---

## Create a Project Group

???+ note "Groups"
    A **Group** is a dedicated tool allowing users to thematically aggregate projects (e.g., by source, year, or place).

1. On the main page, click the **"+"** button next to the **"Groups"** section, provide a name, and click the **"Create"** button.

    ![Create Groups](main-activities/create-group.png)

1. Go to the created group and add a project. You can select from existing or create a new project that will be assigned to that group.

    ![Add project to group](main-activities/add-project-to-group.png)

---

## Annotate TEI Texts and PDF Files

???+ note "Inspect annotations"
    You can inspect existing annotations by opening a dedicated pane on the right side of the page.

1. Choose and open a TEI or PDF document.

1. Mark the pieces of text you want to annotate, provide content for the annotation, and save them.

    ???+ note
        You can add tags to create thematic groups for the annotations.

    ???+ note
        You can add Web URL links, Image URL links and YouTube links to your annotation.

    ![TEI/PDF annotation](main-activities/text-annotation.png)

---

## Annotate IIIF, JPG and PNG Images

???+ note "Inspect annotations"
    You can inspect existing annotations by opening a dedicated pane on the right side of the page.

1. Choose and open a IIIF, JPG or PNG image.

1. Select the rectangular or multiangular marking mode, outline the elements of interest, provide annotation contents, and save.

    ???+ note
        You can add tags to create thematic groups for the annotations.

    ???+ note
        You can add Web URL links, Image URL links and YouTube links to your annotation.

    ![Image annotation](main-activities/image-annotation.png)

---

## Geotagger Plugin

### Install Plugin in Your Project

???+ note "Plugins availability"
    Note that plugins are available per project. This means you need to enable them in each project independently.

1. To enable a plugin, open a project as a **Project Admin**.

1. Go to **"Settings"**.

    ![Project Settings](main-activities/project-settings.png)

1. Next, press the **"Plugins"** tab, click the **"Browse Available Plugins"** button, and install the listed plugin.

    ![Install Plugin](main-activities/install-plugin.png)

1. Add gazetteers and save the settings.

    ???+ note "Plugin limitations"
        Unfortunatelly, the Core Data gazetteer does not work properly. Including it in your project may cause plugin instabilities.

    ![Add Gazetteers](main-activities/add-gazetteers.png)

---

### Annotate with Location

1. [Install plugin in your project](#install-plugin-in-your-project).

1. Mark the text or part of the image and click the **"Add Geo-Tag"** button.

    ![Add Geo-Tag](main-activities/add-geotag-button.png)

1. Provide a fragment of text. The plugin will automatically match the sentence with the closest tag in the gazetteers. If you are satisfied you can confirm it.

    ![Proposed location](main-activities/proposed-location.png)

1. (Optional) If you are not satisfied with the automatic proposition, click **"Change"**, type your text in the dedicated field and choose from displayed list or from the map points.

    ![Change location](main-activities/change-location-window.png)

---

## Mare Nostrum LAB thesaurus Plugin

This plugin tags annotations with concepts from the [Mare Nostrum LAB thesaurus](https://thesaurus.mn.cenagis.edu.pl), using the same Recogito plugin shape as Geotagger. It is installed per project.

### Enable the Plugin in Your Project

???+ note "Plugins availability"
    Plugins are available per project. Enable them in each project independently.

1. Open a project as a **Project Admin**.

1. Go to **"Settings"**.

    ![Project Settings](main-activities/project-settings.png)

1. Open the **"Plugins"** tab, click **"Browse Available Plugins"**, and install **Mare Nostrum Lab Thesaurus**.

    ![Install MN Thesaurus plugin](main-activities/install-mn-plugin.png)

1. In the plugin settings:

    - choose which dictionaries are searchable,
    - optionally keep **Use selected annotation text as the thesaurus search query** enabled (on by default).

    Dictionaries include amphora type, vessel form, vessel part, chronology, material, style, and the other MN vocabularies.

    ![MN Thesaurus plugin settings](main-activities/mn-plugin-settings.png)

---

### Annotate with a Thesaurus Tag

1. [Enable the plugin in your project](#enable-the-plugin-in-your-project).

1. Mark the text or part of the image, then click **"Add Mare Nostrum LAB thesaurus tag"**.

    ![Add MN thesaurus tag](main-activities/add-mn-tag.png)

1. Type a search string. The plugin queries the thesaurus over SPARQL and lists matching concepts (label, dictionary, description, id).

    ![MN thesaurus search](main-activities/mn-tag-search.png)

    ???+ note
        If search-from-selection is on, the selected annotation text is used as the initial query.

1. Select a concept. The tag is saved on the annotation and links to the item in the thesaurus. You can edit or remove it later from the same annotation.

    ![Saved MN thesaurus tag](main-activities/mn-tag-saved.png)

---

## Assignments

**Assignments** can be distributed by the `Project Admins` to `Project Students` and assigned with specific tasks. 

### Creating an Assignment

1. While creating a project, select `Project Type` as `Assignments`. If you omitted this part, go to project settings and set this variable manually. Remember to save the changes.

    ![Project Type - Assignments](main-activities/project-type-assignments.png)

1. (Optional) If you haven't done it yet, go to **"Users"** and invite the requested group of people as `Students`.

    ![Invite Users](main-activities/project-students.png)

1. Switch to the **"Assignments"** tab and click the **"Add Assignment"** button. Then, follow the four steps of creation, verify them as a fifth step, and create an assignment.

    ![Steps of assignment creation](main-activities/create-assignment.png)

---

### Fulfilling an Assignment

1. (Optional) If you haven't done it yet, join to the project via link, email invitation, or inside Recogito Studio.

    ![Join project](main-activities/join-project.png)

1. Go to **"Shared with me"** tab and find project you have joined.

    ???+ note
        If you have no assignments, the Project will appear from your perspective.

    ![Shared with me](main-activities/shared-with-me.png)

1. Open the documents and fulfill the assignments.

    ![Fulfill the assignment](main-activities/fulfill-assignment.png)