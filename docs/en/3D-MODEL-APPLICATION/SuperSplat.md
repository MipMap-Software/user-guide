---
title: SuperSplat
sidebar_position: 1
---

# Editing Gaussian Splat Models in SuperSplat

## Import Gaussian Splat Models into SuperSplat

1. Open SuperSplat: https://superspl.at/editor
2. Top menu: `File → Import → Select Gaussian Splat file (PLY/SOG)`

![](/img/cn-img/supersplatimport.png)

3. Adjust position and rotation parameters on the left panel to center the model on the axis and level it.

![](/img/cn-img/旋转模型.png)

---

## Edit Gaussian Splat Models

### Remove Outlier Splats

1. Use the toolbar at the bottom to select outlier splats for removal.

2. Press the Delete key to erase selected outliers. Use Ctrl+Z to undo actions.

![](/img/cn-img/选择.png)

### Color Adjustment

If the colors of your Gaussian Splat model do not meet expectations, follow the steps below.

1. Click **Color** on the left to open the color parameter panel and adjust values as needed.

2. Click the settings icon on the right. In the tone mapping section, pick your desired filter.

![](/img/cn-img/高斯色彩调整.png)

## Export Gaussian Splat Models

1. Top menu: `File → Export → Select PLY/SOG`

![](/img/cn-img/导出高斯.png)

2. Choose an output folder for the exported file, click Export, and wait for the export progress to finish.

![](/img/cn-img/导出高斯2.png)

---

## Render a Flythrough Video

1. Click the timeline icon in the bottom-left corner.
2. Set the video frame rate and total frame count in the bottom-right panel.
3. Click on the timeline below to add flythrough keyframes.
4. Click Play to preview the flythrough animation.

![](/img/cn-img/录制视频.png)

5. Top menu: `Render → Video` to configure video settings.

![](/img/cn-img/渲染视频.png)

6. Click Render, select the save location for your video, and wait for rendering to complete.

![](/img/cn-img/渲染.gif)