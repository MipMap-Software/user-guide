---
title: Blender
sidebar_position: 1
---

# Import 3D Model Outputs into Blender

## Gaussian Splat PLY Models

> [!tip] Compatible with Blender 5.3 and newer. Native Gaussian Splat PLY loading is not supported in versions older than 5.3.

1. Launch Blender, create a new blank project and delete the default cube.
2. Top menu: `File → Import → Stanford PLY`

![](/img/en-img/ply_blender.png)

3. In the file browser, select the PLY file reconstructed by MipMapDesktop.

![](/img/en-img/ply_blender2.png)

4. Adjust rotation parameters on the right panel to level the model.

![](/img/en-img/ply_blender3.png)

5. Disable outline display at the top-right corner. Set the shading mode to **Material Preview** or **Rendered** to view the Gaussian splat model.

![](/img/en-img/ply_blender4.png)

---

## Mesh Models: OBJ / FBX

Mesh models are exported as tiled files by default. For small scenes, you can merge them into a single model file for easier downstream workflows.

Merging and exporting large scenes requires substantial memory. If merging fails, **import each tiled file one by one**.

![](/img/en-img/merge.png)

1. Launch Blender, create a new blank project and delete the default cube.
2. Top menu: `File → Import → Wavefront OBJ / FBX`

![](/img/en-img/obj_blender.png)

3. In the file browser, select the OBJ or FBX file exported by MipMapDesktop.

![](/img/en-img/obj_blender2.png)

4. Adjust rotation parameters on the right panel to level the model.

![](/img/en-img/obj_blender3.png)

5. Disable outline display at the top-right corner. Set the shading mode to **Material Preview** or **Rendered** to display model textures.

![](/img/cn-img/obj渲染.png)