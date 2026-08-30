# Access Control & Permissions

Arches for JU Excavations utilizes custom authentication groups to manage access to specialized tools and sensitive spatial data. These groups are generated automatically when the application starts, and permissions are pre-assigned by the system. 

System administrators must manually assign users to these groups via the Arches user management interface to grant them access to these features.

## Plugin Access
By default, custom plugins are restricted. To view and utilize custom plugins within the Arches interface, a user must be assigned to the **Plugin Access** group. 

This group explicitly grants view permissions to the following tools:
* **Map Plugin:** The 2D MapLibre-based continuous workspace.
* **Cesium Plugin:** The 3D spatial excavation viewer.
* **Init Workflow Plugin:** The specialized initialization workflow launcher.

## Restricted Basemap Access
The application supports the uploading and serving of custom, high-resolution GeoTIFF basemaps. If a basemap overlay layer is designated as private or sensitive, its tile server is gated behind the **Restricted Basemap Access** group. 

Users must be members of this group to view and render these private basemap tiles within the Map Plugin or any other spatial interface in the application.