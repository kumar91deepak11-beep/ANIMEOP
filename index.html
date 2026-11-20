
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>ANIMEOP</title>
<style>
*{box-sizing:border-box}
body{margin:0;background:#090910;color:white;font-family:Arial}
header{padding:20px;background:#15151f;border-bottom:1px solid #333}
.logo{font-size:30px;font-weight:bold;color:#b56aff}
main{padding:16px;max-width:900px;margin:auto}
input{width:100%;padding:14px;background:#20202a;color:white;border:1px solid #444;border-radius:9px;margin:12px 0}
.tabs{display:flex;gap:8px;overflow-x:auto;padding:10px 0}
button{background:#963be8;color:white;border:0;border-radius:8px;padding:12px}
.tab{background:#252530}
.tab.active{background:#963be8}
.grid{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:12px;margin-top:18px}
.card{background:#191923;border-radius:12px;overflow:hidden}
.thumb{width:100%;aspect-ratio:16/9;object-fit:cover}
.info{padding:12px}
.info h3{font-size:15px}
.info p{font-size:12px;color:#bbb;line-height:1.5}
.play{width:100%}
#watch{display:none;margin-top:25px;background:#191923;padding:14px;border-radius:12px}
iframe{width:100%;aspect-ratio:16/9;border:0;border-radius:10px}
a{color:#c99aff}
.note{color:#bbb;font-size:13px;line-height:1.6}
@media(max-width:420px){.grid{grid-template-columns:1fr}}
</style>
</head>
<body>

<header>
<div class="logo">ANIMEOP</div>
</header>

<main>
<h2>Discover Anime</h2>
<input id="search" placeholder="Search anime..."
oninput="render()">

<div class="tabs">
<button class="tab active" onclick="change('all',this)">All</button>
<button class="tab" onclick="change('full',this)">Full Episodes</button>
<button class="tab" onclick="change('trailers',this)">Trailers</button>
<button class="tab" onclick="change('japanese',this)">Japanese Anime</button>
</div>

<div id="status" class="note"></div>
<div class="grid" id="catalogue"></div>

<div id="watch">
<h2 id="watchTitle">Watch Anime</h2>
<div id="video"></div>
<p id="credit" class="note"></p>
<p><a id="original" target="_blank" rel="noopener">Official original video</a></p>
<p><a id="license" target="_blank" rel="noopener">License details</a></p>
</div>

<p class="note">
ANIMEOP displays officially hosted videos. Reuse or redistribution
requires checking the original license and giving required credit.
</p>
</main>

<script>
const episodes = [
{
 title:"Morevna Episode 3.0.2 (English)",
 category:"full",
 thumbnail:"https://i.ytimg.com/vi/ecVv2IB7f5k/hqdefault.jpg",
 youtube:"ecVv2IB7f5k",
 creator:"Morevna Project",
 license:"Creative Commons Attribution-ShareAlike 4.0 (as stated in the video description)",
 original:"https://www.youtube.com/watch?v=ecVv2IB7f5k",
 licenseURL:"https://creativecommons.org/licenses/by-sa/4.0/"
 }
];

let selected="all";

function change(type,button){
 selected=type;
 document.querySelectorAll(".tab").forEach(b=>
  b.classList.remove("active")
 );
 button.classList.add("active");
 render();
}

function render(){
 const grid=document.getElementById("catalogue");
 const query=document.getElementById("search").value.toLowerCase();

 grid.innerHTML="";

 const results=episodes.filter(item=>{
  const matches=item.title.toLowerCase().includes(query);
  const category=selected==="all" ||
    (selected==="full" && item.category==="full") ||
    (selected==="trailers" && item.category==="trailers") ||
    (selected==="japanese" && item.category==="japanese");
  return matches && category;
 });

 document.getElementById("status").textContent=
  results.length+" verified catalogue item(s)";

 if(selected==="trailers" || selected==="japanese"){
  document.getElementById("status").textContent=
   "No verified items added in this category yet.";
 }

 if(selected==="full" && results.length===0){
  document.getElementById("status").textContent=
   "No verified full episodes available yet.";
 }

 results.forEach(item=>{
  const card=document.createElement("div");
  card.className="card";

  const img=document.createElement("img");
  img.className="thumb";
  img.src=item.thumbnail;
  img.alt=item.title;

  const info=document.createElement("div");
  info.className="info";

  const title=document.createElement("h3");
  title.textContent=item.title;

  const creator=document.createElement("p");
  creator.textContent="Creator: "+item.creator;

  const license=document.createElement("p");
  license.textContent="License: "+item.license;

  const btn=document.createElement("button");
  btn.className="play";
  btn.textContent="WATCH EPISODE";
  btn.onclick=()=>watch(item);

  info.append(title,creator,license,btn);
  card.append(img,info);
  grid.append(card);
 });
}

function watch(item){
 document.getElementById("watchTitle").textContent=item.title;

 document.getElementById("video").innerHTML=
  '<iframe src="https://www.youtube-nocookie.com/embed/'+
  item.youtube+
  '" title="Official Morevna video" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>';

 document.getElementById("credit").textContent=
  "Creator: "+item.creator+" | "+item.license;

 document.getElementById("original").href=item.original;
 document.getElementById("license").href=item.licenseURL;

 document.getElementById("watch").style.display="block";
 document.getElementById("watch").scrollIntoView({behavior:"smooth"});
}

render();
</script>
</body>
</html>
