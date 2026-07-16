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
</style>

<!-- メインビジュアル -->
<div style="width: 100%; margin: 0; padding: 0; overflow: hidden; position: relative; z-index: 1;">
  <img src="./Nattsu.jpg" alt="Nattsu" style="width: 100%; height: auto; display: block; max-height: 85vh; object-fit: cover;">
</div>

<!-- コンテナ -->
<div style="max-width: 900px; margin: 80px auto 0; padding: 0 20px; font-family: 'Helvetica Neue', Arial, sans-serif;">

  <!-- WORK (制作実績) -->
  <div id="work" style="margin-bottom: 120px; text-align: left;">
    <div class="section-title-container">
      <div class="bg-en-title">WORK</div>
      <div class="fg-ja-title">制作実績</div>
    </div>
    
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

  <!-- PROFILE -->
  <div id="profile" style="margin-bottom: 120px; text-align: left;">
    <div class="section-title-container">
      <div class="bg-en-title">PROFILE</div>
      <div class="fg-ja-title">自己紹介</div>
    </div>
    
    <div style="display: flex; flex-wrap: wrap; gap: 40px; align-items: flex-start;">
      <div style="width: 150px; height: 150px; background: #eee; border-radius: 4px; flex-shrink: 0;"></div>
      <div style="flex: 1; min-width: 280px; line-height: 1.8;">
        <p style="font-size: 1.1rem; font-weight: bold; margin-bottom: 10px; color: #111;">蓮田 瑞穂 / Mizuho Hasuda</p>
        <p style="color: #444; font-size: 0.95rem;">ここにプロフィールテキストを入力します。</p>
      </div>
    </div>
  </div>

  <!-- CONTACT -->
  <div id="contact" style="margin-bottom: 100px; text-align: left;">
    <div class="section-title-container">
      <div class="bg-en-title">CONTACT</div>
      <div class="fg-ja-title">お問い合わせ</div>
    </div>
    
    <p style="font-size: 0.95rem; color: #444;">
      Email: <a style="color: #000; text-decoration: underline;" href="mailto:mizuho.nattsu.0809@gmail.com">mizuho.nattsu.0809@gmail.com</a>
    </p>
  </div>
</div>