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

  /* ★ヘッダーの高さを低く（スリムに）調整しました */
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
  /* ヘッダー内部のナビゲーション（高さを制限して細くします） */
  header.header nav.nav {
    min-height: 48px !important; /* 初期値の60px前後から48pxに縮小 */
    height: 48px !important;
    display: flex !important;
    align-items: center !important;
    justify-content: space-between !important;
  }
  /* ロゴの上下余白を無くして高さを抑える */
  .logo a {
    line-height: 48px !important;
    margin: 0 !important;
    padding: 0 !important;
  }
  /* メニュー全体の高さをヘッダーに合わせる */
  ul#menu {
    align-items: center !important;
    margin: 0 !important;
  }
  ul#menu li a {
    padding: 6px 12px !important; /* メニュー項目の上下の隙間を小さく */
  }

  .menu a, .logo a {
    color: #111 !important;
    font-weight: 500 !important;
  }

  /* 重なりタイトル */
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

  /* --- 横スクロール（流れるWORK）の設定 --- */
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

<!-- コンテナ（シングルクォーテーション固定で全角バグを防止） -->
<div style='max-width: 900px; margin: 80px auto 0; padding: 0 20px; font-family: "Helvetica Neue", Arial, sans-serif;'>
  
  <!-- WORK (制作実績 - 横スクロール版) -->
  <div id='work' style='margin-bottom: 120px; text-align: left;'>
    <div class='section-title-container'>
      <div class='bg-en-title'>WORK</div>
      <div class='fg-ja-title'>制作実績</div>
    </div>
    
    <div class='work-scroll-container'>
      <div class='work-card'>
        <div class='work-thumbnail'></div>
        <h3 class='work-title'>Work 01</h3>
        <p class='work-desc'>作品の説明がここに入ります。</p>
      </div>
      <div class='work-card'>
        <div class='work-thumbnail'></div>
        <h3 class='work-title'>Work 02</h3>
        <p class='work-desc'>作品の説明がここに入ります。</p>
      </div>
      <div class='work-card'>
        <div class='work-thumbnail'></div>
        <h3 class='work-title'>Work 03</h3>
        <p class='work-desc'>作品の説明がここに入ります。</p>
      </div>
      <div class='work-card'>
        <div class='work-thumbnail'></div>
        <h3 class='work-title'>Work 04</h3>
        <p class='work-desc'>作品の説明がここに入ります。</p>
      </div>
    </div>
  </div>

  <!-- PROFILE -->
  <div id='profile' style='margin-bottom: 120px; text-align: left;'>
    <div class='section-title-container'>
      <div class='bg-en-title'>PROFILE</div>
      <div class='fg-ja-title'>自己紹介</div>
    </div>
    
    <div style='display: flex; flex-wrap: wrap; gap: 40px; align-items: flex-start;'>
      <div style='width: 150px; height: 150px; background: #eee; border-radius: 4px; flex-shrink: 0;'></div>
      <div style='flex: 1; min-width: 280px; line-height: 1.8;'>
        <p style='font-size: 1.1rem; font-weight: bold; margin-bottom: 10px; color: #111;'>蓮田 瑞穂 / Mizuho Hasuda</p>
        <p style='color: #444; font-size: 0.95rem;'>ここにプロフィールテキストを入力します。</p>
      </div>
    </div>
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