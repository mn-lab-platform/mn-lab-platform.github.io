# 3D Model Workflow

This workflow prepares an uploaded 3D model for web presentation in the MN Lab Arches interface. It uses the 3DHOP viewer and the Nexus Converter service to create an optimised `.nxz` derivative of an original model.

## Before you start

- Create or open the Digital Resource that will contain the model.
- Prepare a source model in **PLY** or **OBJ** format.
- Ensure that the 3DHOP conversion option is enabled for the resource. The conversion service must be running in the deployment.

## 1. Upload the source model

1. Open the Digital Resource in edit mode.
1. In the Files card, upload the PLY or OBJ file.
1. Save the resource.

Keep the original source file. The generated NXZ model is linked to it as a derivative; it is not a replacement for the source file.

## 2. Enable 3DHOP conversion

1. Open the 3DHOP configuration card for the resource.
1. Enable conversion.
1. If the card exposes Nexus conversion settings, enter the required processing parameters.
1. Save the card.

When the card is saved, the Arches function finds eligible PLY or OBJ files attached to the resource and sends them to the Nexus Converter.

## 3. Processing

The converter creates an intermediate NXS model and compresses it to NXZ. When conversion finishes, the generated `.nxz` file is saved in Arches alongside the source file and marked as derived from it.

The process is idempotent: if an NXZ derivative already exists for a source file, the system does not create a second copy.

## 4. View the model

1. Open the resource report.
1. Open the Digital Resource viewer.
1. Select the 3D view, if it is not displayed automatically.
1. Use the 3DHOP controls to inspect the model.

## Troubleshooting

| Problem | Check |
| --- | --- |
| No conversion starts | Confirm that conversion is enabled and that the uploaded file is PLY or OBJ. |
| Conversion fails | Confirm that the Nexus Converter container is running and inspect its service logs. |
| No model appears in the report | Check that an NXZ derivative was created and that the Digital Resource uses the 3DHOP report configuration. |
| A second conversion is needed | Remove or replace the existing NXZ derivative only when a new source model or conversion settings require it. |

## Technical notes

The Nexus Converter is a separate service in the deployment. It runs Nexus tools to convert PLY or OBJ files to NXS and then compresses them to NXZ. The Arches 3DHOP function sends the source file to that service, stores the returned file, and links it to the original upload.
