---
layout: "single"
---

<style>
  body {
    margin: 0 !important;
    padding: 0 !important;
  }
  .container {
    max-width: 100% !important;
    padding: 0 !important;
    margin: 0 !important;
  }

  .main {
    margin-top: 0 !important;
    padding-top: 0 !important;
    max-width: 100% !important;
  }
  
  .post-header, .post-content, .post-meta {
    margin: 0 !important;
    padding: 0 !important;
  }

  header.header {
    position: absolute !important;
    top: 0 !important;
    left: 0 !important;
    width: 100% !important;
    background: rgba(255, 255, 255, 0.4) !important; 
    backdrop-filter: blur(12px) !important; 
    -webkit-backdrop-filter: blur(12px) !important;
    z-index: 999 !important; 
    border: none !important;
    padding: 0 20px !important; 
  }
  header.header nav.nav {
    min-height: 48px !important;
    height: 48px !important;
    display: flex !important;
    align-items: center !important;
    justify-content: space-between !important;
  }
  .logo a {
    line-height: 48px !important;
    margin: 0 !important;
    padding: 0 !important;
  }
  ul#menu {
    align-items: center !important;
    margin: 0 !important;
  }
  ul#menu li a {
    padding: 6px 12px !important;
  }

  .menu a, .logo a {
    color: #111 !important;
    font-weight: 500 !important;
  }

  .section-title-container {
    position: relative;
    margin-bottom: 40px;
    height: 90px;
  }

  .bg-en-title {
    position: absolute;
    top: 0;
    left: 0;
    font-size: 4.5rem;
    font-weight: 800;
    color: rgba(173, 216, 230, 0.45);
    line-height: 1;
    letter-spacing: 4px;
    user-select: none;
  }

  .fg-ja-title {
    position: absolute;
    bottom: 5px;
    left: 10px;
    font-size: 1.6rem;
    font-weight: 700;
    color: #111;
    line-height: 1;
    z-index: 2;
  }

  .work-scroll-container {
    display: flex;
    overflow-x: auto;
    white-space: nowrap;
    gap: 24px;
    padding: 10px 0 30px 0;
    scrollbar-width: thin;
    scrollbar-color: #ccc transparent;
    -webkit-overflow-scrolling: touch;
  }
  .work-scroll-container::-webkit-scrollbar {
    height: 6px;
  }
  .work-scroll-container::-webkit-scrollbar-track {
    background: transparent;
  }
  .work-scroll-container::-webkit-scrollbar-thumb {
    background-color: #ddd;
    border-radius: 10px;
  }
  .work-card {
    flex: 0 0 280px;
    border: 1px solid #eee;
    padding: 18px;
    border-radius: 8px;
    background: #fff;
    box-shadow: 0 4px 12px rgba(0,0,0,0.03);
    transition: transform 0.3s ease;
  }
  .work-card:hover {
    transform: translateY(-4px);
  }
  .work-thumbnail {
    aspect-ratio: 4/3;
    background: #f0f0f0;
    margin-bottom: 12px;
    border-radius: 4px;
  }
  .work-title {
    font-size: 1.1rem;
    font-weight: 600;
    margin: 0 0 6px 0;
    color: #111;
  }
  .work-desc {
    font-size: 0.85rem;
    color: #666;
    margin: 0;
    white-space: normal;
  }
</style>

<!-- メインビジュアル -->
<div style='width: 100%; margin: 0; padding: 0; overflow: hidden; position: relative; z-index: 1;'>
  <img src='./Nattsu.jpg' alt='Nattsu' style='width: 100%; height: auto; display: block; max-height: 85vh; object-fit: cover;'>
</div>

<!-- コンテナ -->
<div style='max-width: 900px; margin: 80px auto 0; padding: 0 20px; font-family: "Helvetica Neue", Arial, sans-serif;'>

<!-- WORK (制作実績) -->
<style>
/* 無限スクロールの枠組み */
.marquee-container {
  overflow: hidden;
  width: 100%;
  margin-bottom: 120px;
  text-align: left;
}

/* 横並びにして動かすトラック */
.marquee-track {
  display: flex;
  gap: 20px;
  width: max-content;
  animation: marquee-scroll 25s linear infinite;
}

/* マウスホバーで一時停止 */
.marquee-container:hover .marquee-track {
  animation-play-state: paused;
}

