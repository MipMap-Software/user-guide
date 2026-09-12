---
title: CHCNAV Handheld LiDAR
sidebar_position: 1
---

## 1. Point Cloud Processing

Raw LiDAR data must first be processed and exported in `CoPre`. Refer to the manufacturer's user manual for detailed procedures.

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

Locate the `Results` folder in the processing output directory, open the folder matching your project name, and import all point cloud files inside the `Las` folder.

![](/img/en-img/chcnavlas.png)

### 3.2 Import Photos

Click Import Folder.

![](/img/en-img/chcnavimportimg.png)

Raw fisheye photos are stored in multiple `Camera` folders. Select all `Camera` folders for import.

![](/img/en-img/chcnavimg.png)

### 3.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/chcnaveditcamera.png)

Click Select from Database.

![](/img/en-img/chcnavdatabase.png)

Choose camera parameters matching your device model and configure all camera groups sequentially.

![](/img/en-img/chcnavcamera.png)

### 3.4 Import POS

Click Import POS.

![](/img/en-img/chcnavpos1.png)

POS data is stored across multiple `Camera` folders. Import the `OrbitPos.txt` file from each `Camera` folder one by one.

![](/img/en-img/chcnavpos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/chcnavpos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/chcnavcrs.png)

---

## 4. Select Outputs

Select a reconstruction template, or manually specify the required 3D output format and output coordinate system.

![](/img/en-img/chcnavoutputs.png)

---

## 5. Start Reconstruction

Click Start Reconstruction![](/img/en-img/start.png) to begin.