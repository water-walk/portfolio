---
title: "TWing mission : ざっくりロケット開発大作戦！"
date: 2026-06-07
period: "2026年6月"
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
  aspect-ratio: 16/10;
  background: #fff;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: none;
  border: none;
  margin-bottom: 12px;
}
.work-main-img-box img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  display: block;
  transition: opacity 0.2s ease;
}

/* 下部のサムネイル横スクロール */
.work-thumb-scroll {
  display: flex;
  gap: 12px;
  overflow-x: auto;
  overflow-y: visible !important; 
  padding: 10px 4px 8px 4px !important; 
  scrollbar-width: thin;
}

/* サムネイルの丸型設定 */
.work-thumb-item {
  width: 60px !important;
  height: 60px !important;
  border-radius: 50% !important;
  flex-shrink: 0;
  overflow: hidden !important;
  cursor: pointer;
  border: 2px solid transparent;
  opacity: 0.6;
  transition: all 0.2s ease;
  background: transparent !important;
  box-sizing: border-box;
  padding: 0 !important;
}

.work-thumb-item.active, .work-thumb-item:hover {
  opacity: 1;
  border-color: #0066cc;
  transform: scale(1.05);
}

.work-thumb-item img {
  width: 100% !important;
  height: 100% !important;
  max-width: 100% !important;
  max-height: 100% !important;
  object-fit: cover !important;
  border-radius: 0 !important; 
  margin: 0 !important; 
  padding: 0 !important;
  display: block !important;
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
<div class='work-period-badge'>制作時期：2026年6月</div>
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
<div class='work-thumb-item' onclick='switchWorkImg(this, "/portfolio/work04_02.jpg")'>
<img src='/portfolio/work04_02.jpg' alt='サムネイル2'>
</div>
<div class='work-thumb-item' onclick='switchWorkImg(this, "/portfolio/work04_03.jpg")'>
<img src='/portfolio/work04_03.jpg' alt='サムネイル3'>
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
<span class='tech-tag'>Processing</span>
<span class='tech-tag'>Arduino</span>
</div>
</div>



<!-- 3. 説明文章 -->
<div class='work-info-block'>
<div class='work-info-label'>CONCEPT & DESCRIPTION</div>
<div class='work-info-text'>
<p style='margin: 0 0 16px 0;'>「エンジニアがブラックサンダーを食べたくなるアイデア」をテーマとしたハッカソン「ブラッカソン」にて、チームで制作したインタラクティブ作品です。共同開発におけるコミュニケーションに着目し、開発そのものをエンターテインメントとして楽しむことで、参加者同士の距離を縮めることを目指しました。</p>

<p style='margin: 0 0 16px 0;'>本作品では、「二人羽織」と「共同開発」を組み合わせ、2人1組でマニュアルを読みながらロケットを組み立てます。組み立てたパーツは画面上にリアルタイムで反映され、パーツの組み合わせによってロケットの性能が変化します。また、開発中にブラックサンダーを相手に食べさせることで、制限時間の延長や燃料の補充ができます。ロケットの組み立てが完了した後は、配線した発射ボタンを使ってロケットを発射します。</p>

<p style='margin: 0 0 16px 0;'>ロケットの開発とブラックサンダーを食べる行為を一つのゲーム体験に取り入れることで、楽しみながら自然にコミュニケーションが生まれる仕組みを考えました。</p>
</div>
</div>



<!-- 関連リンク（RELATED LINKS）セクション -->
<div class='work-info-block' style='margin-top: 50px; padding-top: 30px; border-top: 1px solid #eaeaea;'>
<div class='work-info-label'>RELATED LINKS</div>
<div class='related-links-container'>

<!-- リンク 1（必要に応じて増やしたり減らしたりできます） -->
<a href='https://www.yurakuseika.co.jp/blackathon/?bt=%E3%82%B6%E3%82%AF%E3%82%B6%E3%82%AF%E3%82%B6%E3%82%AF%E2%9A%A1%F0%9F%8D%AB' target='_blank' class='related-link-card'>
<div class='related-link-info'>
<div class='related-link-title'>ブラッカソン　ブラックサンダーが開催するエンジニア向けハッカソン</div>
<div class='related-link-url'>https://www.yurakuseika.co.jp/blackathon/?bt=%E3%82%B6%E3%82%AF%E3%82%B6%E3%82%AF%E3%82%B6%E3%82%AF%E2%9A%A1%F0%9F%8D%AB</div>
</div>
<div class='related-link-icon'>→</div>
</a>

<a href='https://prtimes.jp/main/html/rd/p/000000317.000064626.html' target='_blank' class='related-link-card'>
<div class='related-link-info'>
<div class='related-link-title'>開催レポート】 AI審査員賞を含む各賞を発表！ブラックサンダー初主催のハッカソン「ブラッカソン」！エンジニアがブラックサンダーを食べたくなる遊び心あふれる発明が集結！</div>
<div class='related-link-url'>https://prtimes.jp/main/html/rd/p/000000317.000064626.html</div>
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