---
title: XGRIDS Handheld LiDAR
sidebar_position: 1
---

## 1. Point Cloud Processing

Raw LiDAR data must first be processed and exported in `LixelStudio`. Refer to the manufacturer's user manual for detailed procedures.

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

Locate the colored point cloud file las in the processing output directory and select it for import.

![](/img/en-img/xgridslas.png)

### 3.2 Import Photos

Click Import Folder.

![](/img/en-img/xgridsimportimg.png)

Locate the `images` folder storing raw fisheye photos in the processing output directory and select it for import.

![](/img/en-img/xgridsimg.png)

### 3.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/xgridseditcamera.png)

Click Select from Database.

![](/img/en-img/xgridsdatabase.png)

Choose camera parameters matching your device model and configure all camera groups sequentially.

![](/img/en-img/xgridscamera.png)

### 3.4 Import POS

Click Import POS.

![](/img/en-img/xgridspos1.png)

Locate the POS file `img_traj.csv` in the processing output directory and select it for import.

![](/img/en-img/xgridspos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/xgridspos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/xgridscrs.png)

---

## 4. Select Outputs

Select a reconstruction template, or manually specify the required 3D output format and output coordinate system.

![](/img/en-img/xgridsoutputs.png)

---

## 5. Start Reconstruction

Click Start Reconstruction![](/img/en-img/start.png) to begin.