---
title: "作品タイトル（例：奇跡の軌跡）"
date: 2025-07-01
period: "2025年度前期"
hidemeta: true
---

<style>
/* 個別作品ページの共通レイアウト */
.work-detail-container {
width: 100%;
margin-top: 20px;
font-family: "Helvetica Neue", Arial, sans-serif;
color: #222;
}

/* 上部タイトルエリア */
.work-header {
border-bottom: 2px solid #111;
padding-bottom: 16px;
margin-bottom: 30px;
width: 100%;
}
.work-title-main {
font-size: 2.2rem;
font-weight: 800;
margin: 0 0 8px 0;
color: #111;
line-height: 1.2;
}
.work-period-badge {
font-size: 0.95rem;
color: #666;
font-weight: 600;
}

/* 左右2カラム構造 */
.work-content-grid {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 40px;
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

/* 下部のサムネイル横スクロール（チラ見せ効果） */
.work-thumb-scroll {
display: flex;
gap: 10px;
overflow-x: auto;
padding-bottom: 8px;
scrollbar-width: thin;
}
.work-thumb-item {
width: 70px;
height: 52px;
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
.work-info-title {
font-size: 1.15rem;
font-weight: bold;
color: #111;
margin: 0;
padding-bottom: 4px;
border-bottom: 1px solid #ddd;
}
.work-info-text {
font-size: 0.95rem;
line-height: 1.8;
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
padding: 4px 12px;
border-radius: 4px;
font-size: 0.85rem;
font-weight: 600;
}
</style>

<div class='work-detail-container'>

<!-- 1. 全幅タイトル ＋ 制作時期 -->
<div class='work-header'>
<h1 class='work-title-main'>奇跡の軌跡</h1>
<div class='work-period-badge'>制作時期：2025年度前期</div>
</div>

<!-- 2. コンテンツエリア（左：画像ビューア / 右：詳細説明） -->
<div class='work-content-grid'>

<!-- 左カラム：画像ギャラリー（クリック切替機能付き） -->
<div class='work-gallery-wrapper'>
<div class='work-main-img-box'>
<img id='mainDisplayImg' src='../images/work01.jpg' alt='メイン画像'>
</div>

<!-- 下部のサムネイル（少し横が見える一覧） -->
<div class='work-thumb-scroll'>
<div class='work-thumb-item active' onclick='switchWorkImg(this, "../images/work01.jpg")'>
<img src='../images/work01.jpg' alt='サムネイル1'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "../images/work02.jpg")'>
<img src='../images/work02.jpg' alt='サムネイル2'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "../images/work03.jpg")'>
<img src='../images/work03.jpg' alt='サムネイル3'>
</div>
</div>
</div>

<!-- 右カラム：説明コンテンツ -->
<div class='work-info-section'>

<!-- 1. 制作時期 / 区分 -->
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
「自分自身は見えないけれど、確かに存在する」をテーマに、可視と不可視による存在感について考えるインタラクティブ体験作品。

カメラ内に人がうつった数秒後に「影」として画面上に表示されます。その時の周囲の環境音や動きによって、その影の輪郭や波紋がインタラクティブに揺らぎます。
</div>
</div>

<!-- 4. 動作動画 (YouTube限定公開等) -->
<div class='work-info-block'>
<div class='work-info-label'>DEMO MOVIE</div>
<div style='margin-top: 6px;'>
{{< youtube 8H81Pnpr-js >}}
</div>
</div>

</div>

</div>
</div>

<!-- 画像切り替え用JavaScript -->
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