---
title: SHARE Handheld LiDAR
sidebar_position: 1
---

# SHARE Handheld LiDAR

## 1. Point Cloud Processing

Raw LiDAR data must first be processed and exported in `SHARE PointClouds Studio`. Refer to the manufacturer's user manual for detailed procedures.

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

Locate the colored point cloud file `_colorized.las` in the processing output directory and select it for import.

![](/img/en-img/sharelas.png)

### 3.2 Import Photos

Click Import Folder.

![](/img/en-img/shareimportimg.png)

Open the processing output directory, locate the undistort folder, then select the `left` and `right` folders for import.

![](/img/en-img/shareimg.png)


### 3.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/shareeditcamera.png)

Click Import opt File.

![](/img/en-img/shareopt.png)

For the `left` camera, select `Left_undistort.opt`; for the `right` camera, select `Right_undistort.opt`.

![](/img/en-img/shareopt2.png)

### 3.4 Import POS

Click Import POS.

![](/img/en-img/sharepos1.png)

Open the processing output directory, locate the undistort folder, then select the POS file `ImgPose.txt` for import.

![](/img/en-img/sharepos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/sharepos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/sharecrs.png)

---

## 4. Select Outputs

Select a reconstruction template, or manually specify the required 3D output format and output coordinate system.

![](/img/en-img/shareoutputs.png)

---

## 5. Start Reconstruction

Click Start Reconstruction![](/img/en-img/start.png) to begin.