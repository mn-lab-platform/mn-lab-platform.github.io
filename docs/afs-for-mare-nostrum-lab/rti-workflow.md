# RTI Workflow

This workflow imports a Reflectance Transformation Imaging (RTI) package and makes it available through the MN Lab RTI viewer.

## Before you start

- Create or open the resource to which the RTI will be attached.
- Prepare an RTI ZIP package containing the image planes and a JSON metadata manifest.
- The current RTI function expects three image planes in JPG, JPEG, or PNG format and one JSON manifest with the required RTI metadata.

## 1. Upload the RTI package

1. Open the RTI file card or workflow configured for the resource.
1. Upload the RTI ZIP package.
1. Save the resource or complete the upload workflow.

The system detects the ZIP package after it is saved. A package that does not contain the expected RTI content remains an ordinary file and is not processed as RTI.

## 2. Automatic processing

When the package is recognised as RTI, the Arches function:

1. reads the JSON manifest and validates the metadata;
1. extracts the image planes from the ZIP package;
1. creates Arches file records for the extracted images;
1. records the RTI dimensions, bias, and scale values with the files; and
1. removes the original ZIP package after successful processing.

The extracted images, not the ZIP package, become the files used by the viewer.

## 3. Open the RTI viewer

1. Open the resource report after processing is complete.
1. Open the Digital Resource view that contains the RTI component.
1. Wait for the viewer to load the generated manifest and image planes through the local IIIF service.
1. Use the interactive controls to inspect the RTI resource.

## Troubleshooting

| Problem | Check |
| --- | --- |
| The ZIP is not processed | Confirm that it contains exactly three JPG, JPEG, or PNG image planes and one JSON manifest. |
| The viewer is empty | Check that processing created image files and that the IIIF service is available. |
| The viewer cannot load metadata | Verify that the JSON manifest contains valid RTI dimensions and material data. |
| Processing stops with an error | Inspect the Arches application logs and confirm that the uploaded ZIP can be opened. |

## Technical notes

The RTI function runs after an RTI file card is saved. It stores the extracted image planes as normal Arches files and attaches the metadata required by the frontend component. The viewer requests a local RTI manifest endpoint and loads the processed planes from the IIIF service.
