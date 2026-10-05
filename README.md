<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="MTJ Academy - Plateforme éducative et professionnelle de M K Jérémie">
<title>MTJ Academy | Éducation & Entrepreneuriat</title>

<style>
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{
font-family:Arial,Helvetica,sans-serif;
background:#f4f7fb;
color:#172033;
line-height:1.6
}
header{
position:sticky;
top:0;
z-index:1000;
background:#0b1736;
color:white;
box-shadow:0 3px 15px #0002
}
.nav{
max-width:1200px;
margin:auto;
padding:15px 20px;
display:flex;
align-items:center;
justify-content:space-between;
gap:20px
}
.logo{
font-size:22px;
font-weight:900;
letter-spacing:1px
}
.logo span{color:#35d0ff}
nav a{
color:white;
text-decoration:none;
margin:0 8px;
font-weight:bold
}
nav a:hover{color:#35d0ff}
select{
padding:9px;
border-radius:8px;
border:0
}
.hero{
background:linear-gradient(135deg,#07142f,#123b76,#087fa3);
color:white;
padding:85px 20px;
text-align:center
}
.hero h1{
font-size:clamp(38px,7vw,70px);
margin-bottom:15px
}
.hero p{
font-size:20px;
max-width:750px;
margin:0 auto 30px;
opacity:.92
}
.btn{
display:inline-block;
padding:14px 24px;
border-radius:10px;
background:#35d0ff;
color:#06142e;
font-weight:bold;
text-decoration:none;
border:0;
cursor:pointer
}
.btn:hover{transform:translateY(-2px)}
.stats{
max-width:1100px;
margin:-35px auto 40px;
position:relative;
display:grid;
grid-template-columns:repeat(4,1fr);
gap:15px;
padding:0 20px
}
.stat{
background:white;
padding:25px;
border-radius:15px;
text-align:center;
box-shadow:0 8px 25px #0001
}
.stat strong{
display:block;
font-size:30px;
color:#087fa3
}
.container{
max-width:1200px;
margin:auto;
padding:20px
}
.title{
text-align:center;
margin:30px 0
}
.title h2{
font-size:34px;
color:#0b1736
}
.title p{color:#687386}
.tools{
display:flex;
gap:12px;
flex-wrap:wrap;
margin-bottom:25px
}
.search{
flex:1;
min-width:230px;
padding:14px;
border:2px solid #dce3ee;
border-radius:10px;
font-size:16px
}
.filters{
display:flex;
gap:8px;
flex-wrap:wrap
}
.filter{
padding:11px 15px;
border:0;
border-radius:9px;
background:#e5ebf4;
cursor:pointer;
font-weight:bold
}
.filter.active,.filter:hover{
background:#0b1736;
color:white
}
.grid{
display:grid;
grid-template-columns:repeat(4,1fr);
gap:18px
}
.card{
background:white;
border-radius:16px;
padding:22px;
box-shadow:0 7px 22px #00000010;
border:1px solid #e7ebf2;
transition:.25s;
cursor:pointer
}
.card:hover{
transform:translateY(-5px);
box-shadow:0 14px 30px #0002
}
.icon{font-size:38px;margin-bottom:10px}
.card h3{margin-bottom:8px;color:#0b1736}
.card p{color:#687386;font-size:14px}
.level{
display:inline-block;
margin-top:15px;
padding:5px 9px;
border-radius:20px;
background:#e8f8fc;
color:#087fa3;
font-size:12px;
font-weight:bold
}
#course{
display:none;
background:white;
margin:40px auto;
max-width:1000px;
padding:30px;
border-radius:18px;
box-shadow:0 10px 35px #0002
}
.course-head{
display:flex;
justify-content:space-between;
gap:20px;
align-items:flex-start;
margin-bottom:25px
}
.close{
border:0;
background:#eef2f7;
padding:10px 15px;
border-radius:8px;
cursor:pointer
}
.lesson{
background:#f6f8fc;
padding:20px;
border-radius:12px;
margin:15px 0
}
.lesson h3{color:#0b1736;margin-bottom:7px}
.quiz{
margin-top:30px;
padding:25px;
background:#0b1736;
color:white;
border-radius:15px
}
.quiz button{
margin:7px 5px;
padding:11px 15px;
border:0;
border-radius:8px;
cursor:pointer
}
#result{
margin-top:15px;
font-weight:bold
}
footer{
margin-top:50px;
background:#07142f;
color:white;
text-align:center;
padding:35px 20px
}
footer strong{color:#35d0ff}
.hidden{display:none!important}

@media(max-width:900px){
.grid{grid-template-columns:repeat(2,1fr)}
.stats{grid-template-columns:repeat(2,1fr)}
nav a{display:none}
}
@media(max-width:600px){
.grid{grid-template-columns:1fr}
.stats{grid-template-columns:1fr 1fr}
.hero{padding:65px 18px}
.hero p{font-size:17px}
.course-head{display:block}
.close{margin-top:15px}
}
</style>
</head>

<body>

<header>
<div class="nav">
<div class="logo">MTJ <span>ACADEMY</span></div>

<nav>
<a href="#accueil">Accueil</a>
<a href="#formations">Formations</a>
<a href="#apropos">À propos</a>
</nav>

<select id="language">
<option value="fr">🇫🇷 Français</option>
<option value="en">🇬🇧 English</option>
</select>
</div>
</header>

<section class="hero" id="accueil">
<h1>Apprends. Construis. Réussis.</h1>
<p>
Une plateforme éducative moderne pour développer tes connaissances,
tes compétences et préparer ton avenir.
</p>
<a href="#formations" class="btn">Découvrir les formations</a>
</section>

<section class="stats">
<div class="stat"><strong>20</strong>Formations</div>
<div class="stat"><strong>100+</strong>Leçons</div>
<div class="stat"><strong>FR/EN</strong>Deux langues</div>
<div class="stat"><strong>24/7</strong>Accessible</div>
</section>

<main class="container" id="formations">

<div class="title">
<h2>Nos formations</h2>
<p>Choisis une matière et commence ton apprentissage.</p>
</div>

<div class="tools">
<input
id="search"
class="search"
type="search"
placeholder="🔎 Rechercher une formation..."
>
</div>

<div class="filters">
<button class="filter active" onclick="filterCourses('all',this)">Toutes</button>
<button class="filter" onclick="filterCourses('school',this)">📚 École</button>
<button class="filter" onclick="filterCourses('tech',this)">⚙️ Technique</button>
<button class="filter" onclick="filterCourses('business',this)">💼 Business</button>
<button class="filter" onclick="filterCourses('digital',this)">💻 Numérique</button>
</div>

<div class="grid" id="courseGrid"></div>

<section id="course">
<div class="course-head">
<div>
<h2 id="courseTitle"></h2>
<p id="courseDescription"></p>
</div>
<button class="close" onclick="closeCourse()">✕ Fermer</button>
</div>

<div id="lessons"></div>

<div class="quiz">
<h2>🧠 Mini Quiz</h2>
<p id="question">Quelle est la capitale du Cameroun ?</p>

<button onclick="checkAnswer('yaounde')">Yaoundé</button>
<button onclick="checkAnswer('douala')">Douala</button>
<button onclick="checkAnswer('bertoua')">Bertoua</button>

<div id="result"></div>
</div>
</section>

</main>

<section class="container" id="apropos">
<div class="title">
<h2>À propos de MTJ Academy</h2>
<p>
MTJ Academy est une plateforme éducative créée pour rendre
l'apprentissage plus simple, moderne et accessible.
</p>
</div>
</section>

<footer>
<p><strong>MTJ ACADEMY</strong></p>
<p>Éducation • Technologie • Entrepreneuriat</p>
<p>© 2026 M K Jérémie — Tous droits réservés</p>
</footer>

<script>

const courses = [

{
id:1,name:"Mathématiques",icon:"📐",cat:"school",
desc:"Développe ta logique et maîtrise les bases des mathématiques.",
lessons:[
"Les nombres et les opérations",
"Fractions et pourcentages",
"Équations et expressions",
"Géométrie et calculs"
]},

{
id:2,name:"Français",icon:"📖",cat:"school",
desc:"Améliore ta grammaire, ton vocabulaire et ton expression.",
lessons:[
"Grammaire",
"Conjugaison",
"Orthographe",
"Expression écrite"
]},

{
id:3,name:"Anglais",icon:"🇬🇧",cat:"school",
desc:"Apprends à communiquer et à comprendre l'anglais.",
lessons:[
"Alphabet et vocabulaire",
"Verbes essentiels",
"Conversation",
"English for work"
]},

{
id:4,name:"Électricité",icon:"⚡",cat:"tech",
desc:"Découvre les principes fondamentaux de l'électricité.",
lessons:[
"Tension, courant et résistance",
"Loi d'Ohm",
"Circuits électriques",
"Sécurité électrique"
]},

{
id:5,name:"Électronique",icon:"🔌",cat:"tech",
desc:"Comprends les composants et les circuits électroniques.",
lessons:[
"Résistances",
"Condensateurs",
"Diodes",
"Transistors"
]},

{
id:6,name:"Informatique",icon:"💻",cat:"digital",
desc:"Maîtrise les bases de l'informatique et du numérique.",
lessons:[
"Ordinateur et systèmes",
"Fichiers et dossiers",
"Internet",
"Sécurité numérique"
]},

{
id:7,name:"Programmation",icon:"👨‍💻",cat:"digital",
desc:"Apprends à créer des programmes et des sites web.",
lessons:[
"Introduction au code",
"HTML et CSS",
"JavaScript",
"Logique de programmation"
]},

{
id:8,name:"Entrepreneuriat",icon:"🚀",cat:"business",
desc:"Transforme une idée en projet.",
lessons:[
"Trouver une idée",
"Créer un projet",
"Étudier le marché",
"Développer son activité"
]},

{
id:9,name:"Marketing",icon:"📣",cat:"business",
desc:"Apprends à promouvoir un produit ou un service.",
lessons:[
"Marketing de base",
"Publicité",
"Réseaux sociaux",
"Création de contenu"
]},

{
id:10,name:"Commerce",icon:"🛒",cat:"business",
desc:"Découvre les techniques de vente et de commerce.",
lessons:[
"Introduction au commerce",
"Relation client",
"Techniques de vente",
"Fidélisation"
]},

{
id:11,name:"Gestion",icon:"📊",cat:"business",
desc:"Apprends à organiser et gérer une activité.",
lessons:[
"Organisation",
"Budget",
"Gestion des stocks",
"Gestion d'entreprise"
]},

{
id:12,name:"Histoire",icon:"🏛️",cat:"school",
desc:"Explore les grandes périodes et événements historiques.",
lessons:[
"Antiquité",
"Moyen Âge",
"Époque moderne",
"Histoire du Cameroun"
]},

{
id:13,name:"Géographie",icon:"🌍",cat:"school",
desc:"Découvre les pays, territoires, populations et environnements.",
lessons:[
"Continents",
"Pays et capitales",
"Relief et climat",
"Afrique et Cameroun"
]},

{
id:14,name:"Citoyenneté",icon:"🤝",cat:"school",
desc:"Comprends tes droits, tes devoirs et la vie en société.",
lessons:[
"Citoyen et citoyenneté",
"Droits et devoirs",
"Respect des autres",
"Responsabilité"
]},

{
id:15,name:"Culture générale",icon:"🧠",cat:"school",
desc:"Développe tes connaissances dans plusieurs domaines.",
lessons:[
"Sciences",
"Géographie",
"Histoire",
"Actualités et connaissances"
]},

{
id:16,name:"Développement personnel",icon:"🌱",cat:"business",
desc:"Développe tes habitudes, ton organisation et ta confiance.",
lessons:[
"Objectifs",
"Organisation",
"Discipline",
"Persévérance"
]},

{
id:17,name:"Communication",icon:"🎤",cat:"business",
desc:"Apprends à mieux parler, écouter et présenter tes idées.",
lessons:[
"Communication orale",
"Écoute",
"Présentation",
"Communication professionnelle"
]},

{
id:18,name:"Emploi & CV",icon:"📄",cat:"business",
desc:"Prépare ton CV et développe tes compétences professionnelles.",
lessons:[
"Créer un CV",
"Lettre de motivation",
"Entretien",
"Recherche d'emploi"
]},

{
id:19,name:"Intelligence artificielle",icon:"🤖",cat:"digital",
desc:"Découvre les bases et les usages de l'intelligence artificielle.",
lessons:[
"Qu'est-ce que l'IA ?",
"IA générative",
"Utiliser les outils IA",
"IA et avenir professionnel"
]},

{
id:20,name:"Réseaux & Numérique",icon:"🌐",cat:"digital",
desc:"Comprends les réseaux informatiques et le monde numérique.",
lessons:[
"Réseaux informatiques",
"Internet",
"Adresses IP",
"Sécurité numérique"
]}

];

const grid=document.getElementById("courseGrid");

function displayCourses(list){

grid.innerHTML="";

list.forEach(c=>{

const card=document.createElement("div");

card.className="card";

card.dataset.cat=c.cat;

card.innerHTML=`
<div class="icon">${c.icon}</div>
<h3>${c.name}</h3>
<p>${c.desc}</p>
<span class="level">FORMATION</span>
`;

card.onclick=()=>openCourse(c);

grid.appendChild(card);

});

}

function openCourse(c){

document.getElementById("course").style.display="block";

document.getElementById("courseTitle").textContent=
c.icon+" "+c.name;

document.getElementById("courseDescription").textContent=c.desc;

document.getElementById("lessons").innerHTML=
c.lessons.map((lesson,i)=>`
<div class="lesson">
<h3>Leçon ${i+1}</h3>
<p>${lesson}</p>
</div>
`).join("");

document.getElementById("result").textContent="";

document.getElementById("course").scrollIntoView({
behavior:"smooth"
});

}

function closeCourse(){

document.getElementById("course").style.display="none";

window.scrollTo({
top:document.getElementById("formations").offsetTop-80,
behavior:"smooth"
});

}

function filterCourses(category,button){

document.querySelectorAll(".filter")
.forEach(b=>b.classList.remove("active"));

button.classList.add("active");

if(category==="all"){
displayCourses(courses);
}else{
displayCourses(courses.filter(c=>c.cat===category));
}

}

document.getElementById("search").addEventListener("input",function(){

const text=this.value.toLowerCase();

displayCourses(
courses.filter(c=>
c.name.toLowerCase().includes(text) ||
c.desc.toLowerCase().includes(text)
)
);

});

function checkAnswer(answer){

const result=document.getElementById("result");

if(answer==="yaounde"){

result.textContent="✅ Bonne réponse !";

}else{

result.textContent="❌ Mauvaise réponse. Essaie encore !";

}

}

document.getElementById("language").addEventListener("change",function(){

if(this.value==="en"){

document.querySelector(".hero h1").textContent=
"Learn. Build. Succeed.";

document.querySelector(".hero p").textContent=
"A modern educational platform to develop your knowledge, skills and future.";

document.querySelector(".hero .btn").textContent=
"Discover courses";

document.querySelector(".title h2").textContent=
"Our Courses";

document.querySelector(".title p").textContent=
"Choose a subject and start learning.";

document.getElementById("search").placeholder=
"🔎 Search for a course...";

}else{

document.querySelector(".hero h1").textContent=
"Apprends. Construis. Réussis.";

document.querySelector(".hero p").textContent=
"Une plateforme éducative moderne pour développer tes connaissances, tes compétences et préparer ton avenir.";

document.querySelector(".hero .btn").textContent=
"Découvrir les formations";

document.querySelector(".title h2").textContent=
"Nos formations";

document.querySelector(".title p").textContent=
"Choisis une matière et commence ton apprentissage.";

document.getElementById("search").placeholder=
"🔎 Rechercher une formation...";

}

});

displayCourses(courses);

</script>

</body>
</html>
