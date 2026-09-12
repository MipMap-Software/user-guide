---
title: FEIMA Handheld LiDAR
sidebar_position: 1
---

## 1. Point Cloud Processing

Raw LiDAR data must first be processed and exported in `Slam Go Post Pro`. Refer to the manufacturer's user manual for detailed procedures.

---

## 2. Create New Project

Click New Project![](/img/en-img/newproject1.png), enter the project name, and select LiDAR as the task type.

![](/img/en-img/newproject.png)


---

## 3. Import Data

Click Import LiDAR Data to open the import interface.

![](/img/en-img/importlidardata.png)

> [!tip] Different devices output different files. Follow the import workflow for your specific device.

### 3.1 Built-in Camera

#### 3.1.1 Import Point Cloud

Click Import Point Cloud.

![](/img/en-img/importpoint.png)

Locate the `texture` folder in the processing output directory and select the `.las` point cloud file for import.

![](/img/en-img/feimabuiltinlas.png)

#### 3.1.2 Import Photos

Click Import Folder.

![](/img/en-img/feimabuiltinimportimg.png)

Locate the `frames` folder in the processing output directory, then select photo folders `0` and `1` for import.

![](/img/en-img/feimabuiltinimg.png)

Images inside the masks folder do not need to be imported. Click the delete icon on the right to remove them.

![](/img/en-img/feimabuiltinmask.png)

#### 3.1.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/feimabuiltineditcamera.png)

Click Select from Database.

![](/img/en-img/feimabuiltindatabase.png)

Choose camera parameters matching your device model and configure all camera groups sequentially.

![](/img/en-img/feimabuiltincamera.png)

#### 3.1.4 Import POS

Click Import POS.

![](/img/en-img/feimabuiltinpos1.png)

Locate the `pos` folder in the processing output directory and select the POS file `camera_pos.txt` for import.

![](/img/en-img/feimabuiltinpos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/feimabuiltinpos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/feimabuiltincrs.png)

---

### 3.2 External Camera

#### 3.2.1 Import Point Cloud

Click Import Point Cloud.

![](/img/en-img/importpoint.png)

Locate the `texture` folder in the processing output directory and select the `.las` point cloud file for import.

![](/img/en-img/feimaexternallas.png)

#### 3.2.2 Import Photos

Click Import Folder.

![](/img/en-img/feimaexternalimportimg.png)

Locate the `images` folder in the processing output directory, then select photo folders `0` and `1` for import.

![](/img/en-img/feimaexternalimg.png)

#### 3.2.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/feimaexternaleditcamera.png)

Click Select from Database.

![](/img/en-img/feimaexternaldatabase.png)

Choose camera parameters matching your device model and configure all camera groups sequentially.

![](/img/en-img/feimaexternalcamera.png)

#### 3.2.4 Import POS

Click Import POS.

![](/img/en-img/feimaexternalpos1.png)

Locate the `sfm_pos` folder in the processing output directory and select the POS file `sfm_data_mipmap.txt` for import.

![](/img/en-img/feimaexternalpos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/feimaexternalpos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/feimaexternalcrs.png)

---

### 3.3 SLAM 100

#### 3.3.1 Import Point Cloud

Click Import Point Cloud.

![](/img/en-img/importpoint.png)

Open the processing output directory and select the `.las` point cloud file for import.

![](/img/en-img/feimaslam100las.png)

#### 3.3.2 Import Photos

Click Import Folder.

![](/img/en-img/feimaslam100importimg.png)

Open the original project directory and select photo folders `camera0`, `camera1`, and `camera2` for import.

![](/img/en-img/feimaslam100img.png)

#### 3.3.3 Select Camera Parameters

Click Edit Camera to open the camera parameter panel.

![](/img/en-img/feimaslam100editcamera.png)

Click Select from Database.

![](/img/en-img/feimaslam100database.png)

Choose camera parameters matching your device model and configure all camera groups sequentially.

![](/img/en-img/feimaslam100camera.png)

#### 3.3.4 Import POS

Click Import POS.

![](/img/en-img/feimaslam100pos1.png)

Locate the `pos` folder in the processing output directory and select the POS file `camera_pos_opk.txt` for import.

![](/img/en-img/feimaslam100pos2.png)

Set attitude angles and column mappings as shown below during POS import.

![](/img/en-img/feimaslam100pos3.png)

The coordinate system must match the one used in the point cloud processing project.

![](/img/en-img/feimaslam100crs.png)

## 4. Select Outputs

Select a reconstruction template, or manually specify the required 3D output format and output coordinate system.

![](/img/en-img/feimaslam100outputs.png)

---

## 5. Start Reconstruction

Click Start Reconstruction![](/img/en-img/start.png) to begin.