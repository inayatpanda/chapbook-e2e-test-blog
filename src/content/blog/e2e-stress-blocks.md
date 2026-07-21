---
title: "e2e-stress-blocks"
description: "An end-to-end stress test post exercising every Chapbook block type."
date: 2026-07-21
tags: ["atlas"]
accent: "#2dd4bf"
template: "parchment"
theme: "parchment"
---

This is the **e2e stress** test post exercising _every_ block. It has [a link](https://example.com) and inline `code` plus an ampersand & a < angle to test escaping.

## A Stress-Test Heading

<figure><img src="/images/posts/e2e-stress-blocks/b3.jpg" alt="A solid red test square" loading="lazy"></figure>

> Plain text outlives every format & framework.
> — \<b\>Ada\</b\> Lovelace & Babbage \<script\>alert\(1\)\</script\>

![](./_images/e2e-stress-blocks/gallery-1.jpg)
![](./_images/e2e-stress-blocks/gallery-2.jpg)

<div class="embed-16x9">
  <iframe src="https://www.youtube-nocookie.com/embed/dQw4w9WgXcQ" title="A classic embedded video for the e2e test" loading="lazy" allowfullscreen></iframe>
</div>

| Format | Longevity |
| --- | --- |
| Plain text | Forever &amp; ever |

<div class="playground">
<button id="btn">Count: 0</button>
</div>

<script type="application/pg">
let n=0; const b=document.getElementById("btn"); b.onclick=()=>{n++; b.textContent="Count: "+n;};
</script>

<div class="playground" id="pg-gradient-maker-hl4b10">
<div class="pg-frame"><div class="pg-frame-head"><div class="pg-frame-title">Aurora</div></div><div class="pg-frame-body"><div class="pg-stage"><div class="pg-gm-title">Aurora</div><div class="pg-gm-preview" data-role="preview"></div><div class="pg-gm-swatches"><span class="pg-gm-swatch" style="background:#2dd4bf" title="#2dd4bf"></span><span class="pg-gm-swatch" style="background:#22d3ee" title="#22d3ee"></span><span class="pg-gm-swatch" style="background:#818cf8" title="#818cf8"></span></div><div class="pg-controls"><div class="pg-row"><label><b>Angle</b> <span class="pg-readout" data-role="angle-out">100°</span></label><input type="range" data-role="angle" min="0" max="360" step="1" value="100"></div></div><div class="pg-gm-code"><code data-role="code"></code><button type="button" class="pg-gm-copy" data-role="copy">Copy</button></div></div></div></div>
</div>

<style>
#pg-gradient-maker-hl4b10 .pg-frame-head{margin:0 0 .8rem}
#pg-gradient-maker-hl4b10 .pg-frame-title{font:650 1.12rem/1.25 var(--font-display,system-ui);color:#fff;letter-spacing:-.01em}
#pg-gradient-maker-hl4b10 .pg-frame-sub{margin-top:.15rem;font-size:.86rem;color:var(--ink-dim,#9fb3c8)}
#pg-gradient-maker-hl4b10 .pg-frame-cap{margin-top:.85rem;font-size:.8rem;color:var(--ink-faint,#717d99);line-height:1.5}
#pg-gradient-maker-hl4b10 .pg-gm-title{font-weight:700;font-size:1.05rem;margin-bottom:.6rem;color:var(--ink,#e9eef8)}
#pg-gradient-maker-hl4b10 .pg-gm-preview{height:170px;border-radius:14px;border:1px solid var(--line,#23304a)}
#pg-gradient-maker-hl4b10 .pg-gm-swatches{display:flex;gap:.4rem;margin:.6rem 0 .2rem}
#pg-gradient-maker-hl4b10 .pg-gm-swatch{width:26px;height:26px;border-radius:7px;border:1px solid rgba(255,255,255,.15)}
#pg-gradient-maker-hl4b10 .pg-controls{margin:.7rem 0 .6rem}
#pg-gradient-maker-hl4b10 .pg-row label{display:flex;align-items:center;gap:.5rem;color:var(--ink-dim,#cdd6e6);font-size:.9rem}
#pg-gradient-maker-hl4b10 .pg-readout{color:#22d3ee;font-variant-numeric:tabular-nums;font-weight:600}
#pg-gradient-maker-hl4b10 input[type=range]{width:100%;accent-color:#22d3ee;margin-top:.35rem}
#pg-gradient-maker-hl4b10 .pg-gm-code{display:flex;align-items:center;gap:.6rem;background:rgba(140,160,200,.06);border:1px solid var(--line,#23304a);border-radius:10px;padding:.55rem .7rem}
#pg-gradient-maker-hl4b10 .pg-gm-code code{flex:1;min-width:0;overflow-x:auto;white-space:nowrap;font-family:ui-monospace,SFMono-Regular,Menlo,monospace;font-size:.82rem;color:var(--ink,#e9eef8)}
#pg-gradient-maker-hl4b10 .pg-gm-copy{flex:none;border:1px solid #2dd4bf66;background:rgba(45,212,191,.12);color:#2dd4bf;border-radius:8px;padding:.4rem .8rem;cursor:pointer;font:inherit;font-weight:600}
#pg-gradient-maker-hl4b10 .pg-gm-copy:hover{background:rgba(45,212,191,.2)}
#pg-gradient-maker-hl4b10 .pg-gm-copy.copied{color:#fbbf24;border-color:#fbbf2466;background:rgba(251,191,36,.12)}
#pg-gradient-maker-hl4b10 .pg-gm-caption{margin-top:.6rem;color:var(--ink-dim,#cdd6e6);font-size:.85rem}
</style>

<script type="application/pg">
(function(){
var CONFIG={"domId":"pg-gradient-maker-hl4b10","title":"Aurora","stops":["#2dd4bf","#22d3ee","#818cf8"],"angle":100,"caption":"","subtitle":"","accent":"default","accentCustom":"","maxHeight":"auto"};
var root=document.getElementById("pg-gradient-maker-hl4b10");
if(!root)return;
var reduced=window.matchMedia&&window.matchMedia('(prefers-reduced-motion: reduce)').matches;
var $=function(s){return root.querySelector(s);};
var $$=function(s){return Array.prototype.slice.call(root.querySelectorAll(s));};

var stops=["#2dd4bf","#22d3ee","#818cf8"];
var preview=$('[data-role=preview]'), code=$('[data-role=code]');
var slider=$('[data-role=angle]'), out=$('[data-role=angle-out]'), copy=$('[data-role=copy]');
if(!preview||!code||!slider)return;
function gradient(deg){return 'linear-gradient('+deg+'deg, '+stops.join(', ')+')';}
function render(){
  var deg=parseInt(slider.value,10)||0;
  var g=gradient(deg);
  preview.style.background=g;
  code.textContent='background: '+g+';';
  if(out)out.textContent=deg+'\u00B0';
}
slider.addEventListener('input',render);
if(copy){
  copy.addEventListener('click',function(){
    var text=code.textContent;
    function done(){copy.classList.add('copied');copy.textContent='Copied';setTimeout(function(){copy.classList.remove('copied');copy.textContent='Copy';},1400);}
    if(navigator.clipboard&&navigator.clipboard.writeText){navigator.clipboard.writeText(text).then(done,done);}
    else{done();}
  });
}
render();
})();
</script>

<figure class="fig fig--default" data-draw><svg viewBox="0 0 360 360" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" role="img" fill="none"><style>@keyframes fig-draw { to { stroke-dashoffset:0 } }
.fig-stroke { stroke-dasharray:1000; stroke-dashoffset:1000; animation:fig-draw 1.6s ease forwards }
@media (prefers-reduced-motion: reduce) { .fig-stroke { animation:none; stroke-dashoffset:0 } }</style><path d="M 203.81 72.61 Q 276.17 83.83 286.35 151.91" fill="none" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><g><line x1="286.35" y1="151.91" x2="287.39" y2="156.19" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><polyline points="281.33,149.53 287.39,156.19 289.72,147.5" fill="none" stroke="var(--ink)" stroke-width="2"/></g><path d="M 287.39 203.81 Q 276.17 276.17 208.09 286.35" fill="none" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><g><line x1="208.09" y1="286.35" x2="203.81" y2="287.39" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><polyline points="210.47,281.33 203.81,287.39 212.5,289.72" fill="none" stroke="var(--ink)" stroke-width="2"/></g><path d="M 156.19 287.39 Q 83.83 276.17 73.65 208.09" fill="none" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><g><line x1="73.65" y1="208.09" x2="72.61" y2="203.81" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><polyline points="78.67,210.47 72.61,203.81 70.28,212.5" fill="none" stroke="var(--ink)" stroke-width="2"/></g><path d="M 72.61 156.19 Q 83.83 83.83 151.91 73.65" fill="none" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><g><line x1="151.91" y1="73.65" x2="156.19" y2="72.61" stroke="var(--ink)" stroke-width="2" class="fig-stroke"/><polyline points="149.53,78.67 156.19,72.61 147.5,70.28" fill="none" stroke="var(--ink)" stroke-width="2"/></g><circle cx="180" cy="70" r="18" fill="none" stroke="var(--cyan)" stroke-width="2" class="fig-stroke"/><text x="180" y="74" font-family="var(--font-display), system-ui, sans-serif" font-size="12" text-anchor="middle" fill="var(--ink-dim)">1</text><text x="180" y="38" font-family="var(--font-display), system-ui, sans-serif" font-size="13" text-anchor="middle" fill="var(--ink)">Evaporation</text><circle cx="290" cy="180" r="18" fill="none" stroke="var(--cyan)" stroke-width="2" class="fig-stroke"/><text x="290" y="184" font-family="var(--font-display), system-ui, sans-serif" font-size="12" text-anchor="middle" fill="var(--ink-dim)">2</text><text x="326" y="184" font-family="var(--font-display), system-ui, sans-serif" font-size="13" text-anchor="start" fill="var(--ink)">Condensation</text><circle cx="180" cy="290" r="18" fill="none" stroke="var(--cyan)" stroke-width="2" class="fig-stroke"/><text x="180" y="294" font-family="var(--font-display), system-ui, sans-serif" font-size="12" text-anchor="middle" fill="var(--ink-dim)">3</text><text x="180" y="330" font-family="var(--font-display), system-ui, sans-serif" font-size="13" text-anchor="middle" fill="var(--ink)">Precipitation</text><circle cx="70" cy="180" r="18" fill="none" stroke="var(--cyan)" stroke-width="2" class="fig-stroke"/><text x="70" y="184" font-family="var(--font-display), system-ui, sans-serif" font-size="12" text-anchor="middle" fill="var(--ink-dim)">4</text><text x="34" y="184" font-family="var(--font-display), system-ui, sans-serif" font-size="13" text-anchor="end" fill="var(--ink)">Collection</text></svg></figure>

---
