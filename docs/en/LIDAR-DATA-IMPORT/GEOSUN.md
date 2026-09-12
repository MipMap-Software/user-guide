---
title: GEOSUN Handheld LiDAR
sidebar_position: 1
---

# GEOSUN Handheld LiDAR

## 1. Point Cloud Processing

Raw LiDAR data must first be processed and exported in `PointCloudCreator`. Refer to the manufacturer's user manual for detailed procedures.

All photos in the original `image` folder need to be sorted by suffix for separate lenses. Create two new folders named R and L.

Move photos with the `-R` suffix into the R folder, and photos with the `-L` suffix into the L folder.

![](/img/en-img/geosunlr.png)

---

## 2. Create New Project

Click New Project![](/img/en-img/newproject1.png), enter the project name, and select LiDAR as the task type.

![](/img/en-img/newproject.png)

---

## 3. Import Data

Click Import LiDAR Data to open the import interface.

![](/img/en-img/importlidardata.png)

### 3.1 Import Point Cloud

Click Import Point Cloud.

![](/img/en-img/importpoint.png)

Locate the `ResultOut` folder in the processing output directory and select the LAS point cloud file for import.

![](/img/en-img/geosunlas.png)

### 3.2 Import Photos

Click Import Folder.

![](/img/en-img/geosunimportimg.png)

Open the original project directory, locate the `image` folder storing raw fisheye photos, then select the created `L` and `R` folders for import.

![](/img/en-img/geosunimg.png)

### 3.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/geosuneditcamera.png)

Click Select from Database.

![](/img/en-img/geosundatabase.png)

Choose camera parameters matching your device model and configure all camera groups sequentially.

![](/img/en-img/geosuncamera.png)

### 3.4 Import POS

Click Import POS.

![](/img/en-img/geosunpos1.png)

Locate the POS file `CameraPos_C2E.txt` in the processing output directory and select it for import.

![](/img/en-img/geosunpos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/geosunpos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/geosuncrs.png)

---

## 4. Select Outputs

Select a reconstruction template, or manually specify the required 3D output format and output coordinate system.

![](/img/en-img/geosunoutputs.png)

---

## 5. Start Reconstruction

Click Start Reconstruction![](/img/en-img/start.png) to begin.