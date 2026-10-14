---
title: "りびんぐすくえあ RibinguSukuea"
date: 2026-02-14
period: "2025年度後期"
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
<div class='work-period-badge'>制作時期：2025年度後期</div>
</div>

<!-- コンテンツエリア（左：画像 / 右：詳細説明） -->
<div class='work-content-grid'>

<!-- 左カラム：画像ギャラリー（クリック切替機能付き） -->
<div class='work-gallery-wrapper'>
<div class='work-main-img-box'>
<img id='mainDisplayImg' src='/portfolio/work04.jpg' alt='メイン画像'>
</div>

<!-- 下部のサムネイル一覧 -->
<div class='work-thumb-scroll'>
<div class='work-thumb-item active' onclick='switchWorkImg(this, "/portfolio/work04.jpg")'>
<img src='/portfolio/work04.jpg' alt='サムネイル1'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "/portfolio/work04_2.jpg")'>
<img src='/portfolio/work04_2.jpg' alt='サムネイル2'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "/portfolio/work04_3.jpg")'>
<img src='/portfolio/work04_3.jpg' alt='サムネイル3'>
</div>
</div>
</div>

<!-- 右カラム：説明コンテンツ -->
<div class='work-info-section'>

<!-- 1. 制作時期・区分 -->
<div class='work-info-block'>
<div class='work-info-label'>PERIOD</div>
<div class='work-info-text'>2025年度後期</div>
</div>

<!-- 2. 使用機材・技術 -->


<div class='work-info-block'>
<div class='work-info-label'>TECHNOLOGY / HARDWARE</div>
<div class='tech-tags'>
<span class='tech-tag'>toio</span>
<span class='tech-tag'>Python</span>
<span class='tech-tag'>YOLO</span>
<span class='tech-tag'>Webカメラ</span>
<span class='tech-tag'>ATOM Mate for toio</span>
<span class='tech-tag'>RFID</span>
</div>
</div>



<!-- 3. 説明文章 -->
<div class='work-info-block'>
<div class='work-info-label'>CONCEPT & DESCRIPTION</div>
<div class='work-info-text'>
<p style='margin: 0 0 16px 0;'>「チームアクティビティ2」という授業にて制作した、ロボットの動きを通じて「いきものらしさ」を表現するインタラクティブ作品です。</p>

<p style='margin: 0 0 16px 0;'>人は、思い通りに動かないものや、関わり方によって反応が変化するものに対して、意志や感情があるように感じることがあります。本作品では、外見的な特徴をできるだけ抑えた立方体のロボットを用い、動きや反応の違いから、単なる道具が一つの生き物のように感じられる体験を目指しました。作品では、「認識の不一致」と「相互作用の履歴」という2つの方法から、ロボットの主体性や愛着が生まれる過程を表現しています。2026年2月14・15日にパルテノン多摩で行われた「MEISEI STEAM FESTIVAL 2026」にて展示しました。</p>

<p style='margin: 0 0 16px 0;'>Sonyのtoio コアキューブを使用し、3Dプリンタで制作した黒い立方体のカバーを取り付けました。見た目の情報を減らすことで、ロボットの動きそのものに注目できるようにしています。</p>

<p style='margin: 0 0 16px 0;'>
<strong>①認識の不一致による主体性の提示</strong><br>
カメラ映像からYOLOを用いて体験者の位置を検出し、Pythonでロボットの動きを制御しています。ロボットは基本的に体験者の動きを模倣しますが、マット上に設定された仮想的な障害物に遭遇すると、独自の反応を示します。「壁」では停止し、「トンネル」ではゆっくり移動し、「おばけ」では驚いたような動きをします。体験者には見えない障害物に反応することで、ロボットが自分とは異なる世界を認識しているように感じられる仕組みです。
</p>

<p style='margin: 0 0 0 0;'>
<strong>②相互作用の履歴による愛着の形成</strong><br>
toioに距離センサーを搭載し、人との距離や関わりに応じてロボットの行動が変化するようにしました。最初は人の手が近づくと逃げるように動きますが、繰り返し関わることで徐々に反応が変わり、手にすり寄るような動きを見せます。また、RFIDカードをかざすことで、喜ぶように揺れたり、音を鳴らしながら回転したりするなど、異なる反応を引き出せるようにしました。
</p>
</div></div>

<!-- 4. 動作動画 -->
<p style="margin-top: 20px;">
<a href="https://youtu.be/67kqYj41PUo" target="_blank" style="display: inline-block; padding: 10px 20px; background-color: #FF0000; color: #ffffff; text-decoration: none; border-radius: 6px; font-weight: bold; font-size: 0.95rem;">
▶ YouTubeで見る
</a>
</p>

<!-- 関連リンク（RELATED LINKS）セクション -->
<div class='work-info-block' style='margin-top: 50px; padding-top: 30px; border-top: 1px solid #eaeaea;'>
<div class='work-info-label'>RELATED LINKS</div>
<div class='related-links-container'>

<!-- リンク 1（必要に応じて増やしたり減らしたりできます） -->
<a href='https://www.is.meisei-u.ac.jp/news/2600/' target='_blank' class='related-link-card'>
<div class='related-link-info'>
<div class='related-link-title'>明星大学 情報学部情報学科 MEISEI STEAM FESTIVAL 2026 情報学科×国際コミュニケーション学科 合同展示開催！！
</div>
<div class='related-link-url'>https://www.is.meisei-u.ac.jp/news/2600/</div>
</div>
<div class='related-link-icon'>→</div>
</a>

<a href='https://www.is.meisei-u.ac.jp/news/2642/' target='_blank' class='related-link-card'>
<div class='related-link-info'>
<div class='related-link-title'>明星大学 情報学部情報学科 MEISEI STEAM FESTIVAL 2026 情報学科×国際コミュニケーション学科 合同展示を開催しました！！
</div>
<div class='related-link-url'>https://www.is.meisei-u.ac.jp/news/2642/</div>
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