---
layout: "single"
---

<style>
body {
  margin: 0 !important;
  padding: 0 !important;
  overflow-x: hidden;
}

.container {
  max-width: 100% !important;
  padding: 0 !important;
  margin: 0 !important;
}

.main {
  margin-top: 0 !important;
  padding-top: 60px !important;
  max-width: 100% !important;
}

.post-header, .post-meta {
  margin: 0 !important;
  padding: 0 !important;
}

.post-content {
  width: 80% !important;
  max-width: 2000px !important;
  min-width: 320px;
  margin: 0 auto !important;
  padding: 0 !important;
  box-sizing: border-box;
}

header.header {
  position: fixed !important;
  top: 0 !important;
  left: 0 !important;
  width: 100% !important;
  background: rgba(255, 255, 255, 0.85) !important; 
  backdrop-filter: blur(12px) !important; 
  -webkit-backdrop-filter: blur(12px) !important;
  z-index: 999 !important; 
  border: none !important;
  padding: 0 !important; 
  box-sizing: border-box;
}

header.header nav.nav {
  width: 80% !important;
  max-width: 2000px !important;
  margin: 0 auto !important;
  min-height: 48px !important;
  height: 48px !important;
  display: flex !important;
  align-items: center !important;
  justify-content: space-between !important;
  padding: 0 !important;
  box-sizing: border-box;
}

.logo a {
  line-height: 48px !important;
  margin: 0 !important;
  padding: 0 !important;
}

ul#menu {
  align-items: center !important;
  margin: 0 !important;
  padding-right: 0 !important;
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
  margin-bottom: 30px;
  height: 80px;
  width: 100%;
}

.bg-en-title {
  position: absolute;
  top: 0;
  left: 0;
  font-size: 4rem;
  font-weight: 800;
  color: rgba(60, 179, 113, 0.35);
  line-height: 1;
  letter-spacing: 4px;
  user-select: none;
}

.fg-ja-title {
  position: absolute;
  bottom: 5px;
  left: 0;
  font-size: 1.5rem;
  font-weight: 700;
  color: #111;
  line-height: 1;
  z-index: 2;
}

.marquee-container {
  overflow: hidden;
  width: 100%;
  margin-bottom: 20px; /* カプセルボタンとの間隔を調整するため少し詰めています */
  text-align: left;
}

.marquee-track {
  display: flex;
  gap: 20px;
  width: max-content;
  animation: marquee-scroll 25s linear infinite;
}

.marquee-container:hover .marquee-track {
  animation-play-state: paused;
}

@keyframes marquee-scroll {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

/* カプセル型 VIEW MORE ボタンのスタイル */
.view-more-btn-wrapper {
  display: flex;
  justify-content: flex-end; /* 右寄せ（中央にしたい場合は center に変更） */
  margin: 0 0 50px 0;
  width: 100%;
}

.view-more-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  padding: 12px 32px;
  font-size: 0.95rem;
  font-weight: 700;
  letter-spacing: 1.5px;
  color: #111;
  background-color: transparent;
  border: 2px solid #111;
  border-radius: 50px;
  text-decoration: none !important;
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

.view-more-btn .arrow {
  display: inline-block;
  font-size: 1.1rem;
  transition: transform 0.3s ease;
}

.view-more-btn:hover {
  background-color: #111;
  color: #fff !important;
  transform: translateY(-2px);
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.15);
}

.view-more-btn:hover .arrow {
  transform: translateX(5px);
}

.work-simple-card {
  width: 240px;
  text-decoration: none;
  color: inherit;
  display: flex;
  flex-direction: column;
  transition: transform 0.2s ease, opacity 0.2s ease;
  flex-shrink: 0;
  background: transparent !important;
  border: none !important;
  box-shadow: none !important;
  padding: 0 !important;
}

.work-simple-card:hover {
  transform: translateY(-4px);
  opacity: 0.85;
}

