<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">
<title>Seven Months of Us ❤️</title>

<style>
*{
  box-sizing:border-box;
}

html,body{
  margin:0;
  width:100%;
  height:100%;
  overflow:hidden;
}

body{
  font-family:Georgia,"Times New Roman",serif;
  color:#fff;
  background:
    radial-gradient(circle at 50% 30%,#35123d,#170a25 55%,#090817);
}

/* BACKGROUND */
#stars,#hearts{
  position:fixed;
  inset:0;
  pointer-events:none;
  overflow:hidden;
}

.star{
  position:absolute;
  width:2px;
  height:2px;
  background:white;
  border-radius:50%;
  opacity:.7;
  animation:twinkle 2s infinite;
}

@keyframes twinkle{
  50%{
    opacity:.1;
    transform:scale(.4);
  }
}

.heart{
  position:absolute;
  bottom:-35px;
  opacity:0;
  animation:floatUp 8s linear infinite;
}

@keyframes floatUp{
  10%{
    opacity:.7;
  }

  100%{
    transform:translateY(-115vh) rotate(30deg);
    opacity:0;
  }
}

/* PAGES */
.pages{
  width:100%;
  height:100%;
  position:relative;
}

.page{
  position:absolute;
  inset:0;
  padding:28px 20px 85px;

  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;

  opacity:0;
  transform:translateX(60px) scale(.97);

  pointer-events:none;

  transition:
    opacity .65s ease,
    transform .65s ease;
}

.page.active{
  opacity:1;
  transform:none;
  pointer-events:auto;
}

/* CARD */
.card{
  width:min(850px,94vw);
  max-height:90vh;
  overflow:auto;

  padding:35px 24px;

  border:1px solid rgba(255,255,255,.16);
  border-radius:30px;

  background:rgba(255,255,255,.065);
  backdrop-filter:blur(14px);

  box-shadow:
    0 20px 70px rgba(0,0,0,.35);
}

.kicker{
  letter-spacing:4px;
  text-transform:uppercase;
  color:#f3b8d4;
  font-size:11px;
}

h1{
  font-size:clamp(45px,11vw,90px);
  margin:18px 0 10px;
  line-height:.95;

  text-shadow:
    0 0 35px rgba(255,120,180,.5);
}

h2{
  font-size:clamp(30px,7vw,48px);
  margin:10px 0 20px;
}

p{
  font-size:18px;
  line-height:1.8;
  color:#f8e7ef;
  max-width:700px;
  margin:14px auto;
}

.big7{
  width:110px;
  height:110px;

  margin:18px auto;

  border-radius:50%;

  display:flex;
  align-items:center;
  justify-content:center;

  font-size:60px;

  border:1px solid rgba(255,210,235,.5);

  box-shadow:
    0 0 45px rgba(255,100,175,.3);

  background:rgba(255,255,255,.06);
}

.quote{
  font-size:24px;
  line-height:1.55;

  color:#ffd9e8;

  font-style:italic;

  margin:25px auto;

  max-width:650px;
}

/* BUTTON */
.btn{
  border:0;

  color:#fff;

  background:
    linear-gradient(
      135deg,
      #e85b9c,
      #9c62e8
    );

  padding:13px 23px;

  border-radius:999px;

  font-size:15px;

  cursor:pointer;

  box-shadow:
    0 8px 25px rgba(220,90,160,.25);

  font-family:inherit;

  transition:.2s;
}

.btn:hover{
  transform:translateY(-2px);
}

/* NAVIGATION */
.nav{
  position:fixed;
  z-index:10;

  bottom:22px;
  left:50%;

  transform:translateX(-50%);

  display:flex;
  gap:10px;

  align-items:center;
}

.nav button{
  border:1px solid rgba(255,255,255,.18);

  background:rgba(255,255,255,.08);

  color:#fff;

  border-radius:50%;

  width:44px;
  height:44px;

  font-size:18px;

  cursor:pointer;
}

#counter{
  font-size:12px;
  color:#d8bdcc;
  min-width:48px;
}

