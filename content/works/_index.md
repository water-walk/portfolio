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
}

.work-grid-card:hover {
  transform: translateY(-4px);
  opacity: 0.85;
}

.work-grid-img-wrapper {
  width: 100%;
  aspect-ratio: 16/10;
  background: transparent !important;
  margin-bottom: 8px;
  border-radius: 6px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.06);
}

/* 作品タイトルの調整（小さく上品なキャプションサイズ） */
.work-grid-title {
  font-size: 0.75rem !important;
  font-weight: 500 !important;
  margin: 4px 0 0 0 !important;
  color: #333 !important;
  text-decoration: none !important;
  border-bottom: none !important;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
</style>

<!-- 横3列の作品カード一覧 -->
<div class="works-grid-3col">

  <!-- 作品 1 -->
  <a href="./work01/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work01.jpg" alt="Echoes" style="width: 100%; height: 100%; object-fit: cover; display: block;">
    </div>
    <h3 class="work-grid-title">Echoes</h3>
  </a>

  <!-- 作品 2 -->
  <a href="./work02/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work02.jpg" alt="Cam to Turn" style="width: 100%; height: 100%; object-fit: cover; display: block;">
    </div>
    <h3 class="work-grid-title">Cam to Turn</h3>
  </a>

  <!-- 作品 3 -->
  <a href="./work03/" class="work-grid-card">
    <div class="work-grid-img-wrapper">
      <img src="../work03.jpg" alt="りびんぐすくえあ" style="width: 100%; height: 100%; object-fit: cover; display: block;">
    </div>
    <h3 class="work-grid-title">りびんぐすくえあ</h3>
  </a>

</div>