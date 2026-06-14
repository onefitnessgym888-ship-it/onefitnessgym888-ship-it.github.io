---
title: 空間介紹
date: 2026-06-14 15:56:20
type: "gallery"
---

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"/>

<style>
/* 限制範圍在 gym-gallery 內，避免干擾 Hexo 原生主題 */
.gym-gallery {
  color: var(--text-color, #f0f0f0);
  line-height: 1.6;
  padding-bottom: 40px;
}
.gym-gallery .section-title {
  text-align: center;
  margin: 50px 0 30px;
}
.gym-gallery .section-title h2 {
  font-size: 2.2rem;
  color: #4ecdc4;
  font-weight: 700;
  letter-spacing: 1.5px;
  border-bottom: none;
  padding-bottom: 0;
}
.gym-gallery .equipment-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
  gap: 35px;
  margin-top: 20px;
  align-items: start;
}
.gym-gallery .equipment-card {
  background: rgba(30, 45, 60, 0.35);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 16px;
  overflow: hidden;
  box-shadow: 0 10px 30px rgba(0,0,0,0.15);
  display: flex;
  flex-direction: column;
  transition: transform .3s ease, box-shadow .3s ease, border-color .3s ease;
}
.gym-gallery .equipment-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 15px 35px rgba(78, 205, 196, 0.15);
  border-color: rgba(78, 205, 196, 0.5);
}
.gym-gallery .card-content {
  display: flex;
  align-items: flex-start;
}
.gym-gallery .image-container {
  flex: 0 0 45%;
  position: relative;
  padding-top: 56%;
  overflow: hidden;
}
.gym-gallery .equipment-image {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform .6s ease;
  margin: 0 !important; /* 蓋掉 Hexo 預設圖片外距 */
}
.gym-gallery .image-container:hover .equipment-image {
  transform: scale(1.06);
}
.gym-gallery .card-header {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 15px 18px;
  background: linear-gradient(to top, rgba(0,0,0,0.85), transparent);
  z-index: 2;
}
.gym-gallery .card-header h3 {
  color: #fff !important;
  margin: 0 !important;
  font-size: 1.15rem;
  font-weight: 700;
  letter-spacing: .5px;
  text-shadow: 0 1px 4px rgba(0,0,0,0.7);
  line-height: 1.4;
}
.gym-gallery .info {
  flex: 1;
  padding: 24px;
  display: flex;
  flex-direction: column;
}
.gym-gallery .description-text {
  color: rgba(255,255,255,0.8);
  font-size: 0.95rem;
  line-height: 1.7;
  margin-bottom: 16px;
  text-align: justify;
}
.gym-gallery .description-text strong {
  color: #4ecdc4;
  font-weight: 600;
}
.gym-gallery .toggle-btn {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: none;
  border: none;
  border-top: 1px dashed rgba(255, 255, 255, 0.15);
  padding: 14px 0 0;
  cursor: pointer;
  width: 100%;
  color: #fff;
  font-size: 0.95rem;
  font-weight: 600;
  letter-spacing: .5px;
}
.gym-gallery .toggle-btn .btn-icon {
  color: #4ecdc4;
  margin-right: 8px;
}
.gym-gallery .toggle-btn .arrow {
  color: #4ecdc4;
  font-size: .85rem;
  transition: transform .3s ease;
}
.gym-gallery .toggle-btn.open {
  color: #4ecdc4;
}
.gym-gallery .toggle-btn.open .arrow {
  transform: rotate(180deg);
}
.gym-gallery .feature-wrap {
  max-height: 0;
  overflow: hidden;
  transition: max-height .4s ease;
}
.gym-gallery .feature-wrap.open {
  max-height: 400px;
}
.gym-gallery .feature-list {
  list-style: none !important;
  padding: 10px 0 4px !important;
  margin: 0 !important;
}
.gym-gallery .feature-list li {
  font-size: .9rem;
  color: rgba(255,255,255,0.85);
  padding: 6px 0 6px 28px !important;
  position: relative;
  line-height: 1.5;
  margin: 0 !important;
}
.gym-gallery .feature-list li i {
  position: absolute;
  left: 0;
  top: 9px;
  color: #ff6b6b;
  font-size: .85rem;
}

@media(max-width: 1100px){
  .gym-gallery .equipment-grid {
    grid-template-columns: 1fr;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
  }
  .gym-gallery .card-content {
    flex-direction: column;
  }
  .gym-gallery .image-container {
    flex: none;
    width: 100%;
    padding-top: 55%;
  }
}
</style>

