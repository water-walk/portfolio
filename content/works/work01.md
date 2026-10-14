---
title: "5秒間の軌跡"
date: 2025-07-01
period: "2025年度前期"
hidemeta: true
---

<style>
/* PaperModのメインコンテナ幅を広げてゆとりを持たせる */
.main {
  max-width: 1100px !important;
}
.post-content {
  max-width: 100% !important;
}

/* 個別作品ページのレイアウト */
.work-detail-container {
  width: 100%;
  margin-top: 10px;
  font-family: "Helvetica Neue", Arial, sans-serif;
  color: #222;
}

/* 上部時期バッジ等の下線エリア */
.work-header {
  border-bottom: 2px solid #111;
  padding-bottom: 12px;
  margin-bottom: 30px;
  width: 100%;
}
.work-period-badge {
  font-size: 1rem;
  color: #555;
  font-weight: 600;
}

/* 左右2カラム構造（幅を広く確保） */
.work-content-grid {
  display: grid;
  grid-template-columns: 1fr 1.1fr;
  gap: 50px;
  align-items: start;
}

@media (max-width: 768px) {
  .work-content-grid {
    grid-template-columns: 1fr;
    gap: 24px;
  }
}

/* 左側：ギャラリービューア */
.work-gallery-wrapper {
  width: 100%;
  position: sticky;
  top: 80px;
}

.work-main-img-box {
  width: 100%;
  aspect-ratio: 4/3;
  background: #f4f4f4;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  margin-bottom: 12px;
}
.work-main-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
  transition: opacity 0.2s ease;
}

/* 下部のサムネイル横スクロール */
.work-thumb-scroll {
  display: flex;
  gap: 10px;
  overflow-x: auto;
  padding-bottom: 8px;
  scrollbar-width: thin;
}
.work-thumb-item {
  width: 80px;
  height: 60px;
  flex-shrink: 0;
  border-radius: 4px;
  overflow: hidden;
  cursor: pointer;
  border: 2px solid transparent;
  opacity: 0.6;
  transition: all 0.2s ease;
  background: #eee;
}
.work-thumb-item.active, .work-thumb-item:hover {
  opacity: 1;
  border-color: #0066cc;
}
.work-thumb-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* 右側：情報テキスト群 */
.work-info-section {
  display: flex;
  flex-direction: column;
  gap: 28px;
}

.work-info-block {
  display: flex;
  flex-direction: column;
  gap: 8px;
}
.work-info-label {
  font-size: 0.85rem;
  font-weight: bold;
  color: #0066cc;
  text-transform: uppercase;
  letter-spacing: 1px;
}
.work-info-text {
  font-size: 1rem;
  line-height: 1.9;
  color: #333;
  margin: 0;
  white-space: pre-wrap;
}

/* 技術タグ */
.tech-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 4px;
}
.tech-tag {
  background: #f0f4f8;
  color: #334155;
  padding: 6px 14px;
  border-radius: 4px;
  font-size: 0.9rem;
  font-weight: 600;
}
</style>

<div class='work-detail-container'>

<!-- 制作時期のみ（タイトルはHugo標準に任せて二重化を防止） -->
<div class='work-header'>
<div class='work-period-badge'>制作時期：2025年度前期</div>
</div>

<!-- コンテンツエリア（左：画像 / 右：詳細説明） -->
<div class='work-content-grid'>

<!-- 左カラム：画像ギャラリー -->
<div class='work-gallery-wrapper'>
<div class='work-main-img-box'>
<img id='mainDisplayImg' src='/portfolio/work01.jpg' alt='メイン画像'>
</div>

<div class='work-thumb-scroll'>
<div class='work-thumb-item active' onclick='switchWorkImg(this, "../images/work01.jpg")'>
<img src='/portfolio/work01.jpg' alt='サムネイル1'>
</div>
</div>
</div>

<!-- 右カラム：説明コンテンツ -->
<div class='work-info-section'>

<!-- 1. 制作時期・区分 -->
<div class='work-info-block'>
<div class='work-info-label'>PERIOD</div>
<div class='work-info-text'>2025年度前期（明星大学 インタラクティブシステム 授業課題）</div>
</div>

