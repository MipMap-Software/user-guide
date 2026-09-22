# MipMap  Documentation

📖 简介

本项目是一套 MipMap 软件实操教程文档。

内容涵盖激光雷达数据导入，成果导出到UE、Unity、Blender等第三方软件的跨平台互通方案，整理了实操步骤与案例。

文档面向MipMap生态，旨在解决雷达数据导入、成果应用、多软件协同等常见问题。

[查看在线文档](https://docs.mipmap3d.com/guide/zh-Hans/)

## 安装和运行

### 安装Node

本文档开发需要先配置Node环境，访问[NodeJS官网](https://nodejs.org/zh-cn/download)下载LTS版本进行安装。

### 安装项目依赖

打开Windows终端，执行以下命令安装`yarn`。

```bash
npm install -g yarn
```

在本项目根目录下安装项目所需依赖：


```bash
yarn
```

需要更新文档时，执行以下命令启动开发服务：

```bash
yarn dev
```

开发服务启动后，可以在浏览器打开4002端口来预览文档，在编辑器中修改文档内容后，浏览器可以看到文档视图实时更新。

## 构建与部属

完成编辑后，执行以下命令生成部署安装包：

```bash
yarn build
```

构建完成后，将 `build/` 目录部署到你的托管服务。

