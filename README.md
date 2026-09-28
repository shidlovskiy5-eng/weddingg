<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ольга & Никита — Приглашение на свадьбу</title>
<meta name="description" content="Приглашаем вас разделить с нами самый важный день — нашу свадьбу!">

<link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>💍</text></svg>">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Alex+Brush&family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
/* ============ РАСШИРЕННАЯ ПАЛИТРА ============ */
:root{
  --bg:         #FAF9F6;
  --dark-green: #2E4A35;
  --sage:       #9AA97A;
  --mint:       #A8BFA8;
  --beige:      #D9C8BA;
  --grey:       #B2B2B2;
  --rose:       #D4A5A5;
  --terracotta: #C97B5B;
  --dusty-blue: #8FA5B8;
  --lavender:   #B5A8C9;
  --mustard:    #D4A94E;
  --blush:      #F2E2DA;
  --soft-mint:  #E4EDE4;
  --soft-blue:  #E2EAF0;
  --soft-lav:   #EDE7F2;
  --soft-rose:  #F5E6E6;
  
  --text:       #2C3A2E;
  --muted:      #7A857C;
  --line:       #E2E0D9;
  
  --font-script: 'Alex Brush', cursive;
  --font-h:      'Cormorant Garamond', Georgia, serif;
  --font-b:      'Montserrat', -apple-system, sans-serif;
}

*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{
  font-family:var(--font-b);
  background:var(--bg);
  color:var(--text);
  font-size:16px;
  line-height:1.7;
  font-weight:300;
  overflow-x:hidden;
  -webkit-font-smoothing:antialiased;
}
img{max-width:100%;display:block;}
a{color:inherit;text-decoration:none;}

.wrap{max-width:760px;margin:0 auto;padding:0 24px;}
.wrap--wide{max-width:1000px;}

h1,h2,h3{font-family:var(--font-h);font-weight:400;line-height:1.15;}

.eyebrow{
  font-size:11px;letter-spacing:.32em;text-transform:uppercase;
  color:var(--sage);font-weight:500;margin-bottom:18px;
}

.section{padding:clamp(70px,11vw,130px) 0;position:relative;overflow:hidden;}
.center{text-align:center;}

.divider{
  display:flex;align-items:center;justify-content:center;
  gap:14px;margin:26px auto;
}
.divider::before,.divider::after{
  content:'';height:1px;width:60px;
  background:linear-gradient(90deg, transparent, var(--sage), transparent);
}
.divider span{
  width:7px;height:7px;border:1px solid var(--sage);
  transform:rotate(45deg);background:var(--beige);
}