/* TREASURE GRID */
.grid{
  display:grid;
  grid-template-columns:
    repeat(3,1fr);

  gap:12px;

  margin:22px auto;

  max-width:720px;
}

.tile{
  padding:20px 10px;

  border-radius:20px;

  background:rgba(255,255,255,.055);

  border:
    1px solid rgba(255,255,255,.08);
}

.tile b{
  display:block;

  color:#ffd0e3;

  font-size:20px;

  margin-bottom:7px;
}

.tile span{
  font-size:13px;

  color:#ddcbd5;
}

/* TIMELINE */
.timeline{
  display:flex;

  justify-content:center;

  gap:7px;

  flex-wrap:wrap;

  margin:20px 0;
}

.m{
  padding:12px 15px;

  border-radius:15px;

  background:rgba(255,255,255,.06);
}

.m strong{
  color:#ffd0e3;

  font-size:20px;
}

/* FINAL SURPRISE */
.reveal{
  display:none;

  margin-top:24px;

  animation:appear .8s ease;
}

.reveal.show{
  display:block;
}

@keyframes appear{
  from{
    opacity:0;
    transform:translateY(15px);
  }

  to{
    opacity:1;
    transform:none;
  }
}

.surprise{
  font-size:clamp(40px,10vw,75px);

  margin:15px 0;

  text-shadow:
    0 0 30px rgba(255,120,180,.5);
}

.small{
  font-size:14px;
  color:#d9bdcc;
}

/* MOBILE */
@media(max-width:600px){

  .grid{
    grid-template-columns:1fr;
  }

  .card{
    padding:28px 17px;
  }

  p{
    font-size:16px;
  }

  .quote{
    font-size:20px;
  }
}
</style>
</head>


<body>

<!-- ANIMATED BACKGROUND -->
<div id="stars"></div>
<div id="hearts"></div>


<div class="pages">


<!-- PAGE 1 -->
<section class="page active">

<div class="card">

<div class="kicker">
A little universe made just for us
</div>

<div class="big7">
7
</div>

<h1>
Months of Us
</h1>

<p>
Seven months. Countless memories.
And a story that means so much to me. ❤️
</p>

<button class="btn" onclick="next()">
Open our story →
</button>

</div>

</section>



<!-- PAGE 2 -->
<section class="page">

<div class="card">

<div class="kicker">
Chapter One
</div>

<h2>
It all became “us” ❤️
</h2>

<p>
Somehow, among all the people in this huge world,
our paths crossed.

And since then, you've become one of the most
beautiful parts of my little world.
</p>

<div class="quote">

“The best part of these seven months
is simply that they were ours.”

</div>

<button class="btn" onclick="next()">
Turn the page →
</button>

</div>

</section>



<!-- PAGE 3 -->
<section class="page">

<div class="card">

<div class="kicker">
Chapter Two
</div>

<h2>
Seven little chapters
</h2>

<div class="timeline">

<div class="m">
<strong>1</strong><br>
Beginning
</div>

<div class="m">
<strong>2</strong><br>
Growing
</div>

<div class="m">
<strong>3</strong><br>
Smiles
</div>

<div class="m">
<strong>4</strong><br>
Memories
</div>

<div class="m">
<strong>5</strong><br>
Closer
</div>

<div class="m">
<strong>6</strong><br>
Beautiful
</div>

<div class="m">
<strong>7</strong><br>
Still Us ❤️
</div>

</div>

<p>
Every month added another little piece
to our story.

And I wouldn't trade those pieces
for anything.
</p>

<button class="btn" onclick="next()">
Next →
</button>

</div>

</section>



<!-- PAGE 4 -->
<section class="page">

<div class="card">

<div class="kicker">
Chapter Three
</div>

<h2>
Things I treasure
</h2>

<div class="grid">

<div class="tile">

<b>
Your Smile
</b>

<span>
A little thing that can make
a day feel brighter.
</span>

</div>


<div class="tile">

<b>
Our Talks
</b>

<span>
Even the simplest conversations
become memories.
</span>

</div>


<div class="tile">

