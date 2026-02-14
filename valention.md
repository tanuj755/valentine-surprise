<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Happy Valentine's Day ❤️</title>

<style>

&nbsp;   body {

&nbsp;       margin: 0;

&nbsp;       padding: 0;

&nbsp;       font-family: 'Arial', sans-serif;

&nbsp;       background: linear-gradient(to right, #ff758c, #ff7eb3);

&nbsp;       height: 100vh;

&nbsp;       display: flex;

&nbsp;       justify-content: center;

&nbsp;       align-items: center;

&nbsp;       text-align: center;

&nbsp;       color: white;

&nbsp;       overflow: hidden;

&nbsp;   }



&nbsp;   .container {

&nbsp;       animation: fadeIn 2s ease-in-out;

&nbsp;   }



&nbsp;   h1 {

&nbsp;       font-size: 3em;

&nbsp;       margin-bottom: 10px;

&nbsp;   }



&nbsp;   p {

&nbsp;       font-size: 1.5em;

&nbsp;   }



&nbsp;   button {

&nbsp;       margin-top: 20px;

&nbsp;       padding: 12px 25px;

&nbsp;       font-size: 1em;

&nbsp;       border: none;

&nbsp;       border-radius: 25px;

&nbsp;       background-color: white;

&nbsp;       color: #ff4b7d;

&nbsp;       cursor: pointer;

&nbsp;       transition: 0.3s;

&nbsp;   }



&nbsp;   button:hover {

&nbsp;       background-color: #ff4b7d;

&nbsp;       color: white;

&nbsp;   }



&nbsp;   .heart {

&nbsp;       position: absolute;

&nbsp;       color: white;

&nbsp;       font-size: 20px;

&nbsp;       animation: float 5s linear infinite;

&nbsp;   }



&nbsp;   @keyframes fadeIn {

&nbsp;       from { opacity: 0; }

&nbsp;       to { opacity: 1; }

&nbsp;   }



&nbsp;   @keyframes float {

&nbsp;       from { transform: translateY(100vh); }

&nbsp;       to { transform: translateY(-10vh); }

&nbsp;   }

</style>

</head>

<body>



<div class="container">

&nbsp;   <h1>Happy Valentine's Day ❤️</h1>

&nbsp;   <p>You make my world brighter every single day!</p>

&nbsp;   <button onclick="showMessage()">Click Me 💌</button>

</div>



<script>

function showMessage() {

&nbsp;   alert("I love you more than words can say! 💖");

}



function createHeart() {

&nbsp;   const heart = document.createElement("div");

&nbsp;   heart.classList.add("heart");

&nbsp;   heart.innerHTML = "❤️";

&nbsp;   heart.style.left = Math.random() \* 100 + "vw";

&nbsp;   heart.style.animationDuration = (Math.random() \* 3 + 2) + "s";

&nbsp;   document.body.appendChild(heart);



&nbsp;   setTimeout(() => {

&nbsp;       heart.remove();

&nbsp;   }, 5000);

}



setInterval(createHeart, 300);

</script>



</body>

</html>