/* ============ HERO С ГРАДИЕНТОМ ============ */
.hero{
  min-height:100svh;
  display:flex;flex-direction:column;
  align-items:center;justify-content:center;
  text-align:center;position:relative;
  padding:100px 24px 80px;
  background: 
    radial-gradient(circle at 15% 20%, rgba(168,191,168,.35), transparent 45%),
    radial-gradient(circle at 85% 25%, rgba(217,200,186,.45), transparent 45%),
    radial-gradient(circle at 20% 80%, rgba(143,165,184,.3), transparent 45%),
    radial-gradient(circle at 80% 85%, rgba(181,168,201,.3), transparent 45%),
    radial-gradient(circle at 50% 50%, rgba(242,226,218,.5), transparent 60%),
    linear-gradient(135deg, #FAF9F6 0%, #F0EDE5 100%);
  color:var(--dark-green);
  overflow:hidden;
}
.hero::before{
  content:'';position:absolute;inset:0;
  background-image: 
    radial-gradient(circle at 10% 15%, var(--sage) 1px, transparent 1px),
    radial-gradient(circle at 90% 30%, var(--terracotta) 1px, transparent 1px),
    radial-gradient(circle at 25% 70%, var(--dusty-blue) 1px, transparent 1px),
    radial-gradient(circle at 75% 85%, var(--lavender) 1px, transparent 1px),
    radial-gradient(circle at 50% 40%, var(--mustard) 1px, transparent 1px);
  background-size: 100% 100%;
  opacity:.5;pointer-events:none;
}
.hero::after{
  content:'';position:absolute;inset:24px;
  border:1px solid rgba(154,169,122,.4);
  border-radius:2px;pointer-events:none;
}
/* Декоративные листья/цветы вокруг */
.hero__leaf{
  position:absolute;font-size:60px;opacity:.35;pointer-events:none;
  animation:float 6s ease-in-out infinite;
}
.hero__leaf--1{top:8%;left:6%;transform:rotate(-15deg);}
.hero__leaf--2{top:12%;right:8%;transform:rotate(20deg);animation-delay:-2s;}
.hero__leaf--3{bottom:14%;left:10%;transform:rotate(35deg);animation-delay:-4s;}
.hero__leaf--4{bottom:10%;right:12%;transform:rotate(-25deg);animation-delay:-1s;}
@keyframes float{
  0%,100%{transform:translateY(0) rotate(var(--rot, 0deg));}
  50%{transform:translateY(-15px) rotate(var(--rot, 0deg));}
}

.hero__label{
  font-size:11px;letter-spacing:.42em;text-transform:uppercase;
  color:var(--terracotta);font-weight:500;margin-bottom:34px;
  position:relative;z-index:2;
}
.hero__names{
  font-family:var(--font-script);
  font-size:clamp(60px,14vw,130px);
  font-weight:400;
  letter-spacing:.02em;
  line-height:1;
  color:var(--dark-green);
  position:relative;z-index:2;
}
.hero__amp{
  display:block;
  font-family:var(--font-h);
  font-style:italic;
  font-size:.35em;
  color:var(--terracotta);
  margin:6px 0;
}
.hero__date{
  margin-top:36px;
  font-family:var(--font-h);
  font-size:clamp(22px,4.6vw,34px);
  letter-spacing:.14em;
  color:var(--sage);
  position:relative;z-index:2;
}
.hero__place{
  margin-top:10px;font-size:12px;letter-spacing:.24em;
  text-transform:uppercase;color:var(--muted);
  position:relative;z-index:2;
}
.scroll-cue{
  position:absolute;bottom:40px;left:50%;transform:translateX(-50%);
  font-size:10px;letter-spacing:.3em;text-transform:uppercase;
  color:var(--sage);display:flex;flex-direction:column;align-items:center;gap:10px;
  z-index:2;
}
.scroll-cue i{
  display:block;width:1px;height:44px;
  background:linear-gradient(var(--terracotta),transparent);
  animation:cue 2.2s ease-in-out infinite;
}
@keyframes cue{
  0%,100%{opacity:.25;transform:scaleY(.6);}
  50%{opacity:1;transform:scaleY(1);}
}

/* ============ ОБРАТНЫЙ ОТСЧЁТ ============ */
.section--countdown{
  background:linear-gradient(135deg, #F4F3EE 0%, #EDE8DC 100%);
  position:relative;
}
.countdown{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:12px;max-width:600px;margin:44px auto 0;
}
.cd-item{
  padding:24px 8px;
  border:1px solid var(--line);
  background:#fff;
  position:relative;
  overflow:hidden;
  transition:transform .3s ease;
}
.cd-item::before{
  content:'';position:absolute;top:0;left:0;right:0;height:3px;
}
.cd-item:nth-child(1)::before{background:var(--sage);}
.cd-item:nth-child(2)::before{background:var(--dusty-blue);}
.cd-item:nth-child(3)::before{background:var(--terracotta);}
.cd-item:nth-child(4)::before{background:var(--lavender);}
.cd-item:hover{transform:translateY(-4px);}
.cd-num{
  font-family:var(--font-h);font-size:clamp(30px,7vw,44px);
  color:var(--dark-green);line-height:1;
}
.cd-item:nth-child(1) .cd-num{color:var(--sage);}
.cd-item:nth-child(2) .cd-num{color:var(--dusty-blue);}
.cd-item:nth-child(3) .cd-num{color:var(--terracotta);}
.cd-item:nth-child(4) .cd-num{color:var(--lavender);}
.cd-lbl{
  font-size:9.5px;letter-spacing:.2em;text-transform:uppercase;
  color:var(--muted);margin-top:8px;
}

/* ============ ТЕКСТ ============ */
.lead{
  font-family:var(--font-h);
  font-size:clamp(20px,3.4vw,27px);
  line-height:1.55;color:var(--dark-green);font-weight:300;
}
p+p{margin-top:16px;}
.muted{color:var(--muted);font-size:14.5px;}

/* ============ КАРТОЧКИ ДЕТАЛЕЙ С ЦВЕТНЫМИ АКЦЕНТАМИ ============ */
.cards{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));
  gap:16px;margin-top:46px;
}
.card{
  padding:38px 24px;background:#fff;
  border:1px solid var(--line);text-align:center;
  transition:transform .4s ease, box-shadow .4s ease;
  position:relative;overflow:hidden;
}
.card::before{
  content:'';position:absolute;top:0;left:0;right:0;height:4px;
}
.card:nth-child(1)::before{background:linear-gradient(90deg, var(--sage), var(--mint));}
.card:nth-child(2)::before{background:linear-gradient(90deg, var(--terracotta), var(--rose));}
.card:nth-child(3)::before{background:linear-gradient(90deg, var(--dusty-blue), var(--lavender));}
.card:hover{transform:translateY(-6px);box-shadow:0 20px 45px -22px rgba(46,74,53,.25);}
.card__icon{font-size:28px;margin-bottom:16px;}
.card:nth-child(1) .card__icon{filter:hue-rotate(60deg);}
.card:nth-child(2) .card__icon{filter:hue-rotate(-30deg);}
.card__title{
  font-family:var(--font-h);font-size:23px;
  color:var(--dark-green);margin-bottom:10px;
}
.card__text{font-size:14.5px;color:var(--muted);line-height:1.75;}
.card__text strong{color:var(--text);font-weight:500;}