/* 流れるアニメーション */
@keyframes marquee-scroll {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

/* コンパクトな作品カード */
.work-simple-card {
  width: 220px;
  text-decoration: none;
  color: inherit;
  display: flex;
  flex-direction: column;
  transition: transform 0.2s ease, opacity 0.2s ease;
}

.work-simple-card:hover {
  transform: translateY(-4px);
  opacity: 0.85;
}

.work-img-wrapper {
  width: 100%;
  aspect-ratio: 4/3;
  background: #eee;
  margin-bottom: 8px;
  border-radius: 6px;
  overflow: hidden;
}

.work-simple-title {
  font-size: 0.95rem;
  font-weight: bold;
  margin: 0;
  color: #222;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
</style>

<div id='work' class='marquee-container'>
<div class='section-title-container'>
<div class='bg-en-title'>WORK</div>
<div class='fg-ja-title'>制作実績</div>
</div>

<div class='marquee-track'>

<!-- ===== 1セット目 ===== -->
<a href='./works/work01/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work01.jpg' alt='作品1' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
<h3 class='work-simple-title'>もわもわ</h3>
</a>

<a href='./works/work02/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work02.jpg' alt='作品2' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
<h3 class='work-simple-title'>感情共有デバイス</h3>
</a>

<a href='./works/work03/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work03.jpg' alt='作品3' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
<h3 class='work-simple-title'>奇跡の軌跡</h3>
</a>

<a href='./works/work04/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work04.jpg' alt='作品4' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
<h3 class='work-simple-title'>視覚的モールス信号</h3>
</a>

<a href='./works/work05/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work05.jpg' alt='作品5' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
</a>


<a href='./works/work06/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work06.jpg' alt='作品6' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
<h3 class='work-simple-title'>りびんぐすくえあ</h3>
</a>



<!-- ===== 2セット目（ループ用複製） ===== -->

</div>
</div>

<!-- PROFILE -->
<div id='profile' style='margin-bottom: 120px; text-align: left;'>
<div class='section-title-container'>
<div class='bg-en-title'>PROFILE</div>
<div class='fg-ja-title'>自己紹介</div>
</div>

<div style='display: flex; flex-wrap: wrap; gap: 40px; align-items: flex-start;'>
<img src='./profile.jpg' alt='蓮田 瑞歩' style='width: 150px; height: 150px; object-fit: cover; border-radius: 50%; flex-shrink: 0;'>

<div style='flex: 1; min-width: 280px;'>
<p style='font-size: 1.2rem; font-weight: bold; margin-bottom: 20px; color: #111;'>蓮田 瑞歩 / Mizuho Hasuda</p>

<!-- テーブル形式のリスト（横書きで綺麗に整列） -->
<dl style='display: grid; grid-template-columns: 120px 1fr; gap: 16px 20px; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0;'>
  
  <dt style='font-weight: bold; color: #111; white-space: nowrap;'>所属</dt>
  <dd style='margin: 0;'>明星大学 情報学部 情報学科 4年生</dd>

  <dt style='font-weight: bold; color: #111; white-space: nowrap;'>研究室</dt>
  <dd style='margin: 0;'>インタラクティブメディア 研究室</dd>

  <dt style='font-weight: bold; color: #111; white-space: nowrap;'>連絡先</dt>
  <dd style='margin: 0;'><a href='mailto:mizuho.nattsu.0809@gmail.com' style='color: #333; text-decoration: underline;'>mizuho.nattsu.0809@gmail.com</a></dd>

  <dt style='font-weight: bold; color: #111; white-space: nowrap;'>趣味</dt>
  <dd style='margin: 0;'>カメラ、馬、車</dd>

</dl>
</div>
</div>
</div>

  <!-- ACHIEVEMENTS -->
  <div id='achievements' style='margin-bottom: 120px; text-align: left;'>
    <div class='section-title-container'>
      <div class='bg-en-title'>ACHIEVEMENTS</div>
      <div class='fg-ja-title'>活動・実績</div>
    </div>
    
    <p style='font-size: 0.95rem; color: #444; line-height: 1.8;'>
      ここに受賞歴や資格、その他実績などを記載します。
    </p>
  </div>

  <!-- CONTACT -->
  <div id='contact' style='margin-bottom: 100px; text-align: left;'>
    <div class='section-title-container'>
      <div class='bg-en-title'>CONTACT</div>
      <div class='fg-ja-title'>お問い合わせ</div>
    </div>
    
    <p style='font-size: 0.95rem; color: #444;'>
      Email: <a style='color: #000; text-decoration: underline;' href='mailto:mizuho.nattsu.0809@gmail.com'>mizuho.nattsu.0809@gmail.com</a>
    </p>
  </div>
</div>