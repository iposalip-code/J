<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">

<meta name="viewport"
content="width=device-width,
initial-scale=1.0,
maximum-scale=1.0,
user-scalable=no">

<title>Maafin Gue Dong 😭</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    min-height:100vh;
    overflow:hidden;

    display:flex;
    justify-content:center;
    align-items:center;

    background:
    radial-gradient(circle at 20% 20%,#ffe7a8,transparent 30%),
    radial-gradient(circle at 80% 80%,#b8e8ff,transparent 30%),
    linear-gradient(135deg,#89f7fe,#66a6ff);

    color:#222;
}

/* =========================
   BACKGROUND EMOJI
========================= */

.bg{
    position:fixed;
    inset:0;
    overflow:hidden;
    pointer-events:none;
}

.float{
    position:absolute;
    bottom:-50px;

    font-size:25px;

    animation:floatUp linear infinite;

    opacity:.65;
}

@keyframes floatUp{

    0%{
        transform:translateY(0) rotate(0deg);
        opacity:0;
    }

    15%{
        opacity:.7;
    }

    100%{
        transform:
        translateY(-110vh)
        rotate(360deg);

        opacity:0;
    }
}

/* =========================
   CARD
========================= */

.card{

    width:90%;
    max-width:430px;

    padding:30px 24px;

    text-align:center;

    background:
    rgba(255,255,255,.78);

    backdrop-filter:blur(15px);

    border-radius:28px;

    box-shadow:
    0 20px 60px rgba(0,0,0,.2);

    animation:
    cardIn .8s ease;
}

@keyframes cardIn{

    from{
        opacity:0;
        transform:
        translateY(40px)
        scale(.85);
    }

    to{
        opacity:1;
        transform:
        translateY(0)
        scale(1);
    }
}

/* =========================
   EMOJI
========================= */

.mainEmoji{

    font-size:70px;

    margin-bottom:10px;

    animation:
    shake 1.5s infinite;
}

@keyframes shake{

    0%,100%{
        transform:rotate(0deg);
    }

    25%{
        transform:rotate(-8deg);
    }

    75%{
        transform:rotate(8deg);
    }
}

/* =========================
   TEXT
========================= */

h1{

    font-size:29px;

    margin-bottom:15px;

    color:#333;
}

.message{

    font-size:16px;

    line-height:1.7;

    color:#444;

    margin-bottom:20px;
}

.warning{

    display:inline-block;

    padding:7px 12px;

    margin-top:8px;

    border-radius:20px;

    background:#fff1a8;

    font-weight:bold;
}

/* =========================
   BUTTON AREA
========================= */

.buttons{

    position:relative;

    width:100%;

    height:140px;

    margin-top:10px;
}

button{

    border:none;

    padding:14px 23px;

    border-radius:50px;

    font-size:16px;

    font-weight:bold;

    cursor:pointer;

    box-shadow:
    0 8px 18px rgba(0,0,0,.15);

    transition:.25s;

    -webkit-tap-highlight-color:transparent;
}

/* YES */

.yes{

    position:absolute;

    left:50%;
    top:15px;

    transform:
    translateX(-50%);

    background:#333;

    color:white;
}

.yes:hover{

    transform:
    translateX(-50%)
    scale(1.08);
}

/* NO */

.no{

    position:absolute;

    left:50%;
    top:75px;

    transform:
    translateX(-50%);

    background:#eee;

    color:#555;
}

/* =========================
   SUCCESS
========================= */

.success{

    display:none;

    animation:
    successIn .7s ease;
}

@keyframes successIn{

    from{
        opacity:0;
        transform:scale(.6);
    }

    to{
        opacity:1;
        transform:scale(1);
    }
}

.successEmoji{

    font-size:75px;

    margin-bottom:10px;

    animation:
    bounce .8s infinite alternate;
}

@keyframes bounce{

    from{
        transform:translateY(0);
    }

    to{
        transform:translateY(-10px);
    }
}

.success h2{

    font-size:27px;

    margin-bottom:15px;
}

.success p{

    line-height:1.7;

    color:#444;
}

.friendBadge{

    display:inline-block;

    margin-top:15px;

    padding:8px 14px;

    border-radius:20px;

    background:#e8f4ff;

    font-weight:bold;
}

/* =========================
   CONFETTI
========================= */

.confetti{

    position:fixed;

    top:-30px;

    pointer-events:none;

    animation:
    fall 3s linear forwards;
}

@keyframes fall{

    to{

        transform:
        translateY(110vh)
        rotate(720deg);

        opacity:0;
    }
}

/* =========================
   FOOTER
========================= */

.footer{

    margin-top:18px;

    font-size:12px;

    color:#777;
}

</style>
</head>


<body>


<!-- BACKGROUND -->

<div class="bg" id="bg"></div>


<!-- CARD -->

<div class="card">


    <!-- HALAMAN AWAL -->

    <div id="main">


        <div class="mainEmoji">
            🥲
        </div>


        <h1>
            Woi, jangan ngambek 😭
        </h1>


        <p class="message">

            Oke, gue mau minta maaf dulu
            sebelum keadaan makin kacau 💀

            <br><br>

            Maaf ya kalau tadi gue bikin
            lu kesel, bete, atau kesel sama gue.

            <br><br>

            Gue emang kadang suka
            <b>ngomong/ngelakuin sesuatu tanpa mikir</b> 😭

            <br><br>

            Jadi...

            <br>

            <span class="warning">
                Maafin gue nggak? 🥲
            </span>

        </p>


        <div class="buttons">


            <button
            class="yes"
            onclick="forgive()">

                Ya udah, gue maafin 👍

            </button>


            <button
            class="no"
            id="noBtn">

                Nggak 😤

            </button>


        </div>


        <div class="footer">

            Tenang, ini bukan drama percintaan 😂

        </div>


    </div>



    <!-- HALAMAN SETELAH DI MAAFIN -->

    <div
    class="success"
    id="success">


        <div class="successEmoji">
            🗿
        </div>


        <h2>
            NAH GITU DONG 😂
        </h2>


        <p>

            Makasih udah maafin gue 😭

            <br><br>

            Sekarang kita balik ngobrol
            kayak biasa lagi.

            <br><br>

            Jangan ngambek lama-lama,
            capek gue ngejar tombol
            <b>“Nggak”</b> tadi 💀

        </p>


        <div class="friendBadge">

            BESTIE AMAN 🤝

        </div>


    </div>


</div>



<script>

/* =========================
   FLOATING EMOJI
========================= */

const bg =
document.getElementById("bg");

const emojis = [
    "😂",
    "😭",
    "💀",
    "🤣",
    "😤",
    "🤨",
    "🥲",
    "🗿",
    "✨"
];


function createFloat(){

    const el =
    document.createElement("div");

    el.className="float";

    el.innerText =
    emojis[
        Math.floor(
            Math.random()*emojis.length
        )
    ];

    el.style.left =
    Math.random()*100+"%";

    el.style.fontSize =
    (18+Math.random()*25)+"px";

    el.style.animationDuration =
    (5+Math.random()*6)+"s";

    el.style.animationDelay =
    Math.random()*2+"s";

    bg.appendChild(el);


    setTimeout(()=>{

        el.remove();

    },12000);
}


setInterval(createFloat,450);



/* =========================
   TOMBOL NGGAK KABUR
========================= */

const noBtn =
document.getElementById("noBtn");


function moveButton(){

    const area =
    document.querySelector(".buttons");


    const maxX =
    area.clientWidth -
    noBtn.offsetWidth;


    const maxY =
    area.clientHeight -
    noBtn.offsetHeight;


    const x =
    Math.random()*maxX;


    const y =
    Math.random()*maxY;


    noBtn.style.left =
    x+"px";


    noBtn.style.top =
    y+"px";


    noBtn.style.transform =
    "none";
}



/* HP */

noBtn.addEventListener(
    "touchstart",
    function(e){

        e.preventDefault();

        moveButton();

    }
);


/* PC */

noBtn.addEventListener(
    "mouseenter",
    function(){

        moveButton();

    }
);



/* =========================
   TOMBOL MAAF
========================= */

function forgive(){

    document.getElementById(
        "main"
    ).style.display="none";


    document.getElementById(
        "success"
    ).style.display="block";


    createConfetti();

}



/* =========================
   CONFETTI
========================= */

function createConfetti(){

    const items = [
        "😂",
        "🤣",
        "😭",
        "✨",
        "🎉",
        "⭐",
        "💀"
    ];


    for(
        let i=0;
        i<45;
        i++
    ){

        const c =
        document.createElement("div");


        c.className="confetti";


        c.innerText =
        items[
            Math.floor(
                Math.random()*items.length
            )
        ];


        c.style.left =
        Math.random()*100+"vw";


        c.style.fontSize =
        (14+Math.random()*18)+"px";


        c.style.animationDuration =
        (2+Math.random()*2)+"s";


        c.style.animationDelay =
        Math.random()+"s";


        document.body.appendChild(c);


        setTimeout(()=>{

            c.remove();

        },5000);

    }

}

</script>

</body>
</html>