.work-img-wrapper {
  width: 100%;
  aspect-ratio: 16/10;
  background: transparent !important;
  margin-bottom: 8px;
  border-radius: 6px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0,0,0,0.06);
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

<!-- マウスの周りだけが波打つように上品に浮き上がる立方体グリッド -->
<style>
.interactive-hero-container {
  width: 100%;
  margin: 20px 0 60px 0;
  border-radius: 8px;
  overflow: hidden;
  position: relative;
  background: #111;
  aspect-ratio: 16/9;
  max-height: 70vh;
}
.interactive-hero-container canvas {
  display: block;
  width: 100%;
  height: 100%;
  cursor: pointer;
}
</style>

<div class="interactive-hero-container">
  <canvas id="cubeWaveCanvas"></canvas>
</div>

<script>
(function() {
  const canvas = document.getElementById('cubeWaveCanvas');
  const ctx = canvas.getContext('2d');

  let cols = 16;
  let rows = 10;
  let mouse = { x: -1000, y: -1000, radius: 140 };

  function resize() {
    canvas.width = canvas.parentElement.clientWidth;
    canvas.height = canvas.parentElement.clientHeight;
  }
  window.addEventListener('resize', resize);
  resize();

  canvas.addEventListener('mousemove', (e) => {
    const rect = canvas.getBoundingClientRect();
    mouse.x = e.clientX - rect.left;
    mouse.y = e.clientY - rect.top;
  });

  canvas.addEventListener('mouseleave', () => {
    mouse.x = -1000;
    mouse.y = -1000;
  });

  let angle = 0;

  function draw() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    const cellWidth = canvas.width / cols;
    const cellHeight = canvas.height / rows;

    angle += 0.04;

    for (let i = 0; i < cols; i++) {
      for (let j = 0; j < rows; j++) {
        let x = i * cellWidth + cellWidth / 2;
        let y = j * cellHeight + cellHeight / 2;

        let dx = mouse.x - x;
        let dy = mouse.y - y;
        let dist = Math.sqrt(dx * dx + dy * dy);

        let offsetY = 0;
        let scale = 1;

        if (dist < mouse.radius) {
          let force = (1 - dist / mouse.radius);
          offsetY = -Math.sin(angle * 2.5 + dist * 0.08) * 12 * force;
          scale = 1 + force * 0.15;
        }

        ctx.save();
        ctx.translate(x, y + offsetY);
        ctx.scale(scale, scale);

        let size = Math.min(cellWidth, cellHeight) * 0.78;
        
        ctx.fillStyle = '#dcdcdc';
        ctx.fillRect(-size/2, -size/2, size, size);
        
        ctx.strokeStyle = '#2b2b2b';
        ctx.lineWidth = 1.5;
        ctx.strokeRect(-size/2, -size/2, size, size);

        ctx.fillStyle = 'rgba(255, 255, 255, 0.3)';
        ctx.beginPath();
        ctx.moveTo(-size/2, -size/2);
        ctx.lineTo(size/2, -size/2);
        ctx.lineTo(size/2 - 4, -size/2 - 6);
        ctx.lineTo(-size/2 + 4, -size/2 - 6);
        ctx.closePath();
        ctx.fill();

        ctx.restore();
      }
    }

    requestAnimationFrame(draw);
  }

  draw();
})();
</script>

<div style="width: 100%; font-family: 'Helvetica Neue', Arial, sans-serif;">

<div id="work" style="margin-bottom: 120px; text-align: left;">

<div class="section-title-container">
<div class="bg-en-title">WORKS</div>
<div class="fg-ja-title">作品</div>
</div>

<div class="marquee-container">
<div class="marquee-track">

<a href="./works/work01/" class="work-simple-card">
<div class="work-img-wrapper">
<img src="./work01.jpg" alt="作品1" style="width: 100%; height: 100%; object-fit: cover; display: block;">
</div>
<h3 class="work-simple-title">Echoes</h3>
</a>

