---
title: 優惠
date: 2026-06-14 15:56:28
top_img: https://onefitnessgym.com/wp-content/uploads/2025/07/1.jpg
---

<style>
/* 封裝在獨立類名內，避免污染 Hexo 全域樣式 */
.gym-promotions {
  font-family: "Noto Sans TC", sans-serif;
  line-height: 1.6;
  max-width: 800px;
  margin: 40px auto;
  padding: 0 15px;
}
.gym-promotions .promo-container {
  background-color: rgba(255, 255, 255, 0.06);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 40px;
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
}
/* 讓主題在淺色/深色模式下都有完美的文字對比 */
[data-theme="light"] .gym-promotions .promo-container {
  background-color: rgba(255, 255, 255, 0.85);
  border: 1px solid rgba(0, 0, 0, 0.05);
}
.gym-promotions h1 {
  font-size: 28px;
  text-align: center;
  color: #4ecdc4;
  margin: 0 0 30px 0;
  font-weight: 700;
  letter-spacing: 1px;
  border-bottom: none;
}
[data-theme="light"] .gym-promotions h1 {
  color: #005BAC;
}
.gym-promotions h2 {
  font-size: 20px;
  color: var(--text-color, #f0f0f0);
  margin-top: 35px;
  margin-bottom: 18px;
  display: flex;
  align-items: center;
  padding-bottom: 8px;
  border-bottom: 2px solid rgba(255, 255, 255, 0.1);
}
[data-theme="light"] .gym-promotions h2 {
  border-bottom: 2px solid #eaeaea;
  color: #333;
}
.gym-promotions h2::before {
  content: '';
  display: inline-block;
  width: 6px;
  height: 24px;
  background-color: #4ecdc4;
  margin-right: 10px;
  border-radius: 3px;
}
[data-theme="light"] .gym-promotions h2::before {
  background-color: #005BAC;
}
.gym-promotions .offer-card {
  background-color: rgba(255, 255, 255, 0.05);
  padding: 22px;
  margin-bottom: 18px;
  border-radius: 12px;
  border-left: 5px solid #4ecdc4;
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transition: transform 0.2s ease, box-shadow 0.2s ease, background-color 0.2s ease;
}
[data-theme="light"] .gym-promotions .offer-card {
  background-color: #ffffff;
  border-left: 5px solid #007BFF;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}
.gym-promotions .offer-card:hover {
  transform: translateY(-3px);
  background-color: rgba(255, 255, 255, 0.08);
  box-shadow: 0 6px 20px rgba(78, 205, 196, 0.15);
}
[data-theme="light"] .gym-promotions .offer-card:hover {
  background-color: #ffffff;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}
.gym-promotions .offer-title {
  font-size: 18px;
  font-weight: 700;
  color: #fff;
  margin-bottom: 6px;
  display: block;
}
[data-theme="light"] .gym-promotions .offer-title {
  color: #2c3e50;
}
.gym-promotions .price-deal {
  display: block;
  margin-top: 5px;
  color: rgba(255,255,255,0.8);
  font-weight: 500;
  font-size: 16px;
}
[data-theme="light"] .gym-promotions .price-deal {
  color: #444;
}
.gym-promotions .price-highlight {
  background-color: rgba(214, 0, 0, 0.15);
  color: #ff6b6b;
  padding: 2px 8px;
  border-radius: 4px;
  font-weight: 700;
}
[data-theme="light"] .gym-promotions .price-highlight {
  background-color: #fff0f0;
  color: #d60000;
}
.gym-promotions .line-link {
  color: #25d366 !important;
  font-weight: 700;
  text-decoration: underline;
  text-underline-offset: 3px;
  transition: opacity 0.2s ease;
}
[data-theme="light"] .gym-promotions .line-link {
  color: #00b900 !important;
}
.gym-promotions .line-link:hover {
  opacity: 0.8;
}
.gym-promotions .date-box {
  background-color: rgba(78, 205, 196, 0.2);
  border: 1px solid #4ecdc4;
  color: #fff;
  text-align: center;
  padding: 15px;
  border-radius: 8px;
  margin-top: 25px;
  font-weight: 500;
}
[data-theme="light"] .gym-promotions .date-box {
  background-color: #005BAC;
  border: none;
  color: white;
}
.gym-promotions .promo-footer {
  font-size: 14px;
  color: rgba(255, 255, 255, 0.6);
  margin-top: 35px;
  padding-top: 20px;
  border-top: 1px dashed rgba(255, 255, 255, 0.2);
  line-height: 1.8;
}
[data-theme="light"] .gym-promotions .promo-footer {
  color: #666666;
  border-top: 1px dashed #ccc;
}
.gym-promotions .promo-footer ul {
  list-style: none !important;
  padding: 0 !important;
  margin: 0 !important;
}
.gym-promotions .promo-footer li {
  margin-bottom: 8px;
  padding-left: 20px;
  position: relative;
}
.gym-promotions .promo-footer li::before {
  content: '※';
  position: absolute;
  left: 0;
  color: #4ecdc4;
}
[data-theme="light"] .gym-promotions .promo-footer li::before {
  color: #005BAC;
}
@media (max-width: 600px) {
  .gym-promotions .promo-container { padding: 25px 20px; }
  .gym-promotions h1 { font-size: 22px; }
  .gym-promotions h2 { font-size: 18px; }
  .gym-promotions .offer-card { padding: 15px; }
  .gym-promotions .offer-title { font-size: 16px; }
}
</style>

<div class="gym-promotions">
<div class="promo-container">
<h1>社區特約與好鄰居優惠方案</h1>
<h2>🏢 特約社區優惠方案 詳見特約說明</h2>
<div class="offer-card">
<span class="offer-title">自主訓練</span>
<span class="price-deal">➜ 享有 <span class="price-highlight">社區優惠價</span>，具體請參考 <a href="http://lin.ee/HIys0yu" target="_blank" rel="noopener noreferrer" class="line-link">官方LINE</a></span>
</div>
<div class="offer-card">
<span class="offer-title">1對1 私人教練課程</span>
<span class="price-deal">➜ 享有 <span class="price-highlight">特約贈課優惠</span>，具體請參考 <a href="http://lin.ee/HIys0yu" target="_blank" rel="noopener noreferrer" class="line-link">官方LINE</a></span>
</div>
<div class="offer-card">
<span class="offer-title">1對2 私人教練課程</span>
<span class="price-deal">➜ 享有 <span class="price-highlight">特約贈課優惠</span>，具體請參考 <a href="http://lin.ee/HIys0yu" target="_blank" rel="noopener noreferrer" class="line-link">官方LINE</a></span>
</div>
<h2>🏡 好鄰居優惠方案（限鄰近社區）</h2>
<div class="offer-card">
<span class="offer-title">1對1 私人教練課程</span>
<span class="price-deal">➜ 享有 <span class="price-highlight">鄰居專屬折扣</span>，具體請參考 <a href="http://lin.ee/HIys0yu" target="_blank" rel="noopener noreferrer" class="line-link">官方LINE</a></span>
</div>
<div class="offer-card">
<span class="offer-title">1對2 私人教練課程</span>
<span class="price-deal">➜ 享有 <span class="price-highlight">鄰居專屬折扣</span>，具體請參考 <a href="http://lin.ee/HIys0yu" target="_blank" rel="noopener noreferrer" class="line-link">官方LINE</a></span>
</div>
<h2>📅 特約說明</h2>
<div class="date-box">所有優惠皆適用至 <strong>民國115年12月31日</strong> 止</div>
<div class="promo-footer">
<ul>
<li>特約範圍：遠雄新未來1~3、森木、富宇上城、華悅城、LINE社群:A7大家庭。</li>
<li>請出示社區住戶證明以享社區優惠。</li>
<li>好鄰居方案適用於住家鄰近本館者，請來電或私訊 <a href="http://lin.ee/HIys0yu" target="_blank" rel="noopener noreferrer" class="line-link">官方LINE</a>確認。</li>
<li>優惠方案不得與其他折扣或活動併用。</li>
<li>本公司保留優惠最終解釋權。</li>
</ul>
</div>
</div>
</div>