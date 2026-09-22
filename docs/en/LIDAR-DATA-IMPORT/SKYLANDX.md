---
title: SKYLANDX Handheld LiDAR
sidebar_position: 1
---

# SKYLANDX Handheld LiDAR

## 1. Point Cloud Processing

Raw LiDAR data must first be processed and exported in `MetaCam Studio`. Refer to the manufacturer's user manual for detailed procedures.

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

Locate the colored point cloud file `colorized.las` in the processing output directory and select it for import.

![](/img/en-img/skylandxlas.png)

### 3.2 Import Photos

Click Import Folder.

![](/img/en-img/skylandximportimg.png)

Open the original project directory, locate the `camera` folder storing raw fisheye photos, then select it for import.

![](/img/en-img/skylandximg.png)

### 3.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/skylandxeditcamera.png)

Click Select from Database.

![](/img/en-img/skylandxdatabase.png)

Choose camera parameters matching your device model and configure all camera groups sequentially.

![](/img/en-img/skylandxcamera.png)

### 3.4 Import POS

Click Import POS.

![](/img/en-img/skylandxpos1.png)

Locate the POS file `ImgPose.txt` in the processing output directory and select it for import.

![](/img/en-img/skylandxpos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/skylandxpos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/skylandxcrs.png)

---

## 4. Select Outputs

Select a reconstruction template, or manually specify the required 3D output format and output coordinate system.

![](/img/en-img/skylandxoutputs.png)

---

## 5. Start Reconstruction

Click Start Reconstruction![](/img/en-img/start.png) to begin.