<a href="./works/work02/" class="work-simple-card">
<div class="work-img-wrapper">
<img src="./work02.jpg" alt="作品2" style="width: 100%; height: 100%; object-fit: cover; display: block;">
</div>
<h3 class="work-simple-title">Cam to Turn</h3>
</a>

<a href="./works/work03/" class="work-simple-card">
<div class="work-img-wrapper">
<img src="./work03.jpg" alt="作品3" style="width: 100%; height: 100%; object-fit: cover; display: block;">
</div>
<h3 class="work-simple-title">りびんぐすくえあ</h3>
</a>

<a href="./works/work01/" class="work-simple-card">
<div class="work-img-wrapper">
<img src="./work01.jpg" alt="作品1" style="width: 100%; height: 100%; object-fit: cover; display: block;">
</div>
<h3 class="work-simple-title">Echoes</h3>
</a>

<a href="./works/work02/" class="work-simple-card">
<div class="work-img-wrapper">
<img src="./work02.jpg" alt="作品2" style="width: 100%; height: 100%; object-fit: cover; display: block;">
</div>
<h3 class="work-simple-title">Cam to Turn</h3>
</a>

<a href="./works/work03/" class="work-simple-card">
<div class="work-img-wrapper">
<img src="./work03.jpg" alt="作品3" style="width: 100%; height: 100%; object-fit: cover; display: block;">
</div>
<h3 class="work-simple-title">りびんぐすくえあ</h3>
</a>


</div>
</div>

<!-- 作品カルーセルの直下に置いたカプセル型ボタン -->
<div class="view-more-btn-wrapper">
  <a href="./works/" class="view-more-btn">
    VIEW MORE <span class="arrow">→</span>
  </a>
</div>

<!-- プロトタイプ集の見出し -->
<div style="margin: 30px 0 16px 0; border-bottom: 2px solid #222; padding-bottom: 6px; width: 100%;">
<h3 style="font-size: 1.1rem; font-weight: bold; margin: 0; color: #111;">プロトタイプ集</h3>
</div>

<dl style="display: grid; grid-template-columns: 100px 1fr; gap: 16px 20px; align-items: center; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0; width: 100%; box-sizing: border-box;">
<dt style="font-weight: bold; color: #111; white-space: nowrap; margin: 0;">No.01</dt>
<dd style="margin: 0;"><a href="./works/p01/" style="color: #0066cc; text-decoration: underline; font-weight: bold;">もわもわ</a></dd>

<dt style="font-weight: bold; color: #111; white-space: nowrap; margin: 0;">No.02</dt>
<dd style="margin: 0;"><a href="./works/p02/" style="color: #0066cc; text-decoration: underline; font-weight: bold;">感情共有デバイス</a></dd>

<dt style="font-weight: bold; color: #111; white-space: nowrap; margin: 0;">No.03</dt>
<dd style="margin: 0;"><a href="./works/p03/" style="color: #0066cc; text-decoration: underline; font-weight: bold;">視覚的モールス信号</a></dd>

<dt style="font-weight: bold; color: #111; white-space: nowrap; margin: 0;">No.04</dt>
<dd style="margin: 0;"><a href="./works/p04/" style="color: #0066cc; text-decoration: underline; font-weight: bold;">5秒間の軌跡</a></dd>
</dl>
</div>

<div id="profile" style="margin-bottom: 120px; text-align: left;">
<div class="section-title-container">
<div class="bg-en-title">PROFILE</div>
<div class="fg-ja-title">自己紹介</div>
</div>

<div style="display: flex; flex-wrap: wrap; gap: 40px; align-items: flex-start;">
<img src="./profile.jpg" alt="蓮田 瑞歩" style="width: 150px; height: 150px; object-fit: cover; border-radius: 50%; flex-shrink: 0;">

<div style="flex: 1; min-width: 280px;">
<p style="font-size: 1.2rem; font-weight: bold; margin-bottom: 20px; color: #111;">蓮田 瑞歩 / Mizuho Hasuda</p>

