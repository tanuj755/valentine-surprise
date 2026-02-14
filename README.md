<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Valentine's Day ❤️</title>
<style>
    body {
        margin: 0;
        padding: 0;
        font-family: 'Arial', sans-serif;
        background: linear-gradient(to right, #ff758c, #ff7eb3);
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        color: white;
        overflow: hidden;
    }

    .container {
        animation: fadeIn 2s ease-in-out;
    }

    h1 {
        font-size: 3em;
        margin-bottom: 10px;
    }

    p {
        font-size: 1.5em;
    }

    button {
        margin-top: 20px;
        padding: 12px 25px;
        font-size: 1em;
        border: none;
        border-radius: 25px;
        background-color: white;
        color: #ff4b7d;
        cursor: pointer;
        transition: 0.3s;
    }

    button:hover {
        background-color: #ff4b7d;
        color: white;
    }

    .heart {
        position: absolute;
        color: white;
        font-size: 20px;
        animation: float 5s linear infinite;
    }

    @keyframes fadeIn {
        from { opacity: 0; }
        to { opacity: 1; }
    }

    @keyframes float {
        from { transform: translateY(100vh); }
        to { transform: translateY(-10vh); }
    }
</style>
</head>
<body>

<div class="container">
    <h1>Happy Valentine's Day ❤️</h1>
    <p>You make my world brighter every single day!</p>
    <button onclick="showMessage()">Click Me 💌</button>
</div>

<script>
function showMessage() {
    alert("I love you more than words can say! 💖");
}

function createHeart() {
    const heart = document.createElement("div");
    heart.classList.add("heart");
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.animationDuration = (Math.random() * 3 + 2) + "s";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.remove();
    }, 5000);
}

setInterval(createHeart, 300);
</script>

</body>
</html>
