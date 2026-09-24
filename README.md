<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Fahim Sariyar | CSE Student & Problem Solver</title>
<meta name="description" content="CSE undergraduate at BUBT. C, C++, Java, DSA and OOP projects.">
<style>
:root{--bg:#070b18;--ink:#eaf0ff;--mute:#9aa8d0;--cyan:#3ddcff;--amber:#ffb547;--line:#26335f;--card:#101a3acc}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;background:var(--bg);color:var(--ink);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;overflow-x:hidden}
#bgVideo{position:fixed;inset:0;width:100%;height:100%;object-fit:cover;opacity:.3;z-index:0}
.shade{position:fixed;inset:0;background:linear-gradient(180deg,#070b18cc,#070b18f2);z-index:1}
#model{position:fixed;inset:0;width:100%;height:100%;z-index:2;pointer-events:none}
nav{position:fixed;top:0;left:0;right:0;z-index:5;display:flex;justify-content:space-between;align-items:center;padding:14px 24px;background:#070b18cc;backdrop-filter:blur(10px);border-bottom:1px solid var(--line)}
nav b{font-size:17px}
nav div{display:flex;gap:18px;flex-wrap:wrap}
nav a{color:var(--mute);text-decoration:none;font-size:14px}
nav a:hover{color:var(--cyan)}
main{position:relative;z-index:3;max-width:1040px;margin:0 auto;padding:0 20px}
section{padding:70px 0 10px}
.hero{min-height:100vh;display:flex;align-items:center;gap:40px;padding-top:90px;flex-wrap:wrap}
.photo{width:230px;height:290px;border-radius:26px;border:2px solid var(--cyan);overflow:hidden;background:linear-gradient(135deg,#1c2a5a,#0d1633);box-shadow:0 30px 60px -20px #3ddcff55;transform:perspective(800px) rotateY(-10deg);transition:transform .3s;flex:none;display:grid;place-items:center}
.photo:hover{transform:perspective(800px) rotateY(0) scale(1.03)}
.photo img{width:100%;height:100%;object-fit:cover;display:block}
.photo span{font-size:64px;font-weight:800;color:var(--cyan)}
.intro{max-width:520px}
h1{font-size:clamp(38px,7vw,68px);line-height:1;margin:0 0 14px;letter-spacing:-.03em}
.role{color:var(--amber);font-weight:700;margin:0 0 12px}
.sub{color:var(--mute);font-size:17px;line-height:1.65;margin:0 0 26px}
.btns{display:flex;gap:12px;flex-wrap:wrap}
.btn{padding:13px 22px;border-radius:12px;font-weight:700;text-decoration:none;font-size:15px}
.p{background:var(--cyan);color:#04101f}
.g{border:1px solid var(--line);color:var(--ink);background:#101a3a99;backdrop-filter:blur(8px)}
h2{font-size:28px;margin:0 0 20px}
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:14px}
.stat,.card{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:18px;backdrop-filter:blur(8px)}
.stat b{display:block;font-size:36px;color:var(--cyan)}
.stat span{color:var(--mute);font-size:14px}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:16px}
.card h3{margin:0 0 8px;font-size:18px}
.card p{margin:0 0 12px;color:var(--mute);line-height:1.6;font-size:15px}
.card a{color:inherit;text-decoration:none}
.tag{display:inline-block;font-size:12px;padding:4px 10px;border-radius:99px;border:1px solid var(--line);color:var(--cyan);margin-right:6px}
.bar{height:9px;border-radius:9px;background:#22306099;overflow:hidden;margin:6px 0 14px}
.bar i{display:block;height:100%;width:0;background:linear-gradient(90deg,var(--cyan),#5b6cff);transition:width 1.2s}
.lbl{display:flex;justify-content:space-between;font-size:14px;color:var(--mute)}
.lbl em{font-style:normal;color:var(--ink)}
.two{display:grid;grid-template-columns:1fr 1fr;gap:20px}
@media(max-width:760px){.two{grid-template-columns:1fr}.photo{width:180px;height:230px}}
.tl{border-left:2px solid var(--line);padding-left:22px;margin-left:6px}
.tl div{position:relative;margin-bottom:22px}
.tl div:before{content:"";position:absolute;left:-29px;top:5px;width:12px;height:12px;border-radius:50%;background:var(--cyan)}
.tl b{display:block}
.tl small{color:var(--mute);line-height:1.6}
.note{color:var(--mute);font-size:13px;margin-top:10px}
footer{position:relative;z-index:3;text-align:center;color:var(--mute);font-size:13px;padding:50px 20px}
a:focus-visible{outline:2px solid var(--amber);outline-offset:3px}
</style>
</head>
<body>
<!-- Optional: put hero.mp4 next to this file for a video background -->
<video id="bgVideo" autoplay muted loop playsinline preload="metadata"><source src="hero.mp4" type="video/mp4"></video>
<div class="shade"></div>
<canvas id="model" aria-hidden="true"></canvas>

<nav>
  <b>Fahim Sariyar</b>
  <div><a href="#about">About</a><a href="#skills">Skills</a><a href="#projects">Projects</a><a href="#journey">Journey</a><a href="#contact">Contact</a></div>
</nav>

<main>
  <header class="hero">
    <!-- YOUR PHOTO: save it as photo.jpg next to this file -->
    <div class="photo"><img src="photo.jpg" alt="Portrait of Fahim Sariyar" onerror="this.remove();this.parentNode.innerHTML='<span>FS</span>'"></div>
    <div class="intro">
      <p class="role">CSE Undergraduate | BUBT</p>
      <h1>Fahim Sariyar</h1>
      <p class="sub">I solve problems with C, C++ and Java, and build object-oriented systems. Currently sharpening data structures, algorithms and competitive programming.</p>
      <div class="btns">
        <a class="btn p" href="https://github.com/fahim-sariyar">View GitHub</a>
        <a class="btn g" href="#contact">Hire or collaborate</a>
      </div>
    </div>
  </header>

  <section id="stats">
    <h2>Numbers</h2>
    <div class="stats">
      <div class="stat"><b data-n="517">0</b><span>Total contributions</span></div>
      <div class="stat"><b data-n="306">0</b><span>Contributions in 2026</span></div>
      <div class="stat"><b data-n="15">0</b><span>Longest streak (days)</span></div>
      <div class="stat"><b id="repos">-</b><span>Public repositories (live)</span></div>
      <div class="stat"><b id="followers">-</b><span>Followers (live)</span></div>
    </div>
    <p class="note">Contribution numbers are from my profile snapshot. Repository and follower counts load live from the GitHub API.</p>
  </section>

  <section id="about" class="two">
    <div>
      <h2>About</h2>
      <p class="sub">Computer Science and Engineering student at Bangladesh University of Business and Technology. I like turning a problem statement into clean, testable code, and I practice daily on Codeforces and HackerRank.</p>
      <span class="tag">DSA</span><span class="tag">OOP</span><span class="tag">C / C++</span><span class="tag">Java</span><span class="tag">Python</span>
    </div>
    <div class="card">
      <h3>What I am looking for</h3>
      <p>Internships, open-source collaboration and competitive programming teams.</p>
      <h3>Currently</h3>
      <p>Learning DSA, building console projects, solving Codeforces problems.</p>
    </div>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <div class="two">
      <div class="card"><h3>Languages on my repos (live)</h3><div id="langs"><p>Loading from GitHub...</p></div></div>
      <div class="card"><h3>Focus (self-rated)</h3>
        <div class="lbl"><span>Problem solving</span><em>80%</em></div><div class="bar"><i data-w="80"></i></div>
        <div class="lbl"><span>Data structures and algorithms</span><em>60%</em></div><div class="bar"><i data-w="60"></i></div>
        <div class="lbl"><span>OOP and software design</span><em>65%</em></div><div class="bar"><i data-w="65"></i></div>
        <div class="lbl"><span>Web development</span><em>35%</em></div><div class="bar"><i data-w="35"></i></div>
      </div>
    </div>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="grid" id="projGrid">
      <article class="card"><h3><a href="https://github.com/fahim-sariyar/Bank-Management-System">Bank-Management-System</a></h3><p>Console app for accounts, deposits and withdrawals, built on OOP.</p><span class="tag">C++</span></article>
      <article class="card"><h3>Data-Structure</h3><p>Core data structures implemented from scratch.</p><span class="tag">C / C++</span></article>
      <article class="card"><h3>Codeforces solutions</h3><p>Problem-set solutions and practice notes.</p><span class="tag">Problem solving</span></article>
    </div>
  </section>

  <section id="journey">
    <h2>Journey</h2>
    <div class="tl">
      <div><b>B.Sc. in CSE, BUBT</b><small>Ongoing. Core focus: data structures, algorithms, OOP.</small></div>
      <div><b>Competitive programming</b><small>Active on Codeforces. Practicing on HackerRank in C and C++.</small></div>
      <div><b>Bank-Management-System</b><small>First full console project using C++ and OOP concepts.</small></div>
      <div><b>Longest streak: 15 days</b><small>Next target: a 30-day commit streak.</small></div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <div class="grid">
      <a class="card" href="mailto:fahim.k4.it@gmail.com"><h3>Email</h3><p>fahim.k4.it@gmail.com</p></a>
      <a class="card" href="https://github.com/fahim-sariyar"><h3>GitHub</h3><p>github.com/fahim-sariyar</p></a>
    </div>
  </section>
</main>
<footer>Built by Fahim Sariyar. Numbers are real, updated from GitHub.</footer>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
(function(){
  var U='fahim-sariyar';
  var vid=document.getElementById('bgVideo');
  vid.querySelector('source').addEventListener('error',function(){vid.style.display='none'});

  document.querySelectorAll('[data-n]').forEach(function(el){
    var t=+el.dataset.n,s=performance.now();
    (function f(n){var p=Math.min((n-s)/1200,1);el.textContent=Math.round(t*p);if(p<1)requestAnimationFrame(f)})(s);
  });
  setTimeout(function(){document.querySelectorAll('[data-w]').forEach(function(i){i.style.width=i.dataset.w+'%'})},300);

  // Live GitHub data with safe fallbacks
  fetch('https://api.github.com/users/'+U).then(function(r){return r.json()}).then(function(d){
    document.getElementById('repos').textContent=d.public_repos;
    document.getElementById('followers').textContent=d.followers;
  }).catch(function(){});
  fetch('https://api.github.com/users/'+U+'/repos?per_page=100&sort=updated').then(function(r){return r.json()}).then(function(list){
    if(!Array.isArray(list)||!list.length)return;
    var c={},tot=0;
    list.forEach(function(x){if(x.language){c[x.language]=(c[x.language]||0)+1;tot++}});
    var h='';Object.keys(c).sort(function(a,b){return c[b]-c[a]}).slice(0,5).forEach(function(k){
      var p=Math.round(c[k]/tot*100);
      h+='<div class="lbl"><span>'+k+'</span><em>'+c[k]+' repos ('+p+'%)</em></div><div class="bar"><i style="width:'+p+'%"></i></div>';
    });
    if(h)document.getElementById('langs').innerHTML=h;
    var top=list.filter(function(x){return !x.fork}).slice(0,6),g=document.getElementById('projGrid'),o='';
    top.forEach(function(x){
      var n=x.name.replace(/</g,''),d=(x.description||'').replace(/</g,'');
      o+='<article class="card"><h3><a href="'+x.html_url+'">'+n+'</a></h3><p>'+(d||'Repository on GitHub.')+'</p>'+(x.language?'<span class="tag">'+x.language+'</span>':'')+'<span class="tag">Stars '+x.stargazers_count+'</span></article>';
    });
    if(o)g.innerHTML=o;
  }).catch(function(){
    var l=document.getElementById('langs');l.innerHTML='<p>Could not load live data. Open the page online to see it.</p>';
  });

  if(!window.THREE)return;
  var reduce=matchMedia('(prefers-reduced-motion: reduce)').matches;
  var r=new THREE.WebGLRenderer({canvas:document.getElementById('model'),alpha:true,antialias:true});
  r.setPixelRatio(Math.min(devicePixelRatio,2));
  var scene=new THREE.Scene(),cam=new THREE.PerspectiveCamera(50,1,.1,100);cam.position.z=7;
  var g=new THREE.Group();scene.add(g);
  g.add(new THREE.Mesh(new THREE.IcosahedronGeometry(2.2,1),new THREE.MeshBasicMaterial({color:0x3ddcff,wireframe:true,transparent:true,opacity:.4})),
        new THREE.Mesh(new THREE.TorusKnotGeometry(.9,.28,120,16),new THREE.MeshNormalMaterial()));
  var pts=new Float32Array(900);for(var i=0;i<pts.length;i++)pts[i]=(Math.random()-.5)*16;
  var pg=new THREE.BufferGeometry();pg.setAttribute('position',new THREE.BufferAttribute(pts,3));
  var dust=new THREE.Points(pg,new THREE.PointsMaterial({color:0xffb547,size:.04}));scene.add(dust);
  var mx=0,my=0;
  addEventListener('pointermove',function(e){mx=e.clientX/innerWidth-.5;my=e.clientY/innerHeight-.5});
  function size(){var w=innerWidth,h=innerHeight;r.setSize(w,h,false);cam.aspect=w/h;cam.updateProjectionMatrix();g.position.x=w>900?3.4:0;g.position.y=w>900?0:3;g.scale.setScalar(w>900?1:.5)}
  addEventListener('resize',size);size();
  (function loop(){
    if(!reduce){g.rotation.y+=.006;g.rotation.x+=.003;dust.rotation.y+=.0008}
    g.rotation.y+=mx*.01;cam.position.y+=(-my*1.2-cam.position.y)*.05;cam.lookAt(0,0,0);
    r.render(scene,cam);requestAnimationFrame(loop);
  })();
})();
</script>
</body>
</html>
