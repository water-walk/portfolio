---
title: "Echoes"
date: 2025-11-20
period: "2025.11"
hidemeta: true
---

<style>
.main {
max-width: 1100px !important;
}
.post-content {
max-width: 100% !important;
}
.work-detail-container {
width: 100%;
margin-top: 10px;
font-family: "Helvetica Neue", Arial, sans-serif;
color: #222;
}
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

<!-- 1. 全幅タイトル ＋ 制作時期 -->
<div class='work-header'>
<div class='work-period-badge'>制作時期：2025年11月</div>
</div>

<!-- 2. コンテンツエリア（左：画像ビューア / 右：詳細説明） -->
<div class='work-content-grid'>

<!-- 左カラム：画像ギャラリー（クリック切替機能付き） -->
<div class='work-gallery-wrapper'>
<div class='work-main-img-box'>
<img id='mainDisplayImg' src='/portfolio/work02.jpg' alt='メイン画像'>
</div>

<!-- 下部のサムネイル一覧 -->
<div class='work-thumb-scroll'>
<div class='work-thumb-item active' onclick='switchWorkImg(this, "/portfolio/work02.jpg")'>
<img src='/portfolio/work02.jpg' alt='サムネイル1'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "/portfolio/work02_2.jpg")'>
<img src='/portfolio/work02_2.jpg' alt='サムネイル2'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "/portfolio/work02_3.jpg")'>
<img src='/portfolio/work02_3.jpg' alt='サムネイル3'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "/portfolio/work02_4.jpg")'>
<img src='/portfolio/work02_4.jpg' alt='サムネイル4'>
</div>
</div>
</div>

<!-- 右カラム：説明コンテンツ -->
<div class='work-info-section'>

<!-- 1. 制作時期 / 区分 -->
<div class='work-info-block'>
<div class='work-info-label'>PERIOD</div>
<div class='work-info-text'>2025年11月</div>
</div>

<!-- 2. 使用機材・技術 -->
<div class='work-info-block'>
<div class='work-info-label'>TECHNOLOGY / HARDWARE</div>
<div class='tech-tags'>
<span class='tech-tag'>Arduino</span>
<span class='tech-tag'>Processing</span>
<span class='tech-tag'>超音波距離センサー</span>
<span class='tech-tag'>サーボモーター</span>
</div>
</div>

<!-- 3. 説明文章 -->
<div class='work-info-block'>
<div class='work-info-label'>CONCEPT & DESCRIPTION</div>
<div class='work-info-text'>
グローバル・プロジェクト「MUROS week」にて、ドイツ・デュッセルドルフ応用科学大学の学生を含めた4人のチームで共同制作したインタラクティブ・インスタレーション作品です。
Human Data Interactionを基盤とした「専門家でない人が気候変動データを感覚的に理解する」という課題に対し、気候変動が日本の桜に与える影響をテーマに制作しました。
桜は日本の四季や春の訪れ、再生と希望を象徴する存在です。しかし、地球温暖化による気温の変化は、桜の開花や季節のリズムに影響を与えています。
本作品では、気象データを桜の配置によって立体的に可視化するとともに、人の接近に反応して開閉する桜を制作しました。自然が持つ調和やリズムの変化を感覚的に伝え、自然との関わり方を考えるきっかけとなることを目指しました。
作品名の「Echoes（響き）」には、弱まりながらも響き続ける自然の声に再び耳を傾け、自然の回復への希望を感じてほしいという思いを込めています。

日本の47都道府県の気温・日照時間・降水量のデータを使用し、ProcessingでそれぞれをX軸・Y軸・Z軸に割り当てて3次元座標に変換しました。その座標をもとに47個の桜を天井から吊るし、数値データを立体的な空間表現へと変換しました。
中央に配置した大きな桜は、Arduinoと超音波センサー、サーボモーターを使用して開閉を制御しています。人が近づくと花びらが閉じ、一定の距離まで離れるとゆっくりと開く仕組みにすることで、人間の干渉によって自然のリズムが乱される様子を表現しました。
また、和紙を用いた柔らかな光の表現には、自然の繊細さと再生への希望を込めています。
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