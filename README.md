
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>给你的一封信</title>
<style>
*{box-sizing:border-box}
body{
  margin:0;min-height:100vh;
  font-family:"PingFang SC","Microsoft YaHei",sans-serif;
  color:#633d4d;
  background:linear-gradient(145deg,#fff0f4,#fce4ec,#fff5e8);
  display:flex;justify-content:center;align-items:center;
  padding:24px;overflow-x:hidden
}
.wrap{width:100%;max-width:440px;text-align:center}
.cover{
  position:fixed;inset:0;z-index:5;
  display:flex;align-items:center;justify-content:center;
  flex-direction:column;
  background:linear-gradient(135deg,#f9dce8,#fff1e7);
  transition:opacity .8s,visibility .8s;
  padding:24px
}
.cover.hide{opacity:0;visibility:hidden}
.envelope{font-size:100px;animation:bob 2s infinite ease-in-out}
.cover h1{font-size:28px;color:#a64d70}
.cover p{color:#8b6273}
button{
  border:0;padding:14px 25px;border-radius:30px;
  background:#c76a8b;color:white;font-size:16px;
  box-shadow:0 6px 20px #c76a8b40;
  cursor:pointer;transition:.2s
}
button:hover{transform:translateY(-2px)}
.card{
  background:#fffdfb;border-radius:26px;padding:28px 23px;
  box-shadow:0 20px 60px #ad6c8330;
  border:1px solid #fff;position:relative
}
.tag{font-size:12px;letter-spacing:4px;color:#c27b95}
h2{font-size:30px;color:#b65c7d;margin:14px 0}
.photo{
  width:100%;height:280px;border-radius:18px;
  background:#f6e2e9;overflow:hidden;margin:20px 0;
  display:flex;align-items:center;justify-content:center
}
.photo img{width:100%;height:100%;object-fit:cover}
.photo .placeholder{padding:20px;color:#a97589}
.message{line-height:2;font-size:16px;text-align:left}
.signature{color:#bc6785;text-align:right;margin-top:20px}
.surprise{
  display:none;margin-top:20px;padding:20px;
  background:#fff0f5;border-radius:18px;line-height:2;
  animation:fade .5s
}
.surprise.show{display:block}
.btn{margin-top:20px}
.foot{font-size:12px;color:#b18b9b;margin-top:20px}
.heart{
  position:fixed;pointer-events:none;z-index:4;
  animation:float 5s linear forwards;opacity:.7
}
@keyframes bob{50%{transform:translateY(-12px)}}
@keyframes float{
  0%{transform:translateY(0) rotate(0);opacity:0}
  10%{opacity:.8}
  100%{transform:translateY(-100vh) rotate(30deg);opacity:0}
}
@keyframes fade{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
@media(max-width:480px){
  body{padding:14px}
  .card{padding:22px 18px}
  .photo{height:260px}
}
</style>
</head>
<body>
<div class="cover" id="cover">
  <div class="envelope">💌</div>
  <h1>有一封信，想送给你</h1>
  <p>准备好了吗？</p>
  <button onclick="openLetter()">打开信件 ✨</button>
</div>

<div class="wrap">
  <div class="card">
    <div class="tag">A LETTER FOR YOU</div>
    <h2>生日快乐 🎂</h2>
    <p>愿今天的你，被温柔包围</p>

    <div class="photo" id="photo">
      <div class="placeholder">
        <div style="font-size:50px">📷</div>
        <p>未来这里放上你们的照片</p>
      </div>
    </div>

    <div class="message">
      <p>亲爱的：</p>
      <p>
        今天是属于你的日子。<br>
        愿你在新的一岁里，<br>
        有勇气追逐喜欢的生活，<br>
        有温柔拥抱每一个平凡的日子。
      </p>
      <p>
        愿所有美好如期而至，<br>
        愿你的笑容永远灿烂。
      </p>
    </div>

    <div class="signature">—— 一个想给你惊喜的人</div>

    <button class="btn" onclick="toggleSurprise()">还有一份惊喜 ✨</button>

    <div class="surprise" id="surprise">
      <h3>💗 偷偷告诉你</h3>
      <p>遇见你，是生活送给我的一份礼物。</p>
      <p>希望未来的每一天，我们都能创造更多值得珍藏的回忆。</p>
      <p style="font-size:28px">🌷💕🌷</p>
    </div>
  </div>
  <div class="foot">Made with ♥ · 一份可以珍藏的心意</div>
</div>

<script>
function openLetter(){
  document.getElementById('cover').classList.add('hide');
  createHearts();
}
function toggleSurprise(){
  document.getElementById('surprise').classList.toggle('show');
}
function createHearts(){
  setInterval(()=>{
    const h=document.createElement('div');
    h.className='heart';
    h.innerHTML=['💗','💕','🌸','✨','💖'][Math.floor(Math.random()*5)];
    h.style.left=Math.random()*100+'vw';
    h.style.bottom='-30px';
    h.style.fontSize=(16+Math.random()*20)+'px';
    document.body.appendChild(h);
    setTimeout(()=>h.remove(),5000);
  },700);
}
</script>
</body>
</html>