<b>
Our Story
</b>

<span>
Something real, precious,
and uniquely ours.
</span>

</div>

</div>

<p>
It's not just the big moments.

It's the tiny moments that quietly
became special because they had
<i>you</i> in them.
</p>

<button class="btn" onclick="next()">
There's more… →
</button>

</div>

</section>



<!-- PAGE 5 -->
<section class="page">

<div class="card">

<div class="kicker">
Chapter Four
</div>

<h2>
A little message from my heart
</h2>

<p>
Princess, I hope you always know
how special you are to me.

I love the memories we've made,
the laughs we've shared,
and the feeling of having someone
who makes ordinary days feel
a little more beautiful.
</p>

<p>
I don't know exactly what every
tomorrow will look like,

but I know that these seven months
are memories I'll always be grateful for.
</p>

<div class="quote">

Happy 7 months, Princess. ❤️

</div>

<button class="btn" onclick="next()">
One last page… →
</button>

</div>

</section>



<!-- PAGE 6 -->
<section class="page">

<div class="card">

<div class="kicker">
Wait… I saved something
</div>

<h2>
🎁 Final Surprise For You
</h2>

<p>
I didn't want to end our little story
with just words.
</p>

<p>
<b>
There's one final surprise hidden here.
</b>
</p>

<button
class="btn"
onclick="
document
.getElementById('reveal')
.classList.add('show');

this.style.display='none';
">

✨ Reveal my surprise

</button>


<div
id="reveal"
class="reveal"
>

<div class="surprise">
❤️ ∞ ❤️
</div>

<h2>
You are my favorite chapter.
</h2>

<p>
And if I could add one more page
to this little website,
it would simply say:
</p>

<div class="quote">

“Thank you for being part of my story.
Happy 7 months to us.”

</div>

<p class="small">

This little universe may have an ending…
but our memories don't have to. ✨

</p>

</div>

</div>

</section>


</div>



<!-- BOTTOM NAVIGATION -->

<div class="nav">

<button onclick="prev()">
‹
</button>

<span id="counter">
1 / 6
</span>

<button onclick="next()">
›
</button>

</div>



<script>

/* PAGE NAVIGATION */

let current = 0;

const pages =
[
  ...document.querySelectorAll(".page")
];

const counter =
document.getElementById("counter");


function show(i){

  current =
    (i + pages.length)
    % pages.length;

  pages.forEach(
    (page,index)=>{

      page.classList.toggle(
        "active",
        index === current
      );

    }
  );

  counter.textContent =
    (current + 1)
    + " / "
    + pages.length;
}


function next(){

  show(current + 1);

}


function prev(){

  show(current - 1);

}



/* KEYBOARD CONTROLS */

document.addEventListener(
  "keydown",
  e => {

    if(
      e.key === "ArrowRight" ||
      e.key === " "
    ){

      e.preventDefault();

      next();

    }

    if(e.key === "ArrowLeft"){

      prev();

    }

  }
);



/* CREATE STARS */

const stars =
document.getElementById("stars");

for(let i=0;i<100;i++){

  let star =
  document.createElement("i");

  star.className="star";

  star.style.left =
    Math.random()*100+"%";

  star.style.top =
    Math.random()*100+"%";

  star.style.animationDelay =
    Math.random()*3+"s";

  stars.appendChild(star);

}



/* CREATE FLOATING HEARTS */

const hearts =
document.getElementById("hearts");

const symbols =
[
  "♥",
  "♡",
  "❤",
  "✦"
];

for(let i=0;i<24;i++){

  let heart =
  document.createElement("div");

  heart.className="heart";

  heart.textContent =
    symbols[
      Math.floor(
        Math.random()*symbols.length
      )
    ];

  heart.style.left =
    Math.random()*100+"%";

  heart.style.animationDelay =
    Math.random()*8+"s";

  heart.style.animationDuration =
    6 + Math.random()*6 + "s";

  heart.style.fontSize =
    14 + Math.random()*18 + "px";

  hearts.appendChild(heart);

}

</script>

</body>
</html>