<dl style="display: grid; grid-template-columns: 120px 1fr; gap: 16px 20px; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0;">
<dt style="font-weight: bold; color: #111; white-space: nowrap;">所属</dt>
<dd style="margin: 0;">明星大学 情報学部 情報学科 4年生</dd>

<dt style="font-weight: bold; color: #111; white-space: nowrap;">研究室</dt>
<dd style="margin: 0;">インタラクティブメディア 研究室</dd>

<dt style="font-weight: bold; color: #111; white-space: nowrap;">連絡先</dt>
<dd style="margin: 0;"><a href="mailto:mizuho.nattsu.0809@gmail.com" style="color: #333; text-decoration: underline;">mizuho.nattsu.0809@gmail.com</a></dd>

<dt style="font-weight: bold; color: #111; white-space: nowrap;">趣味</dt>
<dd style="margin: 0;">カメラ、馬、おもちゃ</dd>
</dl>
</div>
</div>
</div>

<div id="achievements" style="margin-bottom: 120px; text-align: left;">
<div class="section-title-container">
<div class="bg-en-title">ACHIEVEMENTS</div>
<div class="fg-ja-title">活動</div>
</div>

<h3 style="font-size: 1.1rem; font-weight: bold; margin: 30px 0 16px; padding-bottom: 6px; border-bottom: 2px solid #222; color: #111; width: 100%;">発表歴</h3>

<dl style="display: grid; grid-template-columns: 100px 1fr; gap: 16px 20px; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0 0 40px 0; width: 100%; box-sizing: border-box;">
<dt style="font-weight: bold; color: #111; white-space: nowrap;">2026.06</dt>
<dd style="margin: 0; width: 100%;">
Mizuho Hasuda, Kota Kikuchi, Toshitaka Amaoka<br>
RibinguSukuea: Creating Lifelikeness through Perceptual Discrepancy and Interaction History<br>
NICOGRAPH International 2026, poster
</dd>

<dt style="font-weight: bold; color: #111; white-space: nowrap;">2025.11</dt>
<dd style="margin: 0;">
2025 大根田花柊, 蓮田瑞歩, 平松守瑠, 菊池康太<br>
Cam to Turn: オルゴールで奏でる人流データ<br>
芸術科学会 NICOGRAPH2025, ポスター発表
</dd>
</dl>

<h3 style="font-size: 1.1rem; font-weight: bold; margin: 30px 0 16px; padding-bottom: 6px; border-bottom: 2px solid #222; color: #111; width: 100%;">その他参加歴</h3>

<dl style="display: grid; grid-template-columns: 100px 1fr; gap: 16px 20px; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0; width: 100%; box-sizing: border-box;">
<dt style="font-weight: bold; color: #111; white-space: nowrap;">2026.08-09</dt>
<dd style="margin: 0; width: 100%;">
<a href="https://yoso.sp.netkeiba.com/masters/ai2026_student/" target="_blank" style="color: #0066cc; text-decoration: underline; font-weight: bold;">機械学習 全国学生大会 2026 AI競馬予想マスターズ</a><br>
大会総合ランキング 16位(的中率：39.18%)<br>
</dd>
</dl>
</div>

<div id="contact" style="margin-bottom: 120px; text-align: left;">
<div class="section-title-container">
<div class="bg-en-title">CONTACT</div>
<div class="fg-ja-title">お問い合わせ</div>
</div>

<p style="font-size: 0.95rem; color: #444; line-height: 1.8; margin-bottom: 16px;">
お問い合わせやご連絡は、以下のメールアドレスまでお願いいたします。
</p>

<div style="font-size: 1.05rem; font-weight: bold;">
<a href="mailto:mizuho.nattsu.0809@gmail.com" style="color: #0066cc; text-decoration: underline;">mizuho.nattsu.0809@gmail.com</a>
</div>
</div>

</div>