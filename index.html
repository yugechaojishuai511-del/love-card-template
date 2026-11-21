
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#fff5f7">
<title>给你的一封情书</title>
<style>
:root {
  --pink: #e98da7;
  --deep: #8e5267;
  --cream: #fff8f3;
  --rose: #f7dce4;
}
* { box-sizing: border-box; }
html { scroll-behavior: smooth; }
body {
  margin: 0;
  color: #795263;
  font-family: -apple-system, BlinkMacSystemFont, "PingFang SC",
    "Microsoft YaHei", sans-serif;
  background:
    radial-gradient(circle at 10% 10%, #fff1f5, transparent 40%),
    radial-gradient(circle at 90% 30%, #ffe7ee, transparent 35%),
    #fffaf6;
  overflow-x: hidden;
}
button { font: inherit; cursor: pointer; }
button:focus-visible { outline: 3px solid #c86b89; outline-offset: 4px; }

#intro {
  position: fixed;
  inset: 0;
  z-index: 20;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #fff3f6, #f9dce6);
  transition: opacity .9s, visibility .9s;
}
#intro.hide { opacity: 0; visibility: hidden; pointer-events: none; }
.envelope-wrap { text-align: center; padding: 20px; }
.envelope {
  position: relative;
  width: min(320px, 80vw);
  height: 210px;
  margin: 30px auto;
  background: #e9a4b8;
  border-radius: 12px;
  box-shadow: 0 18px 45px #c77e9638;
  cursor: pointer;
  transition: transform .4s;
}
.envelope:hover { transform: translateY(-6px); }
.envelope::before {
  content: "";
  position: absolute;
  inset: 0;
  background: #f4c4d2;
  clip-path: polygon(0 0, 100% 0, 50% 62%);
  border-radius: 12px;
  transform-origin: top;
  transition: transform .7s;
  z-index: 2;
}
.envelope.open::before { transform: rotateX(180deg); }
.envelope::after {
  content: "♥";
  position: absolute;
  top: 85px;
  left: 50%;
  transform: translateX(-50%);
  font-size: 42px;
  color: #fff8f8;
  z-index: 3;
}
.envelope-label {
  position: absolute;
  bottom: 25px;
  width: 100%;
  text-align: center;
  font-size: 18px;
  color: #fff;
  letter-spacing: 4px;
}
.open-btn, .pill {
  border: none;
  border-radius: 999px;
  background: #d97998;
  color: white;
  padding: 13px 28px;
  box-shadow: 0 8px 20px #d9799833;
  transition: transform .2s, background .2s;
}
.open-btn:hover, .pill:hover { transform: translateY(-2px); background: #c96889; }
.small-note { color: #a67b8b; font-size: 13px; }

main {
  max-width: 760px;
  margin: auto;
  padding: 30px 20px 80px;
}
.hero { text-align: center; padding: 55px 10px 30px; }
.tag {
  letter-spacing: 4px;
  color: #bd8297;
  font-size: 12px;
}
h1 {
  font-weight: 500;
  font-size: clamp(32px, 8vw, 52px);
  color: var(--deep);
  line-height: 1.4;
  margin: 18px 0;
}
.subtitle { line-height: 2; font-size: 15px; color: #9a7182; }
.divider {
  width: 70px;
  height: 1px;
  background: #e9b9c9;
  margin: 30px auto;
}
.section { margin: 45px 0; }
.section-title {
  text-align: center;
  font-size: 24px;
  font-weight: 500;
  color: var(--deep);
  margin-bottom: 12px;
}
.section-sub { text-align: center; color: #b28a98; font-size: 13px; }
.photos {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 15px;
  margin-top: 28px;
}
.photo {
  padding: 10px 10px 18px;
  background: white;
  border-radius: 12px;
  box-shadow: 0 10px 35px #a36d7a15;
  transform: rotate(-1deg);
}
.photo:nth-child(2) { transform: rotate(2deg); }
.photo:nth-child(3) { transform: rotate(1deg); }
.photo img {
  width: 100%;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  border-radius: 8px;
  display: block;
}
.photo p { text-align: center; font-size: 13px; margin: 12px 0 0; color: #a47c8b; }
.counter {
  background: linear-gradient(135deg, #fff, #fff2f5);
  border: 1px solid #f5dce5;
  border-radius: 22px;
  padding: 30px 15px;
  text-align: center;
  box-shadow: 0 10px 30px #dba0b215;
}
.counter-number {
  font-size: 44px;
  color: #d97998;
  font-family: Georgia, serif;
}
.counter-caption { margin-top: 10px; font-size: 14px; }
.letter {
  background: #fff;
  border-radius: 22px;
  padding: clamp(25px, 7vw, 42px);
  box-shadow: 0 15px 40px #ad778218;
  line-height: 2.2;
  font-size: 16px;
  border: 1px solid #f8e6eb;
}
.letter-head { text-align: center; color: #d97998; font-size: 22px; margin-bottom: 20px; }
.letter-text { white-space: pre-line; }
.signature { text-align: right; margin-top: 30px; color: #d97998; }
.surprise {
  text-align: center;
  margin: 35px 0;
}
#secret {
  display: none;
  background: #fff0f5;
  padding: 25px;
  border-radius: 20px;
  text-align: center;
  margin-top: 20px;
  line-height: 2;
  animation: fadeIn .8s;
}
#secret.show { display: block; }
.footer { text-align: center; font-size: 13px; color: #bb91a1; margin-top: 60px; }
.float-heart {
  position: fixed;
  pointer-events: none;
  z-index: 1;
  bottom: -40px;
  animation: floatUp linear forwards;
  opacity: .65;
}
@keyframes floatUp {
  to { transform: translateY(-110vh) rotate(30deg); opacity: 0; }
}
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}
@media(max-width: 520px) {
  main { padding: 20px 16px 60px; }
  .photos { gap: 10px; }
  .photo { padding: 7px 7px 14px; }
  .letter { font-size: 15px; }
}
@media(prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: .01ms !important;
    transition-duration: .01ms !important;
    scroll-behavior: auto !important;
  }
}
</style>
</head>
<body>

<!-- 开场信封 -->
<div id="intro">
  <div class="envelope-wrap">
    <p class="tag">A LITTLE LOVE LETTER</p>
    <h1 style="font-size:32px">有一份惊喜给你</h1>
    <div class="envelope" id="envelope" onclick="openLetter()">
      <div class="envelope-label">给最特别的你</div>
    </div>
    <button class="open-btn" onclick="openLetter()">打开这封信 ♥</button>
    <p class="small-note">轻轻点击，开启一份温柔</p>
  </div>
</div>

<main>
  <header class="hero">
    <p class="tag">TO MY FAVORITE PERSON</p>
    <h1 id="headline">遇见你，是我的浪漫</h1>
    <p class="subtitle">
      有些心意想慢慢说给你听。<br>
      今天也想把所有温柔，送给你。
    </p>
    <div class="divider"></div>
    <div style="font-size:32px">♡ ✧ ♡</div>
  </header>

  <!-- 照片区域：可以替换为你自己的照片网址 -->
  <section class="section">
    <h2 class="section-title">我们的美好瞬间</h2>
    <p class="section-sub">每一个值得珍藏的时刻</p>
    <div class="photos">
      <div class="photo">
        <img src="https://images.unsplash.com/photo-1516589178581-6cd7833ae3b2?auto=format&fit=crop&w=800&q=85" alt="浪漫时刻">
        <p>温柔的瞬间</p>
      </div>
      <div class="photo">
        <img src="https://images.unsplash.com/photo-1518199266791-5375a83190b7?auto=format&fit=crop&w=800&q=85" alt="花朵">
        <p>想与你分享</p>
      </div>
      <div class="photo">
        <img src="https://images.unsplash.com/photo-1518621736915-f3b1c41bfd00?auto=format&fit=crop&w=800&q=85" alt="浪漫夕阳">
        <p>平凡也浪漫</p>
      </div>
      <div class="photo">
        <img src="https://images.unsplash.com/photo-1516589091380-5d8e1a3a8f5b?auto=format&fit=crop&w=800&q=85" alt="浪漫花束">
        <p>把美好留住</p>
      </div>
    </div>
  </section>

  <!-- 纪念日计时 -->
  <section class="section">
    <h2 class="section-title">我们的时间</h2>
    <p class="section-sub">时间在走，心意不变</p>
    <div class="counter">
      <div class="counter-number" id="days">0</div>
      <div class="counter-caption">天 · 每一天都值得珍惜</div>
    </div>
  </section>

  <!-- 情书 -->
  <section class="section">
    <h2 class="section-title">想对你说的话</h2>
    <p class="section-sub">请慢慢读完这封信</p>
    <div class="letter">
      <div class="letter-head">亲爱的你 ♡</div>
      <div class="letter-text" id="letterText"></div>
      <div class="signature">—— 永远珍惜你的人</div>
    </div>
  </section>

  <!-- 隐藏惊喜 -->
  <section class="section surprise">
    <button class="pill" onclick="showSecret()">点击查看隐藏惊喜 ♥</button>
    <div id="secret">
      <div style="font-size:36px">💗</div>
      <p>如果浪漫有形状，</p>
      <p>那一定是与你相处的每一个瞬间。</p>
      <p>愿我们永远有说不完的话，</p>
      <p>有看不完的风景，</p>
      <p>有彼此陪伴的未来。✨</p>
    </div>
  </section>

  <section class="section" style="text-align:center">
    <button class="pill" onclick="toggleMusic()">♫ 音乐播放 / 暂停</button>
    <p class="small-note" id="musicHint">音乐功能需要添加自己的音乐文件</p>
    <div style="margin-top:18px">
      <button class="pill" onclick="sharePage()">分享这份浪漫 ♡</button>
    </div>
  </section>

  <footer class="footer">
    Made with love ♥<br>
    希望你永远被温柔对待
  </footer>
</main>

<!-- 可选音乐：在下面填入自己的音乐文件网址 -->
<audio id="music" loop></audio>

<script>
/* =================================================
   个性化设置区：以后定制客户时主要修改这里
   ================================================= */

// 纪念日日期：格式 YYYY-MM-DD
const anniversaryDate = "2024-05-20";

// 情书内容
const letterContent = `谢谢你来到我的世界。

生活有时候很普通，
但因为有你，
一些小小的日常也变得闪闪发光。

希望你开心的时候有人分享，
难过的时候有人拥抱。

愿未来的日子，
我们都能成为更好的自己，
也继续把温柔留给彼此。

今天、明天、以后，
都想好好珍惜你。`;

// 音乐文件网址（可选）
// 例如： "music.mp3"（如果文件放在仓库根目录）
// 为空则不播放
const musicSource = "";

/* ================================================= */

const letterEl = document.getElementById("letterText");
const musicEl = document.getElementById("music");
let typingStarted = false;
let musicPlaying = false;

function openLetter() {
  document.getElementById("envelope").classList.add("open");
  document.getElementById("intro").classList.add("hide");
  if (!typingStarted) {
    typingStarted = true;
    typeLetter();
  }
}

function typeLetter() {
  // 优先考虑可访问性及减少动态效果偏好
  if (window.matchMedia("(prefers-reduced-motion: reduce)").matches) {
    letterEl.textContent = letterContent;
    return;
  }
  let i = 0;
  function type() {
    if (i < letterContent.length) {
      letterEl.textContent += letterContent.charAt(i);
      i++;
      setTimeout(type, 45);
    }
  }
  type();
}

// 计算相识纪念日天数
function updateDays() {
  const start = new Date(anniversaryDate + "T00:00:00");
  const now = new Date();
  const today = new Date(now.getFullYear(), now.getMonth(), now.getDate());
  const diff = Math.floor((today - start) / (1000 * 60 * 60 * 24));
  document.getElementById("days").textContent = Math.max(diff, 0);
}
updateDays();

function showSecret() {
  const secret = document.getElementById("secret");
  secret.classList.toggle("show");
}

function toggleMusic() {
  if (!musicSource) {
    document.getElementById("musicHint").textContent =
      "请在代码个性化设置区添加 music.mp3 文件网址后使用";
    return;
  }
  if (!musicEl.src) musicEl.src = musicSource;
  if (musicPlaying) {
    musicEl.pause();
    musicPlaying = false;
  } else {
    musicEl.play().then(() => {
      musicPlaying = true;
    }).catch(() => {
      document.getElementById("musicHint").textContent =
        "浏览器未允许播放，请再次点击按钮";
    });
  }
}

async function sharePage() {
  const url = location.href;
  if (navigator.share) {
    try {
      await navigator.share({
        title: document.title,
        text: "送你一份小小的浪漫 ♥",
        url: url
      });
      return;
    } catch (e) {}
  }
  try {
    await navigator.clipboard.writeText(url);
    alert("网页链接已复制，可以发送给对方啦 ♥");
  } catch (e) {
    prompt("复制下面的网址分享：", url);
  }
}

// 漂浮爱心
function createHeart() {
  if (window.matchMedia("(prefers-reduced-motion: reduce)").matches) return;
  const heart = document.createElement("div");
  heart.className = "float-heart";
  heart.textContent = ["♥", "♡", "💗", "✧", "💕"][Math.floor(Math.random()*5)];
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.fontSize = (14 + Math.random() * 20) + "px";
  heart.style.animationDuration = (6 + Math.random() * 6) + "s";
  document.body.appendChild(heart);
  setTimeout(() => heart.remove(), 12000);
}
setInterval(createHeart, 800);
</script>
</body>
</html>
