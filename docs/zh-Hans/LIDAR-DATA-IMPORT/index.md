---
title: 激光雷达数据导入
---

# <span class="title-gradient">激光雷达数据导入指南</span>

<div class="section-block">

- 以下为明确支持的设备厂商，您可按流程导入激光雷达数据进行重建。        
- 若您的设备不在支持列表中，请确认是否符合必备数据要求，符合即可尝试导入重建。
- 有任何问题可联系技术支持协助。
</div>

## 支持设备
<div class="device-grid">
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/CHCNAV">
  <div class="card-logo">
    <img src="/img/logo/CHCNAV.webp" alt="CHCNAV">
  </div>
  <div class="card-desc">华测导航手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/FEIMA">
  <div class="card-logo">
    <img src="/img/logo/FEIMA.webp" alt="FEIMA">
  </div>
  <div class="card-desc">飞马手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/GEOSUN">
  <div class="card-logo">
    <img src="/img/logo/GEOSUN.webp" alt="GEOSUN">
  </div>
  <div class="card-desc">际上导航手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/GOSLAM">
  <div class="card-logo">
    <img src="/img/logo/GOSLAM.webp" alt="GOSLAM">
  </div>
  <div class="card-desc">GOSLAM手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/MANIFOLD">
  <div class="card-logo">
    <img src="/img/logo/MANIFOLD.webp" alt="MANIFOLD">
  </div>
  <div class="card-desc">留形手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/OmniSLAM">
  <div class="card-logo">
    <img src="/img/logo/OmniSLAM.webp" alt="OmniSLAM">
  </div>
  <div class="card-desc">欧思徕手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/SHARE">
  <div class="card-logo">
    <img src="/img/logo/SHARE.webp" alt="SHARE">
  </div>
  <div class="card-desc">赛尔手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/SKYLANDX">
  <div class="card-logo">
    <img src="/img/logo/SKYLANDX.webp" alt="SKYLANDX">
  </div>
  <div class="card-desc">无穹手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/SOUTH">
  <div class="card-logo">
    <img src="/img/logo/SOUTH.webp" alt="SOUTH">
  </div>
  <div class="card-desc">南方测绘手持激光雷达</div>
</a>
<a class="device-card" href="/zh-Hans/LIDAR-DATA-IMPORT/XGRIDS">
  <div class="card-logo">
    <img src="/img/logo/XGRIDS.webp" alt="XGRIDS">
  </div>
  <div class="card-desc">其域手持激光雷达</div>
</a>
</div>


## 必备数据要求
<div class="spec-wrap">
<div class="spec-item">
<strong>📁 彩色点云 .las 文件</strong>
<p>点云内部必须包含时间戳字段，时间戳需要与POS文件时间戳匹配对齐。</p>
</div>
<div class="spec-item">
<strong>🖼️ 照片文件</strong>
<p>支持去畸变照片、原始鱼眼照片。</p>
</div>
<div class="spec-item">
<strong>📄 相机 POS 文件</strong>
<p>必填字段：时间戳、照片名、X、Y、Z<br/>姿态角为可选字段</p>
</div>
<div class="spec-item">
<strong>🌐 坐标系</strong>
<p>LAS点云坐标与POS坐标必须处于同一坐标系</p>
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