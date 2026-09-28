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

.marquee-container {
overflow: hidden;
width: 100%;
margin-bottom: 40px;
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

<!-- メインビジュアル -->
<div style='width: 100%; margin: 0; padding: 0; overflow: hidden; position: relative; z-index: 1;'>
<img src='./Nattsu.jpg' alt='Nattsu' style='width: 100%; height: auto; display: block; max-height: 85vh; object-fit: cover;'>
</div>

<!-- コンテナ -->
<div style='max-width: 900px; margin: 80px auto 0; padding: 0 20px; font-family: "Helvetica Neue", Arial, sans-serif;'>

<!-- WORK (制作実績) -->
<div id='work' style='margin-bottom: 120px; text-align: left;'>
<div class='section-title-container'>
<div class='bg-en-title'>WORK</div>
<div class='fg-ja-title'>作品</div>
</div>

<div class='marquee-container'>
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
<h3 class='work-simple-title'>Echoes</h3>
</a>

<a href='./works/work06/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work06.jpg' alt='作品6' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
<h3 class='work-simple-title'>りびんぐすくえあ</h3>
</a>

<!-- ===== 2セット目（ループ用複製） ===== -->
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
<h3 class='work-simple-title'>Echoes</h3>
</a>

<a href='./works/work06/' class='work-simple-card'>
<div class='work-img-wrapper'>
<img src='./work06.jpg' alt='作品6' style='width: 100%; height: 100%; object-fit: cover; display: block;'>
</div>
<h3 class='work-simple-title'>りびんぐすくえあ</h3>
</a>
</div>
</div>

<!-- プロトタイプ集 -->
<h3 style='font-size: 1.1rem; font-weight: bold; margin: 40px 0 16px; padding-bottom: 6px; border-bottom: 2px solid #222; color: #111; width: 100%;'>プロトタイプ集</h3>

<dl style='display: grid; grid-template-columns: 100px 1fr; gap: 16px 20px; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0; width: 100%; box-sizing: border-box;'>
<dt style='font-weight: bold; color: #111; white-space: nowrap;'>作品 01</dt>
<dd style='margin: 0;'><a href='./works/work01/' style='color: #0066cc; text-decoration: underline; font-weight: bold;'>もわもわ</a></dd>

<dt style='font-weight: bold; color: #111; white-space: nowrap;'>作品 02</dt>
<dd style='margin: 0;'><a href='./works/work02/' style='color: #0066cc; text-decoration: underline; font-weight: bold;'>感情共有デバイス</a></dd>

<dt style='font-weight: bold; color: #111; white-space: nowrap;'>作品 03</dt>
<dd style='margin: 0;'><a href='./works/work03/' style='color: #0066cc; text-decoration: underline; font-weight: bold;'>奇跡の軌跡</a></dd>

<dt style='font-weight: bold; color: #111; white-space: nowrap;'>作品 04</dt>
<dd style='margin: 0;'><a href='./works/work04/' style='color: #0066cc; text-decoration: underline; font-weight: bold;'>視覚的モールス信号</a></dd>

<dt style='font-weight: bold; color: #111; white-space: nowrap;'>作品 05</dt>
<dd style='margin: 0;'><a href='./works/work05/' style='color: #0066cc; text-decoration: underline; font-weight: bold;'>Echoes</a></dd>

<dt style='font-weight: bold; color: #111; white-space: nowrap;'>作品 06</dt>
<dd style='margin: 0;'><a href='./works/work06/' style='color: #0066cc; text-decoration: underline; font-weight: bold;'>りびんぐすくえあ</a></dd>
</dl>
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
<div class='fg-ja-title'>活動</div>
</div>

<h3 style='font-size: 1.1rem; font-weight: bold; margin: 30px 0 16px; padding-bottom: 6px; border-bottom: 2px solid #222; color: #111; width: 100%;'>発表歴</h3>

<dl style='display: grid; grid-template-columns: 100px 1fr; gap: 16px 20px; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0 0 40px 0; width: 100%; box-sizing: border-box;'>
<dt style='font-weight: bold; color: #111; white-space: nowrap;'>2026.06</dt>
<dd style='margin: 0; width: 100%;'>
Mizuho Hasuda, Kota Kikuchi, Toshitaka Amaoka<br>
RibinguSukuea: Creating Lifelikeness through Perceptual Discrepancy and Interaction History<br>
NICOGRAPH International 2026, poster
</dd>

<dt style='font-weight: bold; color: #111; white-space: nowrap;'>2025.11</dt>
<dd style='margin: 0;'>
2025 大根田花柊, 蓮田瑞歩, 平松守瑠, 菊池康太<br>
Cam to Turn: オルゴールで奏でる人流データ<br>
芸術科学会 NICOGRAPH2025, ポスター発表
</dd>
</dl>

<h3 style='font-size: 1.1rem; font-weight: bold; margin: 30px 0 16px; padding-bottom: 6px; border-bottom: 2px solid #222; color: #111; width: 100%;'>その他参加歴</h3>

<dl style='display: grid; grid-template-columns: 100px 1fr; gap: 16px 20px; font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0; width: 100%; box-sizing: border-box;'>
<dt style='font-weight: bold; color: #111; white-space: nowrap;'>2026.08-09</dt>
<dd style='margin: 0; width: 100%;'>
<a href='https://yoso.sp.netkeiba.com/masters/ai2026_student/' target='_blank' style='color: #0066cc; text-decoration: underline; font-weight: bold;'>機械学習 全国学生大会 2026 AI競馬予想マスターズ</a><br>
大会総合ランキング 16位(的中率：39.18%)<br>
</dd>
</dl>
</div>

<!-- CONTACT (お問い合わせ) -->
<div id='contact' style='margin-bottom: 120px; text-align: left;'>
<div class='section-title-container'>
<div class='bg-en-title'>CONTACT</div>
<div class='fg-ja-title'>お問い合わせ</div>
</div>

<p style='font-size: 0.95rem; color: #444; line-height: 1.8; margin-bottom: 16px;'>
お問い合わせやご連絡は、以下のメールアドレスまでお願いいたします。
</p>

<div style='font-size: 1.05rem; font-weight: bold;'>
<a href='mailto:mizuho.nattsu.0809@gmail.com' style='color: #0066cc; text-decoration: underline;'>mizuho.nattsu.0809@gmail.com</a>
</div>
</div>

</div>