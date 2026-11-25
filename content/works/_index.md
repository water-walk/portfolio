---
layout: "single"
title: "作品一覧"
hidemeta: true
---

<style>
/* 全体の幅を80%に統一 */
.post-content {
  width: 80% !important;
  max-width: 2000px !important;
  margin: 0 auto !important;
  box-sizing: border-box;
}

/* 横3列のカードグリッドレイアウト */
.works-grid-3col {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 40px 30px;
  margin-top: 40px;
}

@media (max-width: 768px) {
  .works-grid-3col {
    grid-template-columns: 1fr;
  }
}

/* カードのデザイン（ホーム画面や詳細ページと完全統一） */
.work-grid-card {
  text-decoration: none !important;
  border-bottom: none !important;
  color: inherit;
  display: flex;
  flex-direction: column;
  transition: transform 0.2s ease, opacity 0.2s ease;
  background: transparent !important;
  border: none !important;
  box-shadow: none !important;
  padding: 0 !important;
  align-items: flex-start !important;
}

.work-grid-card:hover {
  transform: translateY(-4px);
  opacity: 0.85;
}

.work-grid-img-wrapper {
  width: 100% !important;
  aspect-ratio: 16/10 !important;
  background: transparent !important;
  margin-bottom: 8px !important;
  border-radius: 6px !important;
  overflow: hidden !important;
  box-shadow: 0 4px 12px rgba(0,0,0,0.06) !important;
}

.work-grid-img-wrapper img {
  width: 100% !important;
  height: 100% !important;
  object-fit: cover !important;
  display: block !important;
  margin: 0 !important;
}

/* 作品タイトルの調整（途切れないように折り返しを設定） */
.work-grid-title {
  font-size: 0.95rem !important;
  font-weight: bold !important;
  margin: 0 !important;
  color: #222 !important;
  text-decoration: none !important;
  border-bottom: none !important;
  white-space: normal !important;
  overflow: visible !important;
  text-overflow: clip !important;
  line-height: 1.4 !important;
}
</style>

<!-- 横3列の作品カード一覧 -->
<div class="works-grid-3col">

  <!-- 作品 1 -->
  <a href="./work01/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work01.jpg" alt="Echoes">
    </div>
    <h3 class="work-grid-title">Echoes</h3>
  </a>

  <!-- 作品 2 -->
  <a href="./work02/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work02.jpg" alt="Cam to Turn">
    </div>
    <h3 class="work-grid-title">Cam to Turn</h3>
  </a>

  <!-- 作品 3 -->
  <a href="./work03/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work03.jpg" alt="りびんぐすくえあ">
    </div>
    <h3 class="work-grid-title">りびんぐすくえあ</h3>
  </a>

  <!-- 作品 4 -->
  <a href="./work04/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work04.jpg" alt="TWing mission : ざっくりロケット開発大作戦！">
    </div>
    <h3 class="work-grid-title">TWing mission : ざっくりロケット開発大作戦！</h3>
  </a>

  <!-- 作品 5 -->
  <a href="./work05/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work05.jpg" alt="ろばっとぱぼっく">
    </div>
    <h3 class="work-grid-title">ろばっとぱぼっく</h3>
  </a>

</div>