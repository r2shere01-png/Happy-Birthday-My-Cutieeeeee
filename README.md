<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Happy Birthday 🎂</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    height: 100vh;
    overflow: hidden;
    font-family: Arial, sans-serif;
    background: linear-gradient(135deg, #ff758c, #ff7eb3, #7b2ff7);
    display: flex;
    justify-content: center;
    align-items: center;
}

.card {
    position: relative;
    z-index: 10;
    width: 90%;
    max-width: 550px;
    padding: 40px 25px;
    text-align: center;
    border-radius: 30px;
    background: rgba(255,255,255,0.15);
    backdrop-filter: blur(15px);
    box-shadow: 0 20px 50px rgba(0,0,0,0.3);
    color: white;
}

h1 {
    font-size: 45px;
    margin-bottom: 15px;
    animation: glow 1.5s infinite alternate;
}

h2 {
    font-size: 32px;
    margin: 15px 0;
}

p {
    font-size: 19px;
    line-height: 1.6;
}

.cake {
    font-size: 85px;
    animation: bounce 1.5s infinite;
}

button {
    margin-top: 25px;
    padding: 14px 28px;
    border: none;
    border-radius: 30px;
    background: white;
    color: #ff4081;
    font-size: 18px;
    font-weight: bold;
    cursor: pointer;
}

#secret {
    display: none;
    margin-top: 20px;
    font-size: 20px;
}

.balloon {
    position: absolute;
    bottom: -120px;
    font-size: 65px;
    animation: float 8s linear infinite;
}

.b1 { left: 5%; animation-delay: 0s; }
.b2 { left: 25%; animation-delay: 2s; }
.b3 { left: 50%; animation-delay: 1s; }
.b4 { left: 75%; animation-delay: 3s; }
.b5 { left: 90%; animation-delay: 4s; }

@keyframes float {
    0% {
        transform: translateY(0) rotate(0deg);
    }
    100% {
        transform: translateY(-120vh) rotate(20deg);
    }
}

@keyframes bounce {
    0%,100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-15px);
    }
}

@keyframes glow {
    from {
        text-shadow: 0 0 10px white;
    }
    to {
        text-shadow: 0 0 30px white;
    }
}

.firework {
    position: absolute;
    font-size: 45px;
    animation: boom 2s infinite;
}

.f1 { top: 10%; left: 10%; }
.f2 { top: 15%; right: 10%; animation-delay: 1s; }
.f3 { bottom: 10%; left: 15%; animation-delay: .5s; }
.f4 { bottom: 15%; right: 15%; animation-delay: 1.5s; }

@keyframes boom {
    0%,100% {
        transform: scale(0.5);
        opacity: 0.3;
    }
    50% {
        transform: scale(1.3);
        opacity: 1;
    }
}
</style>
</head>

<body>

<div class="balloon b1">🎈</div>
<div class="balloon b2">🎈</div>
<div class="balloon b3">🎈</div>
<div class="balloon b4">🎈</div>
<div class="balloon b5">🎈</div>

<div class="firework f1">🎆</div>
<div class="firework f2">🎇</div>
<div class="firework f3">🎆</div>
<div class="firework f4">🎇</div>

<div class="card">

    <div class="cake">🎂</div>

    <h1>🎉 Happy Birthday 🎉</h1>

    <!-- Change the name here -->
    <h2>Dear Bestie ❤️</h2>

    <p>
        Wishing you a very happy birthday! 🥳
        <br>
        May your life be filled with happiness,
        success and countless beautiful memories. ✨
    </p>

    <button onclick="showWish()">
        🎁 Open Your Surprise
    </button>

    <div id="secret">
        💖 You deserve all the happiness in the world! 💖
        <br><br>
        🎊 Have an amazing birthday! 🎊
    </div>

</div>

<script>
function showWish() {
    document.getElementById("secret").style.display = "block";

    // Extra celebration
    document.body.style.animation = "glow 1s infinite alternate";
}
</script>

</body>
</html>
