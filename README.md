<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Someone Special ❤️</title>
<style>
    body {
        background: linear-gradient(to right, #ff758c, #ff7eb3);
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: Arial, sans-serif;
        margin: 0;
    }

    .card {
        background: white;
        padding: 30px;
        border-radius: 15px;
        text-align: center;
        box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        animation: fadeIn 2s ease-in-out;
    }

    h1 {
        color: #ff4d6d;
    }

    button {
        background: #ff4d6d;
        color: white;
        border: none;
        padding: 12px 25px;
        margin: 10px;
        border-radius: 25px;
        cursor: pointer;
        font-size: 16px;
        transition: 0.3s;
    }

    button:hover {
        background: #e63950;
    }

    #noBtn {
        position: absolute;
    }

    @keyframes fadeIn {
        from {opacity: 0;}
        to {opacity: 1;}
    }
</style>
</head>
<body>

<div class="card">
    <h1>Hey ❤️</h1>
    <p id="text">I have something special to ask you...</p>
    
    <button onclick="propose()">Click Me 💖</button>
    
    <div id="proposal" style="display:none;">
        <h2>Will You Be Mine Forever? 💍</h2>
        <button onclick="yes()">Yes 💕</button>
        <button id="noBtn" onmouseover="moveNo()">No 😢</button>
    </div>
</div>

<script>
function propose() {
    document.getElementById("text").innerHTML = "You make my world brighter every day ☀️";
    document.getElementById("proposal").style.display = "block";
}

function yes() {
    document.body.innerHTML = "<h1 style='color:white;text-align:center;'>Yay!!! 💖 I Love You 😍</h1>";
}

function moveNo() {
    let btn = document.getElementById("noBtn");
    btn.style.top = Math.random() * window.innerHeight + "px";
    btn.style.left = Math.random() * window.innerWidth + "px";
}
</script>

</body>
</html>
