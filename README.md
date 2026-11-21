
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>给你的一封情书</title>
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", sans-serif;
  background: #fff5f7;
  color: #754452;
  overflow-x: hidden;
}
.page {
  min-height: 100vh;
  padding: 30px 20px 60px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  position: relative;
}
.intro {
  position: fixed;
  inset: 0;
  z-index: 10;
  background: linear-gradient(145deg,#f8dce6,#fff4f4,#f5d4df);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: opacity .8s, transform .8s;
}
.intro.hide {
  opacity: 0;
  pointer-events: none;
  transform: scale(1.08);
}
.envelope {
  width: 240px;
  height: 155px;
  position: relative;
  cursor: pointer;
  margin: 30px;
  background: #eaa9bf;
  border-radius: 12px;
  box-shadow: 0 15px 40px #c47b9580;
}
.envelope:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  border-left: 120px solid transparent;
  border-right: 120px solid transparent;
  border-top: 90px solid #f4c4d4;
  z-index: 2;
}
.envelope:after {
  content: "♥";
  position: absolute;
  left: 50%;
  top: 53%;
  transform: translate(-50%,-50%);
  color: white;
  font-size: 35px;
  z-index: 3;
}
.intro h1 {
  font-size: 28px;
  color: #a34f6c;
  margin-bottom: 12px;
}
.intro p { color: #a36b7f; }
.open-btn {
  border: none;
  background: #b85e7d;
  color: white;
  padding: 14px 30px;
  border-radius: 30px;
  margin-top: 20px;
  font-size: 16px;
  box-shadow: 0 5px 20px #b85e7d55;
  cursor: pointer;
}
.card {
  max-width: 430px;
  width: 100%;
  border-radius: 26px;
  padding: 30px 22px;
  background: rgba(255,255,255,.85);
  box-shadow: 0 10px 45px #b8788b22;
  text-align: center;
  position: relative;
}
.tag {
  letter-spacing: 4px;
  font-size: 12px;
  color: #bc8295;
}
h2 {
  font-size: 30px;
  margin: 18px 0;
  color: #a14f6d;
}
.message {
  line-height: 2;
  color: #815568;
  font-size: 16px;
}
.photo {
  width: 100%;
  height: 260px;
  margin: 24px 0;
  border-radius: 20px;
  background: linear-gradient(145deg,#f5d8e2,#eec4d5,#f9e8eb);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  overflow: hidden;
  color: #9c5d75;
}
.photo span { font-size: 50px; }
.photo small { margin-top: 10px; }
.divider {
  width: 60px;
  height: 2px;
  background: #edc0d0;
  margin: 22px auto;
}
.love {
  font-size: 35px;
  animation: beat 1.3s infinite;
}
.btn {
  border: none;
  background: #c46c89;
  color: white;
  border-radius: 30px;
  padding: 13px 24px;
  font-size: 15px;
  margin-top: 20px;
  cursor: pointer;
}
.hidden { display: none; }
.surprise {
  margin-top: 22px;
  line-height: 2;
  color: #b25477;
  animation: fade .8s;
}
.floating {
  position: fixed;
  pointer-events: none;
  bottom: -30px;
  animation: floatUp linear forwards;
  z-index: 1;
}
footer {
  margin-top: 25px;
  font-size: 12px;
  color: #b58b9b;
}
@keyframes beat {
  50% { transform: scale(1.18); }
}
@keyframes floatUp {
  to { transform: translateY(-110vh) rotate(30deg); opacity: 0; }
}
@keyframes fade {
  from { opacity: 0; transform: translateY(15px); }
  to { opacity: 1; transform: translateY(0); }
}
</style>
</head>
<body>

<div class="intro" id="intro">
  <h1>有一份小小的惊喜</h1>
  <p>我想把一些温柔送给你</p>
  <div class="envelope" onclick="openCard()"></div>
  <button class="open-btn" onclick="openCard()">点击打开信件</button>
  <p style="margin-top:25px;font-size:13px;">♡ 给特别的你 ♡</p>
</div>

<div class="page">
  <main class="card">
    <div class="tag">A LITTLE LOVE LETTER</div>
    <div class="love">💗</div>
    <h2>生日快乐</h2>

    <p class="message">
      在这个特别的日子，<br>
      想把最温柔的祝福送给你。<br>
      愿你所遇皆美好，<br>
      所想皆如愿。
    </p>

    <div class="photo">
      <span>🌷</span>
      <small>这里是属于你们的照片位置</small>
    </div>

    <div class="divider"></div>

    <p class="message">
      愿你被世界温柔以待，<br>
      愿每一个平凡的日子<br>
      都有值得期待的小惊喜。
    </p>

    <button class="btn" onclick="showSurprise()">还有一份惊喜 ✨</button>

    <div class="surprise hidden" id="surprise">
      <h3>💌 想对你说</h3>
      <p>
        你值得所有美好。<br>
        愿快乐永远陪伴你，<br>
        愿未来的每一天都闪闪发光。
      </p>
      <p>♡ 爱与祝福 ♡</p>
    </div>
    <footer>Made with love ♡</footer>
  </main>
</div>

<script>
function openCard() {
  document.getElementById("intro").classList.add("hide");
}

function showSurprise() {
  const el = document.getElementById("surprise");
  el.classList.toggle("hidden");
}

function createHeart() {
  const h = document.createElement("div");
  h.className = "floating";
  h.innerHTML = ["💗","💕","🌸","♡","✨"][Math.floor(Math.random()*5)];
  h.style.left = Math.random()*100+"vw";
  h.style.animationDuration = (5+Math.random()*5)+"s";
  h.style.fontSize = (16+Math.random()*20)+"px";
  document.body.appendChild(h);
  setTimeout(()=>h.remove(),10000);
}
setInterval(createHeart,800);
</script>
</body>
</html>