<div class="gym-gallery">

  <div class="section-title"><h2>重訓器材</h2></div>
  <div class="equipment-grid">
    <!-- 卡片 1 -->
    <div class="equipment-card">
      <div class="card-content">
        <div class="image-container">
          <img src="https://onefitnessgym.com/wp-content/uploads/2025/08/史密推舉-scaled.jpg" alt="多功能三合一史密斯" class="equipment-image"/>
          <div class="card-header"><h3>多功能三合一史密斯訓練架</h3></div>
        </div>
        <div class="info">
          <div class="description-text">本工作室配備商用級 <strong>三合一多功能史密斯訓練架</strong>，滿足全身肌力與功能性訓練需求。</div>
          <button class="toggle-btn" onclick="toggleGymFeature(this)">
            <span><i class="fas fa-dumbbell btn-icon"></i>功能重點</span>
            <i class="fas fa-chevron-down arrow"></i>
          </button>
          <div class="feature-wrap">
            <ul class="feature-list">
              <li><i class="fas fa-shield-alt"></i> <strong>史密斯導軌：</strong>軌跡固定，安全穩定。</li>
              <li><i class="fas fa-sliders-h"></i> <strong>可調滑輪：</strong>多角度強化肌肉控制。</li>
              <li><i class="fas fa-layer-group"></i> <strong>自由槓：</strong>提升核心協調。</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <!-- 卡片 2 -->
    <div class="equipment-card">
      <div class="card-content">
        <div class="image-container">
          <img src="https://onefitnessgym.com/wp-content/uploads/2025/07/多功能深蹲架-1-scaled.jpg" alt="自由重量多功能訓練架" class="equipment-image"/>
          <div class="card-header"><h3>自由重量多功能訓練架</h3></div>
        </div>
        <div class="info">
          <div class="description-text">提供高度自由的訓練環境，更能有效訓練核心穩定及力量傳導。</div>
          <button class="toggle-btn" onclick="toggleGymFeature(this)">
            <span><i class="fas fa-dumbbell btn-icon"></i>功能重點</span>
            <i class="fas fa-chevron-down arrow"></i>
          </button>
          <div class="feature-wrap">
            <ul class="feature-list">
              <li><i class="fas fa-cube"></i> <strong>自由重量：</strong>複合式大動作必備。</li>
              <li><i class="fas fa-random"></i> <strong>高自由度：</strong>適合功能性整合訓練。</li>
              <li><i class="fas fa-arrows-alt-v"></i> <strong>可調滑輪：</strong>輔助小肌群訓練。</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="section-title"><h2>自由重量器材</h2></div>
  <div class="equipment-grid">
    <!-- 卡片 3 -->
    <div class="equipment-card">
      <div class="card-content">
        <div class="image-container">
          <img src="https://onefitnessgym.com/wp-content/uploads/2026/03/啞鈴-1-scaled.jpg" alt="啞鈴" class="equipment-image"/>
          <div class="card-header"><h3>啞鈴</h3></div>
        </div>
        <div class="info">
          <div class="description-text">最經典的自由重量訓練工具，是用於 <strong>肌力、肌肥大或功能性訓練</strong> 的必備器材，訓練部位涵蓋全身。</div>
          <button class="toggle-btn" onclick="toggleGymFeature(this)">
            <span><i class="fas fa-dumbbell btn-icon"></i>功能重點</span>
            <i class="fas fa-chevron-down arrow"></i>
          </button>
          <div class="feature-wrap">
            <ul class="feature-list">
              <li><i class="fas fa-weight-hanging"></i> <strong>多重量：</strong>適合各階段。</li>
              <li><i class="fas fa-random"></i> <strong>靈活操作：</strong>單／雙手皆可，孤立或協調訓練均適合。</li>
              <li><i class="fas fa-shield-alt"></i> <strong>安全提示：</strong>選適當重量，控制動作避免甩動。</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <!-- 卡片 4 -->
    <div class="equipment-card">
      <div class="card-content">
        <div class="image-container">
          <img src="https://onefitnessgym.com/wp-content/uploads/2025/07/S__90546210.jpg" alt="壺鈴" class="equipment-image"/>
          <div class="card-header"><h3>壺鈴</h3></div>
        </div>
        <div class="info">
          <div class="description-text">結合 <strong>力量與有氧</strong> 的多功能訓練神器，能有效提升核心穩定性與全身肌肉協調性。</div>
          <button class="toggle-btn" onclick="toggleGymFeature(this)">
            <span><i class="fas fa-dumbbell btn-icon"></i>功能重點</span>
            <i class="fas fa-chevron-down arrow"></i>
          </button>
          <div class="feature-wrap">
            <ul class="feature-list">
              <li><i class="fas fa-running"></i> <strong>多樣化：</strong>甩壺、深蹲、硬舉、推舉均適用。</li>
              <li><i class="fas fa-bullseye"></i> <strong>核心強化：</strong>重心特殊，需高度核心穩定。</li>
              <li><i class="fas fa-shield-alt"></i> <strong>安全提示：</strong>輕重量熟悉動作，收緊核心保護腰椎。</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="section-title"><h2>有氧與輔助器材</h2></div>
  <div class="equipment-grid">
    <!-- 卡片 5 -->
    <div class="equipment-card">
      <div class="card-content">
        <div class="image-container">
          <img src="https://onefitnessgym.com/wp-content/uploads/2025/07/跑步機-1-scaled.jpg" alt="跑步機" class="equipment-image"/>
          <div class="card-header"><h3>跑步機</h3></div>
        </div>
        <div class="info">
          <div class="description-text">標準有氧訓練器材，適合進行心肺耐力訓練與熱身。</div>
          <button class="toggle-btn" onclick="toggleGymFeature(this)">
            <span><i class="fas fa-heartbeat btn-icon"></i>功能重點</span>
            <i class="fas fa-chevron-down arrow"></i>
          </button>
          <div class="feature-wrap">
            <ul class="feature-wrap">
              <ul class="feature-list">
                <li><i class="fas fa-check"></i> 提升心肺耐力與燃脂</li>
                <li><i class="fas fa-check"></i> 多段速度／坡度模擬</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- 卡片 6 -->
    <div class="equipment-card">
      <div class="card-content">
        <div class="image-container">
          <img src="https://onefitnessgym.com/wp-content/uploads/2025/07/輪-scaled.jpg" alt="風扇車" class="equipment-image"/>
          <div class="card-header"><h3>風扇車</h3></div>
        </div>
        <div class="info">
          <div class="description-text">全身性 HIIT 神器，阻力隨風扇轉速自動調整。</div>
          <button class="toggle-btn" onclick="toggleGymFeature(this)">
            <span><i class="fas fa-wind btn-icon"></i>功能重點</span>
            <i class="fas fa-chevron-down arrow"></i>
          </button>
          <div class="feature-wrap">
            <ul class="feature-list">
              <li><i class="fas fa-check"></i> 阻力隨速度增加</li>
              <li><i class="fas fa-check"></i> 高效燃脂與肌耐力</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="section-title"><h2>爆發力與平衡訓練</h2></div>
  <div class="equipment-grid">
    <!-- 卡片 7 -->
    <div class="equipment-card">
      <div class="card-content">
        <div class="image-container">
          <img src="https://onefitnessgym.com/wp-content/uploads/2026/03/IMG_20260316_103303-scaled.jpg" alt="跳箱、藥球、平衡球" class="equipment-image"/>
          <div class="card-header"><h3>跳箱<br>藥球<br>平衡球</h3></div>
        </div>
        <div class="info">
          <div class="description-text">整合 <strong>爆發力、協調性與核心穩定</strong> 的多功能訓練組合，適合暖身活化、功能性訓練與運動表現提升。</div>
          <button class="toggle-btn" onclick="toggleGymFeature(this)">
            <span><i class="fas fa-bolt btn-icon"></i>功能重點</span>
            <i class="fas fa-chevron-down arrow"></i>
          </button>
          <div class="feature-wrap">
            <ul class="feature-list">
              <li><i class="fas fa-layer-group"></i> <strong>跳箱：</strong>可堆疊調整高度，訓練下肢爆發力與落地控制。</li>
              <li><i class="fas fa-circle"></i> <strong>藥球：</strong>投擲、深蹲加壓，強化核心與上肢連動。</li>
              <li><i class="fas fa-sync-alt"></i> <strong>平衡球：</strong>提升本體感覺，搭配動作增加難度。</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>

</div>

<script>
function toggleGymFeature(btn){
  btn.classList.toggle('open');
  btn.nextElementSibling.classList.toggle('open');
}
</script>