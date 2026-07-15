---
layout: "single"
---

<style>
  /* サイトの一番上のヘッダーメニュー自体を少し半透明（透過）にして、浮かせます */
  .header {
    background: rgba(255, 255, 255, 0.75) !important;
    backdrop-filter: blur(8px); /* 後ろの画像が少しボケて透けるオシャレエフェクト */
    position: relative;
    z-index: 10;
  }
  /* 余計な境界線を消して、画像と一体化させます */
  .nav {
    background: transparent !important;
  }
</style>

<!-- 1. メインビジュアル（位置を上に引き上げてメニューの下に入り込ませます） -->
<div style="width: 100vw; margin-left: calc(-50vw + 50%); margin-top: -120px; margin-bottom: 80px; overflow: hidden; position: relative; z-index: 1;">
  <img src="./Nattsu.jpg" alt="Nattsu" style="width: 100%; height: auto; display: block; max-height: 85vh; object-fit: cover;">
</div>

<!-- 全体の幅を整えるコンテナ（ここから下はそのまま） -->
<!-- 全体の幅を整えるコンテナ（ここから下はそのまま） -->
<!-- 全体の幅を整えるコンテナ -->
<div style="max-width: 900px; margin: 0 auto; padding: 0 20px; font-family: 'Helvetica Neue', Arial, sans-serif;">
  
  <!-- 2. WORK (制作実績) -->
  <div id="work" style="margin-bottom: 120px; text-align: left;">
    <h2 style="font-size: 1.8rem; font-weight: 300; letter-spacing: 2px; margin-bottom: 10px; border-bottom: 1px solid #111; padding-bottom: 5px; color: #111; border-top: none;">WORK</h2>
    <p style="font-size: 0.9rem; color: #666; margin-bottom: 30px;">制作実績</p>
    
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 20px;">
      <div style="border: 1px solid #ddd; padding: 15px; border-radius: 4px; background: #fff;">
        <div style="aspect-ratio: 4/3; background: #eee; margin-bottom: 10px; border-radius: 2px;"></div>
        <h3 style="font-size: 1rem; margin-bottom: 5px; color: #111;">Work 01</h3>
        <p style="font-size: 0.8rem; color: #666;">作品の説明がここに入ります。</p>
      </div>
      <div style="border: 1px solid #ddd; padding: 15px; border-radius: 4px; background: #fff;">
        <div style="aspect-ratio: 4/3; background: #eee; margin-bottom: 10px; border-radius: 2px;"></div>
        <h3 style="font-size: 1rem; margin-bottom: 5px; color: #111;">Work 02</h3>
        <p style="font-size: 0.8rem; color: #666;">作品の説明がここに入ります。</p>
      </div>
      <div style="border: 1px solid #ddd; padding: 15px; border-radius: 4px; background: #fff;">
        <div style="aspect-ratio: 4/3; background: #eee; margin-bottom: 10px; border-radius: 2px;"></div>
        <h3 style="font-size: 1rem; margin-bottom: 5px; color: #111;">Work 03</h3>
        <p style="font-size: 0.8rem; color: #666;">作品の説明がここに入ります。</p>
      </div>
    </div>
  </div>

  <!-- 3. PROFILE -->
  <div id="profile" style="margin-bottom: 120px; text-align: left;">
    <h2 style="font-size: 1.8rem; font-weight: 300; letter-spacing: 2px; margin-bottom: 30px; border-bottom: 1px solid #111; padding-bottom: 5px; color: #111; border-top: none;">PROFILE</h2>
    
    <div style="display: flex; flex-wrap: wrap; gap: 40px; align-items: flex-start;">
      <div style="width: 150px; height: 150px; background: #eee; border-radius: 4px; flex-shrink: 0;"></div>
      <div style="flex: 1; min-width: 280px; line-height: 1.8;">
        <p style="font-size: 1.1rem; font-weight: bold; margin-bottom: 10px; color: #111;">蓮田 瑞穂 / Mizuho Hasuda</p>
        <p style="color: #444; font-size: 0.95rem;">ここにプロフィールテキストを入力します。</p>
      </div>
    </div>
  </div>

  <!-- 4. PUBLICATION -->
  <div id="publication" style="margin-bottom: 120px; text-align: left;">
    <h2 style="font-size: 1.8rem; font-weight: 300; letter-spacing: 2px; margin-bottom: 30px; border-bottom: 1px solid #111; padding-bottom: 5px; color: #111; border-top: none;">PUBLICATION</h2>
    <p style="font-size: 0.95rem; color: #444;">学会発表や展示などの実績をここに記載します。</p>
  </div>

  <!-- 5. CONTACT -->
  <div id="contact" style="margin-bottom: 100px; text-align: left;">
    <h2 style="font-size: 1.8rem; font-weight: 300; letter-spacing: 2px; margin-bottom: 30px; border-bottom: 1px solid #111; padding-bottom: 5px; color: #111; border-top: none;">CONTACT</h2>
    <p style="font-size: 0.95rem; color: #444;">
      お問い合わせは以下までお願いいたします。<br>
      Email: <a href="mailto:your-email@example.com" style="color: #000; text-decoration: underline;">your-email@example.com</a>
    </p>
  </div>
</div>