<!-- 2. 使用機材・技術 -->
<div class='work-info-block'>
<div class='work-info-label'>TECHNOLOGY / HARDWARE</div>
<div class='tech-tags'>
<span class='tech-tag'>Webカメラ</span>
<span class='tech-tag'>p5.js</span>
<span class='tech-tag'>JavaScript</span>
<span class='tech-tag'>HTML/CSS</span>
</div>
</div>

<!-- 3. 説明文章 -->
<div class='work-info-block'>
<div class='work-info-label'>CONCEPT & DESCRIPTION</div>
<div class='work-info-text'>
「インタラクティブシステム」の授業課題として、チームで制作したインタラクティブ作品です。
<a href='https://www.tokyonode.jp/sp/exhibition-ah-neo/' target='_blank' style='color: #0066cc; text-decoration: underline;'>デザインあ展neo</a>の《あるきかたログ》から着想を得て、一人ひとりの動きが重なり、一つの流れになるという表現をもとに、人がその場にいた痕跡を可視化する作品を考えました。

「自分自身は見えないけれど、確かに存在する」をコンセプトに、カメラに映った人物の姿が数秒後に「影」として画面上に現れます。影は時間とともに徐々に濃くなり、その後ゆっくりと消えていきます。また、周囲の音の大きさに応じて影の輪郭が揺らぎ、目には見えない存在の痕跡や曖昧さを表現しています。

p5.jsを使用して映像の描画とインタラクションを制御しています。Webカメラで取得した映像からml5.js（BodyPix）を用いて人物の輪郭を抽出し、時間差で影として表示しています。
また、マイクから取得した周囲の音をFFTで解析し、音の大きさに応じて影の輪郭が揺らぐ仕組みを実装しました。
</div>
</div>

<!-- 4. 動作動画 -->
<p style="margin-top: 20px;">
<a href="https://youtu.be/OPBoLv4kO8c" target="_blank" style="display: inline-block; padding: 10px 20px; background-color: #FF0000; color: #ffffff; text-decoration: none; border-radius: 6px; font-weight: bold; font-size: 0.95rem;">
▶ YouTubeで見る
</a>
</p>

<!-- 関連リンク（RELATED LINKS）セクション -->
<div class='work-info-block' style='margin-top: 50px; padding-top: 30px; border-top: 1px solid #eaeaea;'>
<div class='work-info-label'>RELATED LINKS</div>
<div class='related-links-container'>

<!-- リンク 1（必要に応じて増やしたり減らしたりできます） -->
<a href='https://openlab.is.meisei-u.ac.jp/2025/08/02/1050/' target='_blank' class='related-link-card'>
<div class='related-link-info'>
<div class='related-link-title'>Open Lab公式サイト 授業紹介企画第4弾「インタラクティブシステム」</div>
<div class='related-link-url'>https://openlab.is.meisei-u.ac.jp/2025/08/02/1050/</div>
</div>
<div class='related-link-icon'>→</div>
</a>

</div>
</div>

<style>
/* 関連リンクのカードデザイン */
.related-links-container {
display: flex;
flex-direction: column;
gap: 12px;
margin-top: 10px;
}
.related-link-card {
display: flex;
align-items: center;
justify-content: space-between;
padding: 16px 20px;
background: #f8fafc;
border: 1px solid #e2e8f0;
border-radius: 8px;
text-decoration: none;
color: inherit;
transition: all 0.2s ease;
}
.related-link-card:hover {
background: #f1f5f9;
border-color: #cbd5e1;
transform: translateY(-2px);
box-shadow: 0 4px 12px rgba(0,0,0,0.03);
}
.related-link-info {
display: flex;
flex-direction: column;
gap: 4px;
}
.related-link-title {
font-size: 0.95rem;
font-weight: bold;
color: #1e293b;
}
.related-link-url {
font-size: 0.8rem;
color: #64748b;
word-break: break-all;
}
.related-link-icon {
font-size: 1.1rem;
font-weight: bold;
color: #0066cc;
padding-left: 12px;
}
</style>

</div>
</div>

<script>
function switchWorkImg(element, newSrc) {
  var mainImg = document.getElementById('mainDisplayImg');
  if (mainImg) {
    mainImg.style.opacity = '0.3';
    setTimeout(function() {
      mainImg.src = newSrc;
      mainImg.style.opacity = '1';
    }, 150);
  }
  var thumbs = document.querySelectorAll('.work-thumb-item');
  thumbs.forEach(function(thumb) {
    thumb.classList.remove('active');
  });
  element.classList.add('active');
}
</script>