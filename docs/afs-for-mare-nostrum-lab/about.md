# AfS for Mare Nostrum Lab

**AfS for Mare Nostrum Lab** is a customised deployment of [Arches for Science](https://www.archesproject.org/arches-for-science/) (AfS) for the management, processing, and presentation of archaeological digital resources. It combines the Arches data-management environment with MN Lab tools for deploying the platform, presenting 3D models, and processing Reflectance Transformation Imaging (RTI) resources.

The deployment code is maintained in the [AFS for MN Lab Excavation repository](https://github.com/mn-lab-platform/afs-for-mn-lab).

## Purpose

The project provides a shared environment in which archaeological resources can be documented together with their associated digital files. Its MN Lab extensions focus on files that need dedicated processing or viewers:

- 3D models supplied as PLY or OBJ files;
- compressed NXZ models for web presentation through 3DHOP;
- RTI packages containing image planes and metadata; and
- digital-resource reports that bring these files and viewers into the Arches interface.

## MN Lab extensions

### Deployment and operations

The upstream Docker deployment was adapted for the MN Lab environment. This work includes project-specific Docker Compose settings, Nginx configuration and start-up scripts, and adjustments to the application and frontend build configuration. The result is a deployable production-oriented stack rather than a stock local AfS installation.

### Custom interface and reports

MN Lab introduced a customised landing page, imagery, icons, and resource presentation. The platform includes custom report templates for digital resources, allowing specialised viewers to appear within the normal Arches resource interface instead of as separate applications.

### 3D model workflow

The project integrates [3DHOP](https://3dhop.net/) for browser-based presentation of high-resolution 3D models. The implementation includes:

- a dedicated Digital Resource viewer and report template;
- 3DHOP frontend assets and example NXZ models;
- an Arches function that detects uploaded PLY and OBJ files; and
- a conversion workflow that stores a generated NXZ file as a derivative of its source model.

To prepare models for the viewer, MN Lab added a separate **Nexus Converter** service. It exposes an API that converts PLY or OBJ files to NXS with Nexus tools and compresses the result to NXZ. The Arches 3DHOP function sends eligible files to this service, records the generated file in Arches, and avoids converting the same source file twice.

### RTI workflow

MN Lab also added an RTI processing workflow. An Arches function recognises an RTI ZIP package, validates its expected image and metadata content, extracts the image planes, stores them as Arches files, and records the RTI metadata required by the viewer.

The frontend includes a dedicated RTI viewer component and a manifest endpoint. The viewer loads the processed planes through the local IIIF service and uses the stored metadata to provide interactive RTI visualisation. The integration also includes viewer initialisation, visibility, orientation, and presentation refinements.

### Frontend integration

The implementation adds Leaflet and related frontend assets used by the custom visualisation work. It also includes updates to report components, resource display, styles, and build artefacts required to package the custom 3D and RTI functionality with the AfS application.

## Upstream, attribution, and licence

This project is a fork of [OpenContext's `arches-via-docker`](https://github.com/opencontext/arches-via-docker), built on its Arches for Science deployment work. MN Lab retains the upstream source history and the **GNU Affero General Public License v3.0 (AGPL-3.0)**.

The upstream deployment documentation remains available in the fork's [README](https://github.com/mn-lab-platform/afs-for-mn-lab#readme). This page documents the MN Lab-specific architecture and functionality added on top of that base.
