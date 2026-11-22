<!DOCTYPE html>
<html lang="ca">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Càrrega4 · Planificador de càrrega d’entrenament</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Familjen+Grotesk:wght@400;600;700&display=swap">
<style>
:root{--bg:#f2f5f3;--card:#fff;--ink:#14232a;--mute:#5d6e74;--line:#d5dfdb;--vol:#1f6f5c;--int:#c2410c;--den:#b7840f;--rest:#4b5fb5;--ld:#14232a;
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media (prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#0f1a1e;--card:#172429;--ink:#e8f0ed;--mute:#93a6ac;--line:#2b3c42;--vol:#4fc1a5;--int:#f08a52;--den:#e5b84a;--rest:#8d9cf0;--ld:#e8f0ed}}
:root[data-theme="dark"]{--bg:#0f1a1e;--card:#172429;--ink:#e8f0ed;--mute:#93a6ac;--line:#2b3c42;--vol:#4fc1a5;--int:#f08a52;--den:#e5b84a;--rest:#8d9cf0;--ld:#e8f0ed}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font:16px/1.5 "Familjen Grotesk",system-ui,sans-serif}
main{max-width:1000px;margin:0 auto;padding:24px 16px 48px}
h1{font-size:2rem;line-height:1.15;margin:0 0 6px;letter-spacing:-.01em}
h2{font-size:1.15rem;margin:0 0 10px}
p{margin:0 0 10px;max-width:70ch}.mute{color:var(--mute);font-size:.92rem}
section{background:var(--card);border:1px solid var(--line);border-radius:10px;padding:16px;margin-top:16px}
.scroll{overflow-x:auto}
table{border-collapse:collapse;width:100%;min-width:620px}
th,td{padding:6px 6px;text-align:left;border-bottom:1px solid var(--line);font-size:.93rem;white-space:nowrap}
th{font-weight:600;color:var(--mute)}
input,select,button{font:inherit;color:var(--ink);background:var(--bg);border:1px solid var(--line);border-radius:6px;padding:5px 7px}
input[type=number]{width:70px}input.nm{width:150px}
button{cursor:pointer}button.pri,button[aria-selected=true]{background:var(--vol);color:#fff;border-color:var(--vol)}
button:focus-visible,input:focus-visible,select:focus-visible{outline:2px solid var(--rest);outline-offset:2px}
.bar{display:inline-block;height:8px;border-radius:4px;vertical-align:middle;margin-right:6px}
.legend span{margin-right:14px;font-size:.9rem}.dot{display:inline-block;width:10px;height:10px;border-radius:50%;margin-right:5px}
.row{display:flex;gap:10px;flex-wrap:wrap;align-items:center;margin:8px 0}
.kpis{display:grid;grid-template-columns:repeat(auto-fit,minmax(130px,1fr));gap:10px}
.kpi{border-left:4px solid var(--c);padding:2px 10px}.kpi b{display:block;font-size:1.5rem}
code{background:var(--bg);padding:1px 5px;border-radius:4px}
.help{background:none;border:none;color:var(--mute);font-size:.8rem;padding:4px 0;margin-top:20px;cursor:pointer;text-decoration:underline;opacity:.7}.help:hover,.help:focus-visible{opacity:1}#hp[hidden]{display:none}
#pk{position:fixed;inset:0;background:rgba(0,0,0,.55);display:flex;align-items:flex-start;justify-content:center;padding:max(16px,env(safe-area-inset-top)) 12px 12px;z-index:50;overflow:auto}#pk[hidden]{display:none}
.pn{background:var(--card);border:1px solid var(--line);border-radius:10px;padding:14px;width:100%;max-width:640px;max-height:88vh;overflow:auto}
button.ex{display:block;width:100%;text-align:left;margin:0 0 6px;padding:8px 70px 8px 10px;position:relative}.sub{display:block;font-size:.74rem;color:var(--mute);font-weight:400}.tg{position:absolute;right:10px;top:8px;font-size:.7rem;color:var(--mute)}
</style>
</head>
<body>
<main>
<h1>Càrrega4</h1>
<p>Omple les 4 setmanes del mes, dia a dia (dilluns a diumenge), i obtén la càrrega de cada dia, de cada setmana i del mes, integrant <b>intensitat</b>, <b>volum</b>, <b>densitat</b> i <b>descans</b>.</p>

<section>
<h2>1. Setmanes i sessions</h2>
<div class="row" id="tabs" role="tablist"></div>
<div class="row" id="dtabs" role="tablist"></div>
<p class="mute">Tria la setmana i després el dia. Cada fila és un exercici d’aquell dia. Escriu el teu 1RM i el pes que faràs servir: l’app calcula el %1RM. Tempo = segons per repetició; descans = segons entre sèries.</p>
<div class="scroll"><table id="ses"><thead><tr><th>Exercici</th><th>Sèries</th><th>Reps</th><th>1RM (kg)</th><th>Pes (kg)</th><th>Tempo (s)</th><th>Descans (s)</th><th>Intensitat %1RM</th><th>Volum</th><th>Tonatge (kg)</th><th>Densitat</th><th>Ràtio T:D</th><th>Càrrega</th><th></th></tr></thead><tbody></tbody></table></div>
<div class="row"><button class="pri" id="add">Afegeix exercici</button><button id="cp">Copia aquesta setmana a les altres</button><button id="ex">Carrega exemple (4 setmanes)</button><button id="clr">Buida aquest dia</button><button id="clrall">Buida tot (4 setmanes)</button></div>
</section>

<section>
<h2>2. Càrrega per dia: <span id="wl"></span></h2>
<div class="scroll"><table id="dia"><thead><tr><th>Dia</th><th>Volum (reps)</th><th>Tonatge (kg)</th><th>Intensitat mitjana</th><th>Densitat mitjana</th><th>Càrrega</th></tr></thead><tbody></tbody></table></div>
</section>

<section>
<h2>3. Resultat del mes</h2>
<div class="kpis" id="kp"></div>
<div class="legend row"><span><i class="dot" style="background:var(--vol)"></i>Volum</span><span><i class="dot" style="background:var(--int)"></i>Intensitat</span><span><i class="dot" style="background:var(--den)"></i>Densitat</span><span><i class="dot" style="background:var(--rest)"></i>Descans</span><span><i class="dot" style="background:var(--ld)"></i>Càrrega</span></div>
<div class="scroll"><table id="res"><thead><tr><th>Setmana</th><th>Volum (reps)</th><th>Tonatge (kg)</th><th>Intensitat mitjana</th><th>Densitat mitjana</th><th>Descans total (min)</th><th>Càrrega</th></tr></thead><tbody></tbody></table></div>
<p class="mute">Les barres es comparen amb la setmana màxima de cada columna. La fila «Mes» suma o fa la mitjana de les 4 setmanes.</p>
</section>

<section>
<h2>4. Historial de càlculs</h2>
<div class="row"><input id="hn" class="nm" placeholder="Nom del càlcul (opcional)" maxlength="40"><button class="pri" id="hs">Desa aquest càlcul</button></div>
<div class="scroll"><table><thead><tr><th>Data</th><th>Nom</th><th>Set. 1</th><th>Set. 2</th><th>Set. 3</th><th>Set. 4</th><th>Total (UA)</th><th></th></tr></thead><tbody id="hl"></tbody></table></div>
<p class="mute">Es guarda en aquest navegador (fins a 20 càlculs). «Obre» recupera el càlcul complet.</p>
</section>
<div id="pk" hidden><div class="pn" role="dialog" aria-label="Tria un exercici"><div class="row"><input id="pq" type="search" placeholder="Cerca un exercici o múscul (p. ex. pit)" style="flex:1;min-width:180px"><button id="px">Tanca</button></div><div class="row" id="pc"></div><div id="pl"></div><p class="mute" id="pm"></p></div></div>
<div style="text-align:right"><button class="help" id="hb" aria-expanded="false" aria-controls="hp">Com funciona</button></div>
<section id="hp" hidden>
<h2>Com funciona</h2>
<p><b>Volum</b> = sèries × repeticions. <b>Intensitat</b> = pes ÷ 1RM × 100 (%1RM). <b>Densitat</b> = temps de treball ÷ (temps de treball + descans), amb temps de treball = sèries × repeticions × tempo. <b>Descans</b> = (sèries − 1) × descans entre sèries. <b>Tonatge</b> = sèries × repeticions × pes (kg).</p>
<p><b>Càrrega</b> = volum × (intensitat/100) × (0,5 + densitat). A igual volum i intensitat, descansar menys fa pujar la càrrega. El 0,5 evita que els descansos llargs facin caure la càrrega a zero. Unitats arbitràries (UA), per comparar sessions entre elles.</p>
</section>
</main>
<script>
const $=s=>document.querySelector(s);
const DN=["Dilluns","Dimarts","Dimecres","Dijous","Divendres","Dissabte","Diumenge"];
const GR={Pit:`Press banca|Press de pit en banc pla amb barra~Press inclinat|Press de pit en banc inclinat amb barra~Press declinat|Press de pit en banc declinat amb barra~Press amb manuelles|Press de pit en banc pla amb manuelles~Press inclinat amb manuelles|Press de pit en banc inclinat amb manuelles~Obertures a la pec deck|Obertura horitzontal de braços en màquina contractora~Obertures amb manuelles|Obertura de braços en banc pla amb manuelles~Creuaments a politja|Adducció horitzontal d'espatlla en politges~Fons per a pit|Flexió-extensió de colzes en paral·leles (tronc inclinat)~Press en màquina|Press de pit en màquina guiada~Flexions|Flexió de braços a terra`,
Espatlla:`Press militar|Press d'espatlles dret amb barra~Press d'espatlles amb manuelles|Press d'espatlles assegut amb manuelles~Elevacions laterals|Abducció d'espatlla amb manuelles (deltoide mitjà)~Elevacions frontals|Flexió d'espatlla amb manuelles (deltoide anterior)~Pàjaros|Abducció horitzontal d'espatlla inclinat (deltoide posterior)~Cara pull|Rem a la cara en politja alta amb corda~Encongiments|Elevació d'escàpules amb manuelles (trapezi superior)`,
Tríceps:`Extensió de tríceps amb corda|Extensió de colze en politja alta amb corda~Press francès|Extensió de colze tombat amb barra Z~Fons per a tríceps|Extensió de colzes en paral·leles (tronc vertical)~Extensió sobre el cap|Extensió de colze per sobre del cap amb manuella~Press tancat|Press de pit en banc pla amb agafada tancada`,
Esquena:`Rem en T|Rem amb barra T~Estirada al pit|Tracció vertical en politja alta~Rem amb agafada tancada|Rem en politja baixa amb agafada neutra~Dominades|Tracció vertical amb el propi pes~Rem amb barra|Rem inclinat amb barra~Rem amb manuella|Rem unilateral amb manuella~Pes mort|Elevació de barra des del terra (cadena posterior)~Pullover a politja|Extensió d'espatlla en politja alta amb braços estesos`,
Bíceps:`Curl de bíceps amb barra Z|Flexió de colze amb barra Z~Curl amb barra|Flexió de colze amb barra recta~Curl amb manuelles|Flexió de colze alterna amb manuelles~Curl martell|Flexió de colze amb manuelles i agafada neutra~Curl predicador|Flexió de colze en banc Scott`,
Quàdriceps:`Esquat amb barra|Esquat posterior amb barra~Esquat hack|Esquat en màquina hack~Premsa de cames|Extensió de maluc i genoll en premsa inclinada~Extensió de genolls|Extensió de genoll en màquina~Gambades|Gambada alterna amb manuelles`,
Isquiotibials:`Curl femoral|Flexió de genoll en màquina~Pes mort romanès|Extensió de maluc amb genolls lleugerament flexionats`,
Glutis:`Hip thrust|Extensió de maluc amb barra i banc~Patada de glutis a politja|Extensió de maluc en politja baixa`,
Adductors:`Màquina d'adductors|Adducció de maluc en màquina~Màquina d'abductors|Abducció de maluc en màquina`,
Bessons:`Bessons|Elevació de talons dret~Bessons asseguts|Elevació de talons assegut (sol)`,
Abdominals:`Crunch|Flexió de tronc a terra~Planxa|Isomètric abdominal en pronació~Elevació de cames|Flexió de maluc penjat de barra`};
const CAT=Object.entries(GR).flatMap(([g,v])=>v.split("~").map(x=>[g,...x.split("|")]));
const A=[["Press inclinat",1,4,10,90,63,3,90],["Press banca",1,4,8,110,85,3,120],["Obertures a la pec deck",1,3,12,70,45,3,60],["Press militar",1,3,10,60,42,3,90],["Elevacions laterals",1,3,15,25,15,3,45],["Extensió de tríceps amb corda",1,3,12,50,35,3,60],["Rem en T",2,4,10,80,56,3,90],["Estirada al pit",2,4,10,90,63,3,90],["Rem amb agafada tancada",2,3,12,80,52,3,75],["Curl de bíceps amb barra Z",2,3,10,50,35,3,60],["Màquina d'adductors",3,3,15,90,55,3,60],["Esquat hack",3,4,10,180,126,3,150],["Curl femoral",3,3,12,70,46,3,75],["Extensió de genolls",3,3,12,90,63,3,75],["Bessons",3,4,15,140,98,2,60]];
const EX=A.concat(A.map(a=>[a[0],a[1]+3,...a.slice(2)]));
const FV=[1,1.1,1.2,.7],FI=[1,1.02,1.04,.9];
let S=[[],[],[],[]],cur=0,cd=0;
const pct=s=>s.rm>0?s.kg/s.rm*100:0;
const f=(x,d=0)=>Number(x).toLocaleString("ca",{maximumFractionDigits:d,minimumFractionDigits:d});
const mk=a=>({name:a[0],day:a[1],sets:a[2],reps:a[3],rm:a[4],kg:a[5],tempo:a[6],rest:a[7],tech:(CAT.find(e=>e[1]==a[0])||[])[2]||""});
function calc(s){const p=pct(s),w=s.sets*s.reps*s.tempo,r=Math.max(s.sets-1,0)*s.rest,den=w+r?w/(w+r):0,vol=s.sets*s.reps;
return{vol,ton:vol*s.kg,int:p,den,rest:r,ratio:w?r/w:0,load:vol*(p/100)*(.5+den)}}
function agg(list){const d=Array(7).fill(0),dv=Array(7).fill(0),dt=Array(7).fill(0),di=Array(7).fill(0),dd=Array(7).fill(0),dn=Array(7).fill(0);let ton=0,vol=0,is=0,ds=0,rest=0;
list.forEach(s=>{const c=calc(s),k=Math.min(Math.max(s.day,1),7)-1;d[k]+=c.load;dv[k]+=c.vol;dt[k]+=c.ton;ton+=c.ton;di[k]+=c.int;dd[k]+=c.den;dn[k]++;vol+=c.vol;is+=c.int;ds+=c.den;rest+=c.rest});
const n=list.length,tot=d.reduce((a,b)=>a+b,0),m=tot/7,sd=Math.sqrt(d.reduce((a,b)=>a+(b-m)**2,0)/7),mono=sd?m/sd:0;
return{d,dv,dt,ton,di,dd,dn,vol,int:n?is/n:0,den:n?ds/n:0,rest:rest/60,load:tot,mono,strain:tot*mono}}
function tabs(){$("#tabs").innerHTML=["Primera","Segona","Tercera","Quarta"].map((t,w)=>`<button role="tab" data-w="${w}" aria-selected="${w==cur}" class="${w==cur?"pri":""}">${t} setmana</button>`).join("");const cnt=S[cur].reduce((a,x)=>(a[x.day-1]++,a),Array(7).fill(0));$("#dtabs").innerHTML=DN.map((n,i)=>`<button role="tab" data-d="${i}" aria-selected="${i==cd}" class="${i==cd?"pri":""}">${n}${cnt[i]?" ("+cnt[i]+")":""}</button>`).join("");$("#wl").textContent=["Primera","Segona","Tercera","Quarta"][cur]+" setmana"}
function rows(){const tb=$("#ses tbody");tb.innerHTML="";let n=0;S[cur].forEach((s,k)=>{if(s.day!=cd+1)return;n++;const c=calc(s),tr=document.createElement("tr");
tr.innerHTML=`<td><b>${s.name}</b><small class="sub">${s.tech||""}</small></td>`+["sets","reps","rm","kg","tempo","rest"].map(x=>`<td><input type="number" min="0" value="${s[x]}" data-k="${k}" data-f="${x}"></td>`).join("")+
`<td><b>${f(c.int,1)}%</b></td><td>${f(c.vol)}</td><td>${f(c.ton)}</td><td>${f(c.den*100)}%</td><td>1:${f(c.ratio,1)}</td><td><b>${f(c.load,1)}</b></td><td><button data-del="${k}" aria-label="Elimina">✕</button></td>`;tb.appendChild(tr)});
if(!n)tb.innerHTML=`<tr><td colspan="14" class="mute">Cap exercici el ${DN[cd].toLowerCase()} d’aquesta setmana. Afegeix-ne un amb el botó de sota.</td></tr>`;}
function bar(v,m,c){return`<i class="bar" style="width:${m?Math.round(v/m*70):0}px;background:var(--${c})"></i>`}
function results(){const A=agg(S[cur]),mxd=Math.max(...A.d,0);
$("#dia tbody").innerHTML=DN.map((n,i)=>{const q=A.dn[i];return`<tr><td>${n}</td><td>${f(A.dv[i])}</td><td>${f(A.dt[i])}</td><td>${q?f(A.di[i]/q,1)+"%":"–"}</td><td>${q?f(A.dd[i]/q*100)+"%":"–"}</td><td>${bar(A.d[i],mxd,"ld")}<b>${f(A.d[i],1)}</b>${q?"":" (descans)"}</td></tr>`}).join("");
const W=S.map(agg),mx=k=>Math.max(...W.map(x=>x[k]),0),t=W.reduce((a,x)=>a+x.load,0),act=W.filter((x,w)=>S[w].length);
$("#res tbody").innerHTML=W.map((x,w)=>`<tr><td>Setmana ${w+1}</td><td>${bar(x.vol,mx("vol"),"vol")}${f(x.vol)}</td><td>${f(x.ton)}</td><td>${bar(x.int,mx("int"),"int")}${f(x.int,1)}%</td><td>${bar(x.den,mx("den"),"den")}${f(x.den*100)}%</td><td>${bar(x.rest,mx("rest"),"rest")}${f(x.rest,1)}</td><td>${bar(x.load,mx("load"),"ld")}<b>${f(x.load,1)}</b></td></tr>`).join("")+
`<tr><td><b>Mes</b></td><td><b>${f(W.reduce((a,x)=>a+x.vol,0))}</b></td><td><b>${f(W.reduce((a,x)=>a+x.ton,0))}</b></td><td><b>${f(act.length?act.reduce((a,x)=>a+x.int,0)/act.length:0,1)}%</b></td><td><b>${f(act.length?act.reduce((a,x)=>a+x.den,0)/act.length*100:0)}%</b></td><td><b>${f(W.reduce((a,x)=>a+x.rest,0),1)}</b></td><td><b>${f(t,1)}</b></td></tr>`;
const top=mx("load");
$("#kp").innerHTML=[["Càrrega del mes",f(t,1)+" UA","ld"],["Mitjana setmanal",f(t/4,1)+" UA","vol"],["Tonatge del mes",f(W.reduce((a,x)=>a+x.ton,0))+" kg","rest"],["Setmana més exigent",top?"Setmana "+(W.findIndex(x=>x.load===top)+1):"–","int"],["Densitat mitjana",f(act.length?act.reduce((a,x)=>a+x.den,0)/act.length*100:0)+"%","den"]].map(k=>`<div class="kpi" style="--c:var(--${k[2]})"><span class="mute">${k[0]}</span><b>${k[1]}</b></div>`).join("");}
function all(){tabs();rows();results()}
$("#dtabs").addEventListener("click",e=>{const d=e.target.dataset.d;if(d!=null){cd=+d;all()}});
$("#tabs").addEventListener("click",e=>{const w=e.target.dataset.w;if(w!=null){cur=+w;all()}});
$("#ses").addEventListener("change",e=>{const t=e.target,k=t.dataset.k;if(k==null)return;S[cur][k][t.dataset.f]=t.dataset.f==="name"?t.value:Math.max(0,+t.value||0);all()});
$("#ses").addEventListener("click",e=>{const k=e.target.dataset.del;if(k!=null){S[cur].splice(k,1);all()}});
const nz=t=>t.normalize("NFD").replace(/[\u0300-\u036f]/g,"").toLowerCase(),esc=t=>t.replace(/[&<>"]/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;"}[c]));
let pg="",q="";
function pick(){$("#pc").innerHTML=["",...Object.keys(GR)].map(x=>`<button data-g="${x}" class="${x==pg?"pri":""}">${x||"Tots"}</button>`).join("");
const r=CAT.filter(e=>(!pg||e[0]==pg)&&(!q||nz(e[1]+" "+e[2]+" "+e[0]).includes(nz(q))));
$("#pl").innerHTML=r.length?r.map(e=>`<button class="ex" data-n="${e[1]}"><b>${e[1]}</b><small class="sub">${e[2]}</small><span class="tg">${e[0]}</span></button>`).join(""):'<p class="mute">Cap resultat.</p>'}
$("#add").onclick=()=>{$("#pm").textContent="Afegint al "+DN[cd].toLowerCase()+" de la setmana "+(cur+1)+".";$("#pk").hidden=false;pick();$("#pq").focus()};
$("#px").onclick=()=>{$("#pk").hidden=true};
$("#pk").addEventListener("click",e=>{if(e.target.id=="pk")$("#pk").hidden=true});
$("#pq").oninput=e=>{q=e.target.value;pick()};
$("#pc").onclick=e=>{if(e.target.dataset.g!=null){pg=e.target.dataset.g;pick()}};
$("#pl").onclick=e=>{const b=e.target.closest("button.ex");if(b){S[cur].push(mk([b.dataset.n,cd+1,3,10,100,70,3,90]));all();$("#pm").textContent="Afegit: "+b.dataset.n+" ("+DN[cd]+", setmana "+(cur+1)+"). Pots afegir-ne més o tancar."}};
const LK="c4h";
function hget(){try{return JSON.parse(localStorage.getItem(LK))||[]}catch(e){return[]}}
function hset(h){try{localStorage.setItem(LK,JSON.stringify(h))}catch(e){}}
function hist(){const h=hget();$("#hl").innerHTML=h.length?h.map((x,i)=>`<tr><td>${esc(x.date)}</td><td>${esc(x.name)}</td>`+x.w.map(v=>`<td>${f(v,1)}</td>`).join("")+`<td><b>${f(x.t,1)}</b></td><td><button data-r="${i}">Obre</button> <button data-x="${i}" aria-label="Elimina">✕</button></td></tr>`).join(""):'<tr><td colspan="8" class="mute">Encara no hi ha càlculs desats.</td></tr>'}
$("#hs").onclick=()=>{const W=S.map(agg).map(x=>x.load),h=hget();h.unshift({date:new Date().toLocaleString("ca",{dateStyle:"short",timeStyle:"short"}),name:$("#hn").value.trim()||"Sense nom",w:W,t:W.reduce((a,b)=>a+b,0),d:S});hset(h.slice(0,20));$("#hn").value="";hist()};
$("#hl").onclick=e=>{const b=e.target,h=hget();if(b.dataset.r!=null){S=JSON.parse(JSON.stringify(h[b.dataset.r].d));cur=0;cd=0;all()}else if(b.dataset.x!=null){h.splice(b.dataset.x,1);hset(h);hist()}};
hist();
$("#cp").onclick=()=>{S=S.map((w,i)=>i==cur?w:S[cur].map(s=>({...s})));all()};
$("#ex").onclick=()=>{S=FV.map((v,w)=>EX.map(a=>mk([a[0],a[1],Math.max(1,Math.round(a[2]*v)),a[3],a[4],Math.round(a[5]*FI[w]),a[6],a[7]])));all()};
$("#clr").onclick=()=>{S[cur]=S[cur].filter(s=>s.day!=cd+1);all()};
$("#clrall").onclick=()=>{S=[[],[],[],[]];cur=0;cd=0;all()};
$("#hb").onclick=()=>{const h=$("#hp"),o=h.hidden;h.hidden=!o;$("#hb").setAttribute("aria-expanded",o)};
$("#ex").click();
</script>
</body>
</html>
