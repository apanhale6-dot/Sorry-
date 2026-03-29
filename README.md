<html>
<head>
  <title>Sorry My Love ❤️</title>

  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;600&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Quicksand', sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #ffd6e0, #fff0f5);
      overflow: hidden;
    }

    h1 {
      color: white;
      margin-top: 20px;
      font-weight: 600;
    }

    .page {
      display: none;
      height: 100vh;
      padding: 40px 20px;
      animation: fade 0.6s ease;
    }

    .active {
      display: block;
    }

    @keyframes fade {
      from { opacity: 0; transform: scale(0.95);}
      to { opacity: 1; transform: scale(1);}
    }

    p {
      font-size: 20px;
      max-width: 650px;
      margin: auto;
      margin-top: 80px;
      color: #5a3e36;
      line-height: 1.7;
    }

    button {
      margin-top: 40px;
      padding: 14px 30px;
      border-radius: 30px;
      border: none;
      background: #ff8fab;
      color: white;
      font-size: 16px;
      cursor: pointer;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      transition: 0.3s;
    }

    button:hover {
      transform: scale(1.1);
      background: #ff6f91;
    }

    /* floating emojis */
    .float {
      position: absolute;
      font-size: 22px;
      animation: floatUp 6s linear infinite;
    }

    @keyframes floatUp {
      from { transform: translateY(100vh); opacity: 1; }
      to { transform: translateY(-10vh); opacity: 0; }
    }

  </style>
</head>

<body>

<h1>Sorry My Love ❤️</h1>

<!-- PAGE 1 -->
<div id="page1" class="page active">
  <p>Dear bubu I am sorry for eveyrthinf till now and what ive been till now 🧸❤️</p>
  <button onclick="showPage(2)">Next ❤️</button>
</div>

<!-- PAGE 2 -->
<div id="page2" class="page">
  <p>So Ill just be frank and honest . Ive not been the best ive had many faults in me I dont wanna loose you lets sort everything and make our reln work and I really will do my beat to be a good boyf for you but one real thing see i really really love you and i cammot imagine a life without you . I really always want you really . 💖</p>
  <button onclick="showPage(3)">Next 🧸</button>
</div>

<!-- PAGE 3 -->
<div id="page3" class="page">
  <p>I really am always in love with you and tbh the feelings that ive for you are really very different . Things are really really messed uo but still ik we cam figure out and even that ik if im all good reln will be as u want i really really love you the most and i do really mean this ik u might be nkt seeing mt actions but i give you a promise from this moment you will 🫶</p>
  <button onclick="showPage(4)">Next 💖</button>
</div>

<!-- PAGE 4 -->
<div id="page4" class="page">
  <p>Please lets just fix everything together because i always want us to be togetjer and i really will do anything to keep u with me and yes i want you and only you and you are the love of my life my everything i cant be without you ❤️</p>
  <button onclick="showPage(5)">Last ❤️</button>
</div>

<!-- PAGE 5 -->
<div id="page5" class="page">
  <p>So pls im sorry and lets fix<br>Yes or yes no option u have 😤❤️</p>
  <button onclick="alert('I love you Bubu ❤️🧸')">Yes ❤️</button>
  <button onclick="alert('No option 😏❤️')">Yes 😏</button>
</div>

<script>

function showPage(n) {
  document.querySelectorAll(".page").forEach(p => p.classList.remove("active"));
  document.getElementById("page" + n).classList.add("active");
}

/* floating emojis */
function floatEmoji() {
  const emojis = ["❤️","💖","🧸","💕","💗"];
  let el = document.createElement("div");
  el.className = "float";
  el.innerHTML = emojis[Math.floor(Math.random()*emojis.length)];
  el.style.left = Math.random()*100 + "vw";
  document.body.appendChild(el);
  setTimeout(()=>el.remove(), 6000);
}

setInterval(floatEmoji, 500);

</script>

</body>
</html>
