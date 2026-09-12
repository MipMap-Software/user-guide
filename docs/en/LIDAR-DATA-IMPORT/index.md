---
title: LiDAR Data Import Guide
---

# <span class="title-gradient">LiDAR Data Import Guide</span>

<div class="section-block">

- The following lists supported device manufacturers. You may import LiDAR data for reconstruction following the workflow.        
- If your device is not on the support list, check if it meets the mandatory data requirements. Data that satisfies the requirements can be imported for reconstruction.
- Contact technical support for assistance if you encounter any issues.
</div>

## Supported Devices
<div class="device-grid">
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/CHCNAV">
  <div class="card-logo">
    <img src="/img/logo/CHCNAV.webp" alt="CHCNAV">
  </div>
  <div class="card-desc">CHCNAV Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/FEIMA">
  <div class="card-logo">
    <img src="/img/logo/FEIMA.webp" alt="FEIMA">
  </div>
  <div class="card-desc">FEIMA Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/GEOSUN">
  <div class="card-logo">
    <img src="/img/logo/GEOSUN.webp" alt="GEOSUN">
  </div>
  <div class="card-desc">GEOSUN Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/GOSLAM">
  <div class="card-logo">
    <img src="/img/logo/GOSLAM.webp" alt="GOSLAM">
  </div>
  <div class="card-desc">GOSLAM Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/MANIFOLD">
  <div class="card-logo">
    <img src="/img/logo/MANIFOLD.webp" alt="MANIFOLD">
  </div>
  <div class="card-desc">MANIFOLD Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/OmniSLAM">
  <div class="card-logo">
    <img src="/img/logo/OmniSLAM.webp" alt="OmniSLAM">
  </div>
  <div class="card-desc">OmniSLAM Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/SHARE">
  <div class="card-logo">
    <img src="/img/logo/SHARE.webp" alt="SHARE">
  </div>
  <div class="card-desc">SHARE Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/SKYLANDX">
  <div class="card-logo">
    <img src="/img/logo/SKYLANDX.webp" alt="SKYLANDX">
  </div>
  <div class="card-desc">SKYLANDX Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/SOUTH">
  <div class="card-logo">
    <img src="/img/logo/SOUTH.webp" alt="SOUTH">
  </div>
  <div class="card-desc">SOUTH Handheld LiDAR</div>
</a>
<a class="device-card" href="/en/LIDAR-DATA-IMPORT/XGRIDS">
  <div class="card-logo">
    <img src="/img/logo/XGRIDS.webp" alt="XGRIDS">
  </div>
  <div class="card-desc">XGRIDS Handheld LiDAR</div>
</a>
</div>


## Mandatory Data Requirements
<div class="spec-wrap">
<div class="spec-item">
<strong>📁 Colored Point Cloud .las File</strong>
<p>The point cloud must contain timestamp fields, which must be time-aligned and matched with the POS file.</p>
</div>
<div class="spec-item">
<strong>🖼️ Image Files</strong>
<p>Undistorted photos and raw fisheye photos are supported.</p>
</div>
<div class="spec-item">
<strong>📄 Camera POS File</strong>
<p>Mandatory fields: Timestamp, Image Name, X, Y, Z<br/>Attitude angles are optional fields</p>
</div>
<div class="spec-item">
<strong>🌐 Coordinate System</strong>
<p>The LAS point cloud and POS coordinates must use the same coordinate system</p>
</div>
</div>

<style>
.title-gradient {
  background: linear-gradient(135deg, #3b82f6, #0ea5e9);
  -webkit-background-clip: text;
  color: transparent;
  display:block;
  margin-bottom:20px;
}
.section-block {
  padding: 6px 20px;
  border-left: 3px solid var(--vp-c-brand);
  background: var(--vp-c-bg-soft);
  border-radius: 0 8px 8px 0;
  margin-bottom: 20px;
  line-height: 1.7;
}
.device-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 16px;
  margin-bottom: 20px;
}
.device-card {
  display: block;
  padding: 20px;
  border: 1px solid var(--vp-c-divider);
  border-radius: 12px;
  text-decoration: none !important;
  transition: all 0.24s ease;
  background: #27272ac0; 
}
.device-card:hover {
  transform: translateY(-4px);
  border-color: var(--vp-c-brand);
  box-shadow: 0 8px 24px rgba(0,0,0,0.18);
}
.card-logo {
  height: 64px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 14px;
}
.card-logo img {
  max-height: 54px;
  max-width: 50%;
  object-fit: contain;
}
.device-card .card-desc {
  font-size: 16px;
  color: #eaeaee;
  text-align:center;
}
.spec-wrap {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(240px,1fr));
  gap:16px;
  margin-bottom:32px;
}
.spec-item {
  padding:18px;
  border-radius:10px;
  background: var(--vp-c-bg-soft);
}
.spec-item strong {
  display:block;
  margin-bottom:6px;
}
@media (max-width: 640px) {
  .card-logo img {
    max-height: 38px;
    max-width: 50%;
  }
  .card-logo {
    height: 52px;
    margin-bottom:10px;
  }
}
</style>