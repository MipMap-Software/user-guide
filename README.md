# MipMap Documentation

📖 Introduction

This project is a collection of practical tutorial documents for the MipMap software.

It covers laser LiDAR data import and cross-platform workflows for exporting outputs to third-party software including UE, Unity, Blender, with compiled operational procedures and case studies.

Targeted at the MipMap ecosystem, these documents address common challenges involving LiDAR data ingestion, result utilization, and multi-software collaboration.

[View the online documentation](https://docs.mipmap3d.com/guide/en/)

## Install and Run

### Install Node.js

Before working on this documentation project, install Node.js first. Visit the [Node.js official website](https://nodejs.org/en/download) and install the LTS version.

### Install Project Dependencies

Open a Windows terminal and run the following command to install `yarn`:

```bash
npm install -g yarn
```

Install all required dependencies in the project root directory:

```bash
yarn
```

When you need to update the docs, run the command below to start the development server:

```bash
yarn dev
```

After the development server starts, open port 4002 in your browser to preview the docs. Any content changes in the editor will be reflected in real time.

## Build and Deploy

After editing is complete, run the following command to generate the deployment package:

```bash
yarn build
```

After the build is finished, deploy the `build/` directory to your hosting service.