/* ============ ПРОГРАММА С ЦВЕТНЫМИ ТОЧКАМИ ============ */
.section--timeline{
  background:linear-gradient(180deg, #FAF9F6 0%, #F5F2EA 50%, #FAF9F6 100%);
}
.timeline{max-width:520px;margin:50px auto 0;position:relative;}
.timeline::before{
  content:'';position:absolute;left:80px;top:8px;bottom:8px;
  width:2px;
  background:linear-gradient(180deg, var(--sage), var(--dusty-blue), var(--terracotta), var(--lavender), var(--mustard));
  border-radius:2px;
}
.tl-item{
  display:grid;grid-template-columns:80px 1fr;
  gap:32px;padding:16px 0;position:relative;
}
.tl-time{
  font-family:var(--font-h);font-size:21px;
  text-align:right;padding-top:1px;
}
.tl-item:nth-child(1) .tl-time{color:var(--sage);}
.tl-item:nth-child(2) .tl-time{color:var(--dusty-blue);}
.tl-item:nth-child(3) .tl-time{color:var(--terracotta);}
.tl-item:nth-child(4) .tl-time{color:var(--lavender);}
.tl-item:nth-child(5) .tl-time{color:var(--mustard);}

.tl-body{position:relative;padding-left:0;}
.tl-body::before{
  content:'';position:absolute;left:-36px;top:11px;
  width:11px;height:11px;background:#fff;
  border-radius:50%;
}
.tl-item:nth-child(1) .tl-body::before{border:2px solid var(--sage);}
.tl-item:nth-child(2) .tl-body::before{border:2px solid var(--dusty-blue);}
.tl-item:nth-child(3) .tl-body::before{border:2px solid var(--terracotta);}
.tl-item:nth-child(4) .tl-body::before{border:2px solid var(--lavender);}
.tl-item:nth-child(5) .tl-body::before{border:2px solid var(--mustard);}
.tl-title{font-family:var(--font-h);font-size:20px;color:var(--dark-green);}
.tl-desc{font-size:13.5px;color:var(--muted);margin-top:2px;}

/* ============ ДРЕСС-КОД ============ */
.section--dresscode{
  background: linear-gradient(135deg, #F5F2EA 0%, #EDE7F2 50%, #F2E2DA 100%);
}
.dresscode-block {
  background: #fff;
  border: 1px solid var(--line);
  padding: 60px 30px;
  max-width: 800px;
  margin: 0 auto;
  text-align: center;
  position: relative;
  overflow: hidden;
}
.dresscode-block::before,
.dresscode-block::after{
  content:'';position:absolute;width:100px;height:100px;
  border-radius:50%;filter:blur(40px);opacity:.5;
}
.dresscode-block::before{background:var(--rose);top:-30px;left:-30px;}
.dresscode-block::after{background:var(--dusty-blue);bottom:-30px;right:-30px;}
.dresscode-title {
  font-family: var(--font-script);
  font-size: clamp(60px, 12vw, 100px);
  color: var(--dark-green);
  line-height: 1;
  margin-bottom: 20px;
  position:relative;z-index:1;
}
.dresscode-text {
  font-family: var(--font-h);
  font-size: clamp(18px, 3.5vw, 24px);
  color: var(--text);
  text-transform: uppercase;
  letter-spacing: 0.1em;
  line-height: 1.5;
  max-width: 600px;
  margin: 0 auto 50px;
  position:relative;z-index:1;
}
.swatches {
  display: flex;
  justify-content: center;
  gap: 20px;
  flex-wrap: wrap;
  position:relative;z-index:1;
}
.swatch {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  box-shadow: 0 10px 25px rgba(0,0,0,0.12);
  transition: transform 0.3s ease;
  position: relative;
  cursor:pointer;
}
.swatch:hover {
  transform: scale(1.15) translateY(-5px);
}
.swatch::after {
  content: attr(data-name);
  position: absolute;
  bottom: -28px;
  left: 50%;
  transform: translateX(-50%);
  font-size: 10px;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--muted);
  white-space: nowrap;
  opacity: 0;
  transition: opacity 0.3s;
}
.swatch:hover::after {
  opacity: 1;
}

/* ============ МЕНЮ С ЦВЕТНЫМИ БЛОКАМИ ============ */
.menu-grid{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:16px;margin-top:40px;text-align:left;
}
.menu-item{
  padding:28px 24px;background:#fff;
  border:1px solid var(--line);
  position:relative;overflow:hidden;
  transition:transform .3s ease;
}
.menu-item:hover{transform:translateY(-4px);}
.menu-item::before{
  content:'';position:absolute;left:0;top:0;bottom:0;width:4px;
}
.menu-item:nth-child(1)::before{background:var(--sage);}
.menu-item:nth-child(2)::before{background:var(--terracotta);}
.menu-item:nth-child(3)::before{background:var(--dusty-blue);}
.menu-item:nth-child(4)::before{background:var(--lavender);}
.menu-item__title{
  font-family:var(--font-h);font-size:20px;
  color:var(--dark-green);margin-bottom:8px;
}
.menu-item__desc{font-size:13px;color:var(--muted);line-height:1.65;}

/* ============ ПОДАРКИ ============ */
.section--gifts{
  background: linear-gradient(180deg, #FAF9F6 0%, var(--soft-mint) 100%);
  position:relative;
}
.gift-note{
  max-width:540px;margin:30px auto 0;
  font-family:var(--font-h);font-size:19px;
  font-style:italic;color:var(--dark-green);line-height:1.6;
}

/* ============ RSVP ============ */
.section--rsvp{
  background: linear-gradient(135deg, #EDE7F2 0%, #E2EAF0 50%, #F5E6E6 100%);
}
.form{
  max-width:520px;margin:44px auto 0;
  background:#fff;border:1px solid var(--line);
  padding:clamp(28px,5vw,46px);
  text-align:left;
  position:relative;overflow:hidden;
}
.form::before{
  content:'';position:absolute;top:0;left:0;right:0;height:4px;
  background:linear-gradient(90deg, var(--sage), var(--dusty-blue), var(--terracotta), var(--lavender));
}
.field{margin-bottom:24px;}
.field label{
  display:block;font-size:11px;letter-spacing:.18em;
  text-transform:uppercase;color:var(--muted);margin-bottom:10px;
}
.field input[type=text],
.field input[type=number],
.field select,
.field textarea{
  width:100%;padding:13px 14px;
  border:1px solid var(--line);background:var(--bg);
  font-family:var(--font-b);font-size:15px;font-weight:300;
  color:var(--text);border-radius:2px;
  transition:border-color .25s, box-shadow .25s;
}
.field input:focus,.field select:focus,.field textarea:focus{
  outline:none;border-color:var(--sage);
  box-shadow:0 0 0 3px rgba(154,169,122,.15);
}
.radio-row{display:flex;gap:10px;flex-wrap:wrap;}
.radio-row label{
  flex:1;min-width:180px;
  display:flex;align-items:center;gap:10px;
  padding:13px 16px;border:1px solid var(--line);
  background:var(--bg);cursor:pointer;
  font-size:14px;letter-spacing:0;text-transform:none;
  color:var(--text);margin:0;transition:.25s;
  border-radius:2px;
}
.radio-row label:hover{border-color:var(--sage);background:var(--soft-mint);}
.radio-row input{accent-color:var(--dark-green);}
.radio-row input:checked + span{font-weight:500;}

.checks{display:flex;flex-wrap:wrap;gap:8px;}
.checks label{
  display:flex;align-items:center;gap:8px;
  padding:10px 16px;border:1px solid var(--line);
  background:var(--bg);border-radius:100px;cursor:pointer;
  font-size:13.5px;letter-spacing:0;text-transform:none;
  color:var(--text);margin:0;transition:.25s;
}
.checks label:hover{border-color:var(--terracotta);background:var(--soft-rose);}
.checks input{accent-color:var(--dark-green);}

.btn{
  display:inline-flex;align-items:center;justify-content:center;gap:10px;
  padding:16px 42px;
  background:linear-gradient(135deg, var(--dark-green), var(--sage));
  color:#fff;
  border:none;
  font-family:var(--font-b);font-size:11.5px;font-weight:500;
  letter-spacing:.22em;text-transform:uppercase;
  cursor:pointer;border-radius:2px;
  transition:.3s;width:100%;
  box-shadow:0 10px 25px -10px rgba(46,74,53,.5);
}
.btn:hover{
  background:linear-gradient(135deg, var(--terracotta), var(--rose));
  box-shadow:0 15px 30px -10px rgba(201,123,91,.5);
  transform:translateY(-2px);
}

/* ============ КАРТА ============ */
.map-embed{
  margin-top:36px;border:1px solid var(--line);
  background:#fff;overflow:hidden;
  position:relative;
}
.map-embed::before{
  content:'';position:absolute;top:0;left:0;right:0;height:4px;
  background:linear-gradient(90deg, var(--sage), var(--dusty-blue), var(--lavender));
  z-index:2;
}
.map-embed iframe{width:100%;height:360px;border:0;display:block;}

/* ============ ФУТЕР ============ */
.footer{
  padding:80px 24px 60px;text-align:center;
  background:linear-gradient(135deg, var(--dark-green) 0%, #1F3425 100%);
  color:#fff;
  position:relative;overflow:hidden;
}
.footer::before{
  content:'';position:absolute;inset:0;
  background: 
    radial-gradient(circle at 20% 30%, rgba(154,169,122,.15), transparent 40%),
    radial-gradient(circle at 80% 70%, rgba(201,123,91,.15), transparent 40%);
  pointer-events:none;
}
.footer__names{
  font-family:var(--font-script);font-size:clamp(50px,10vw,80px);
  font-weight:400;letter-spacing:.03em;line-height:1;
  position:relative;z-index:1;
}
.footer__names em{font-family:var(--font-h);font-style:italic;color:var(--beige);font-size:.5em;}
.footer__date{
  margin-top:16px;font-size:11px;letter-spacing:.34em;
  text-transform:uppercase;color:rgba(255,255,255,.55);
  position:relative;z-index:1;
}
.footer__note{
  margin-top:30px;font-family:var(--font-h);font-style:italic;
  font-size:17px;color:rgba(255,255,255,.75);
  position:relative;z-index:1;
}

/* ============ АНИМАЦИЯ ============ */
.reveal{opacity:0;transform:translateY(26px);transition:opacity .9s ease, transform .9s ease;}
.reveal.visible{opacity:1;transform:none;}

@media (max-width:520px){
  .timeline::before{left:58px;}
  .tl-item{grid-template-columns:58px 1fr;gap:24px;}
  .tl-body::before{left:-28px;}
  .tl-time{font-size:18px;}
  .hero::after{inset:12px;}
  .swatch { width: 60px; height: 60px; }
  .hero__leaf{font-size:40px;opacity:.25;}
}
</style>
</head>
<body>

<!-- ==================== СТАРТОВЫЙ ЭКРАН ==================== -->
<header class="hero">
  <div class="hero__leaf hero__leaf--1">🌿</div>
  <div class="hero__leaf hero__leaf--2">🌸</div>
  <div class="hero__leaf hero__leaf--3">🌾</div>
  <div class="hero__leaf hero__leaf--4">🍃</div>

  <div class="hero__label">Мы женимся</div>

  <h1 class="hero__names">
    Ольга
    <span class="hero__amp">&</span>
    Никита
  </h1>

  <div class="divider"><span></span></div>

  <div class="hero__date">12 . 08 . 2027</div>
  <div class="hero__place">Москва</div>

  <div class="scroll-cue">
    Листайте
    <i></i>
  </div>
</header>

<!-- ==================== ПРИГЛАШЕНИЕ ==================== -->
<section class="section">
  <div class="wrap center reveal">
    <div class="eyebrow">Дорогие друзья и близкие</div>
    <p class="lead">
      В нашей жизни скоро случится самое тёплое и важное событие —
      мы станем семьёй.
    </p>
    <div class="divider"><span></span></div>
    <p class="lead">
      И нам очень хочется, чтобы в этот день рядом были самые дорогие люди.
      Приглашаем вас разделить с нами радость нашей свадьбы.
    </p>
  </div>
</section>

<!-- ==================== ОБРАТНЫЙ ОТСЧЁТ ==================== -->
<section class="section section--countdown">
  <div class="wrap center reveal">
    <div class="eyebrow">До нашего праздника осталось</div>
    <div class="countdown" id="countdown">
      <div class="cd-item"><div class="cd-num" id="cd-d">—</div><div class="cd-lbl">дней</div></div>
      <div class="cd-item"><div class="cd-num" id="cd-h">—</div><div class="cd-lbl">часов</div></div>
      <div class="cd-item"><div class="cd-num" id="cd-m">—</div><div class="cd-lbl">минут</div></div>
      <div class="cd-item"><div class="cd-num" id="cd-s">—</div><div class="cd-lbl">секунд</div></div>
    </div>
  </div>
</section>

<!-- ==================== ДЕТАЛИ ==================== -->
<section class="section">
  <div class="wrap wrap--wide center reveal">
    <div class="eyebrow">Детали</div>
    <h2 style="font-size:clamp(32px,6vw,48px);color:var(--dark-green);">Когда и где</h2>

    <div class="cards">
      <div class="card">
        <div class="card__icon">📅</div>
        <div class="card__title">Дата</div>
        <div class="card__text">
          <strong>12 августа 2027</strong><br>четверг
        </div>
      </div>

      <div class="card">
        <div class="card__icon">🕓</div>
        <div class="card__title">Сбор гостей</div>
        <div class="card__text">
          <strong>14:00</strong><br>просим не опаздывать
        </div>
      </div>

      <div class="card">
        <div class="card__icon">📍</div>
        <div class="card__title">Место</div>
        <div class="card__text">
          <strong>Загородный клуб «Сосны»</strong><br>
          Московская обл., д. Сосновка, ул. Лесная, 1
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== ПРОГРАММА ==================== -->
<section class="section section--timeline">
  <div class="wrap center reveal">
    <div class="eyebrow">Программа дня</div>
    <h2 style="font-size:clamp(32px,6vw,48px);color:var(--dark-green);">Как пройдёт наш день</h2>

    <div class="timeline" style="text-align:left;">
      <div class="tl-item">
        <div class="tl-time">14:00</div>
        <div class="tl-body">
          <div class="tl-title">Сбор гостей</div>
          <div class="tl-desc">Добро пожаловать! Приветственные напитки и лёгкие закуски</div>
        </div>
      </div>
      <div class="tl-item">
        <div class="tl-time">15:00</div>
        <div class="tl-body">
          <div class="tl-title">Церемония</div>
          <div class="tl-desc">Самый волнительный момент — мы скажем друг другу «Да»</div>
        </div>
      </div>
      <div class="tl-item">
        <div class="tl-time">16:00</div>
        <div class="tl-body">
          <div class="tl-title">Фуршет и фотосессия</div>
          <div class="tl-desc">Поздравления, объятия и общие кадры на память</div>
        </div>
      </div>
      <div class="tl-item">
        <div class="tl-time">17:30</div>
        <div class="tl-body">
          <div class="tl-title">Банкет</div>
          <div class="tl-desc">Ужин, тосты, музыка и танцы до самого утра</div>
        </div>
      </div>
      <div class="tl-item">
        <div class="tl-time">22:00</div>
        <div class="tl-body">
          <div class="tl-title">Торт и финал вечера</div>
          <div class="tl-desc">Сладкое завершение и праздничный салют</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== ДРЕСС-КОД ==================== -->
<section class="section section--dresscode">
  <div class="wrap center reveal">
    <div class="dresscode-block">
      <div class="dresscode-title">Dress code</div>
      <div class="dresscode-text">
        Нам будет очень приятно,<br>
        если ваш наряд будет<br>
        соответствовать цветовой гамме<br>
        нашей свадьбы
      </div>
      
      <div class="swatches">
        <div class="swatch" style="background:#2E4A35" data-name="Тёмно-зелёный"></div>
        <div class="swatch" style="background:#9AA97A" data-name="Шалфей"></div>
        <div class="swatch" style="background:#A8BFA8" data-name="Мята"></div>
        <div class="swatch" style="background:#D9C8BA" data-name="Беж"></div>
        <div class="swatch" style="background:#B2B2B2" data-name="Серый"></div>
        <div class="swatch" style="background:#D4A5A5" data-name="Роза"></div>
        <div class="swatch" style="background:#8FA5B8" data-name="Пыльно-синий"></div>
        <div class="swatch" style="background:#B5A8C9" data-name="Лаванда"></div>
        <div class="swatch" style="background:#D4A94E" data-name="Горчица"></div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== МЕНЮ ==================== -->
<section class="section">
  <div class="wrap wrap--wide center reveal">
    <div class="eyebrow">Меню</div>
    <h2 style="font-size:clamp(32px,6vw,48px);color:var(--dark-green);">Что будет на столе</h2>
    <p class="muted" style="max-width:520px;margin:22px auto 0;">
      Меню разнообразно, поэтому сообщите нам заранее, если у вас есть
      предпочтения или диетические ограничения.
    </p>

    <div class="menu-grid">
      <div class="menu-item">
        <div class="menu-item__title">Холодные закуски</div>
        <div class="menu-item__desc">Сырная тарелка, мясные деликатесы, овощные нарезки, тарталетки</div>
      </div>
      <div class="menu-item">
        <div class="menu-item__title">Горячее</div>
        <div class="menu-item__desc">Мясные и рыбные блюда, вегетарианские опции по запросу</div>
      </div>
      <div class="menu-item">
        <div class="menu-item__title">Напитки</div>
        <div class="menu-item__desc">Вино красное и белое, шампанское, крепкий алкоголь, безалкогольные</div>
      </div>
      <div class="menu-item">
        <div class="menu-item__title">Десерты</div>
        <div class="menu-item__desc">Свадебный торт, фрукты, мороженое, кофе и чай</div>
      </div>
    </div>
  </div>
</section>

<!-- ==================== ПОДАРКИ ==================== -->
<section class="section section--gifts">
  <div class="wrap center reveal">
    <div class="eyebrow">Пожелания по подаркам</div>
    <h2 style="font-size:clamp(32px,6vw,48px);color:var(--dark-green);">Что нам подарить</h2>

    <p class="gift-note">
      Ваше присутствие в день нашей свадьбы — самый значимый подарок для нас!
      Мы понимаем, что дарить цветы — это традиция, но мы не сможем
      насладиться их красотой в полной мере.
      Будем рады любой другой альтернативе.
    </p>
  </div>
</section>

<!-- ==================== RSVP ==================== -->
<section class="section section--rsvp" id="rsvp">
  <div class="wrap center reveal">
    <div class="eyebrow">Подтверждение</div>
    <h2 style="font-size:clamp(32px,6vw,48px);color:var(--dark-green);">
      Будете с нами?
    </h2>
    <p class="muted" style="max-width:480px;margin:20px auto 0;">
      Пожалуйста, ответьте до <strong>1 июля 2027</strong> — так мы сможем
      всё предусмотреть и позаботиться о каждом госте.
    </p>

    <form class="form" id="rsvpForm">
      <div class="field">
        <label for="name">Ваше имя и фамилия</label>
        <input type="text" id="name" placeholder="Иван Иванов" required>
      </div>

      <div class="field">
        <label>Сможете прийти?</label>
        <div class="radio-row">
          <label>
            <input type="radio" name="attend" value="Да, обязательно буду" checked>
            <span>Да, обязательно буду</span>
          </label>
          <label>
            <input type="radio" name="attend" value="К сожалению, не смогу">
            <span>К сожалению, не смогу</span>
          </label>
        </div>
      </div>

      <div class="field">
        <label for="guests">Сколько вас будет (включая вас)</label>
        <input type="number" id="guests" min="1" max="6" value="1">
      </div>

      <div class="field">
        <label>Предпочтения по напиткам</label>
        <div class="checks">
          <label><input type="checkbox" value="Вино красное"> Вино красное</label>
          <label><input type="checkbox" value="Вино белое"> Вино белое</label>
          <label><input type="checkbox" value="Шампанское"> Шампанское</label>
          <label><input type="checkbox" value="Крепкий алкоголь"> Крепкий алкоголь</label>
          <label><input type="checkbox" value="Безалкогольные"> Безалкогольные</label>
        </div>
      </div>

      <div class="field">
        <label for="wishes">Пожелания и комментарии</label>
        <textarea id="wishes" rows="3" placeholder="Аллергии, особенности питания, пожелания..."></textarea>
      </div>

      <button type="submit" class="btn">Отправить ответ</button>

      <p class="muted center" style="margin-top:20px;font-size:12.5px;">
        Или напишите нам напрямую:
        <a href="tel:+79999999999" style="color:var(--dark-green);border-bottom:1px solid var(--line);">+7 999 999-99-99</a>
      </p>
    </form>
  </div>
</section>

<!-- ==================== КАРТА ==================== -->
<section class="section">
  <div class="wrap wrap--wide center reveal">
    <div class="eyebrow">Как добраться</div>
    <h2 style="font-size:clamp(32px,6vw,48px);color:var(--dark-green);">Мы ждём вас здесь</h2>

    <div class="map-embed">
      <iframe
        src="https://yandex.ru/map-widget/v1/?ll=37.617635%2C55.755814&z=12"
        loading="lazy"
        allowfullscreen>
      </iframe>
    </div>

    <p class="muted" style="margin-top:18px;">
      Для точного маршрута откройте карту в приложении или напишите нам — подскажем.
    </p>
  </div>
</section>

<!-- ==================== ФУТЕР ==================== -->
<footer class="footer">
  <div class="footer__names">Ольга <em>&</em> Никита</div>
  <div class="footer__date">12 августа 2027 · Москва</div>
  <div class="footer__note">Будем счастливы видеть вас в этот особенный день!</div>
</footer>

<script>
const CONFIG = {
  weddingDate: new Date(2027, 7, 12, 14, 0, 0),
  whatsapp: '79999999999'
};

/* ---------- Обратный отсчёт ---------- */
(function(){
  const d = document.getElementById('cd-d'),
        h = document.getElementById('cd-h'),
        m = document.getElementById('cd-m'),
        s = document.getElementById('cd-s');
  const pad = n => String(n).padStart(2, '0');

  function tick(){
    const diff = CONFIG.weddingDate - new Date();
    if (diff <= 0){
      document.getElementById('countdown').innerHTML =
        '<div style="grid-column:1/-1;font-family:var(--font-h);font-size:32px;color:var(--dark-green);">Этот день наступил! 🎉</div>';
      return;
    }
    d.textContent = Math.floor(diff / 86400000);
    h.textContent = pad(Math.floor(diff / 3600000) % 24);
    m.textContent = pad(Math.floor(diff / 60000) % 60);
    s.textContent = pad(Math.floor(diff / 1000) % 60);
  }
  tick();
  setInterval(tick, 1000);
})();

/* ---------- Появление блоков ---------- */
(function(){
  const els = document.querySelectorAll('.reveal');
  if (!('IntersectionObserver' in window)){
    els.forEach(el => el.classList.add('visible'));
    return;
  }
  const io = new IntersectionObserver((entries) => {
    entries.forEach(e => {
      if (e.isIntersecting){
        e.target.classList.add('visible');
        io.unobserve(e.target);
      }
    });
  }, { threshold: 0.12, rootMargin: '0px 0px -60px 0px' });
  els.forEach(el => io.observe(el));
})();

/* ---------- Форма RSVP → WhatsApp ---------- */
document.getElementById('rsvpForm').addEventListener('submit', function(e){
  e.preventDefault();
  const name    = document.getElementById('name').value.trim();
  const attend  = document.querySelector('input[name="attend"]:checked').value;
  const guests  = document.getElementById('guests').value;
  const drinks  = [...document.querySelectorAll('.checks input:checked')]
                    .map(i => i.value).join(', ') || '—';
  const wishes  = document.getElementById('wishes').value.trim() || '—';

  const text =
    `Свадьба Ольги и Никиты 💍\n\n` +
    `Имя: ${name}\n` +
    `Присутствие: ${attend}\n` +
    `Гостей: ${guests}\n` +
    `Напитки: ${drinks}\n` +
    `Комментарий: ${wishes}`;

  const url = `https://wa.me/${CONFIG.whatsapp}?text=${encodeURIComponent(text)}`;
  window.open(url, '_blank');
});
</script>

</body>
</html>
