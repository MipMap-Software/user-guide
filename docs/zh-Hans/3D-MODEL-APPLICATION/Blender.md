---
title: Blender
sidebar_position: 1
---

# 三维模型成果导入 Blender 教程

## 高斯泼溅模型 PLY

> [!tip] 适用 Blender5.3 及以上版本，低于5.3版本不支持原生高斯泼溅ply加载。

1. 启动 Blender，新建空白工程，删除默认立方体。
2. 顶部菜单：`文件 → 导入 → Stanford PLY`

![](/img/cn-img/ply.png)

3. 在文件浏览器，选择MipMapDesktop重建的PLY文件。

![](/img/cn-img/ply2.png)

4. 右侧可调整旋转参数，将模型置平。

![](/img/cn-img/ply3.png)

5. 右上角可关闭轮廓线显示，着色方式选择**材质预览**或**渲染**即可显示高斯泼溅模型。

![](/img/cn-img/ply4.png)

---

## 网格模型OBJ / FBX

网格模型默认为分块文件，小场景可导出合并为单个模型文件，方便后续操作。

大场景合并导出需要较大内存，若合并失败，则需**依次导入每个分块文件**即可。

![](/img/cn-img/成果合并.png)


1. 启动 Blender，新建空白工程，删除默认立方体。
2. 顶部菜单：`文件 → 导入 → Wavefront OBJ/FBX`

![](/img/cn-img/obj.png)

3. 在文件浏览器，选择MipMapDesktop导出的OBJ/FBX文件。

![](/img/cn-img/obj2.png)

4. 右侧可调整旋转参数，将模型置平。

![](/img/cn-img/旋转obj.png)

5. 右上角可关闭轮廓线显示，着色方式选择**材质预览**或**渲染**即可显示模型纹理。

![](/img/cn-img/obj渲染.png)




