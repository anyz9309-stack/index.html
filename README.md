<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #ffdde1, #ee9ca7);
            margin-top: 100px;
            overflow: hidden;
        }

        h1 {
            color: #ffffff;
            font-size: 40px;
        }

        button {
            padding: 12px 25px;
            font-size: 18px;
            margin: 15px;
            border: none;
            border-radius: 15px;
            cursor: pointer;
            transition: 0.3s;
        }

        #yes {
            background-color: #ff4d6d;
            color: white;
        }

        #yes:hover {
            transform: scale(1.1);
        }

        #no {
            background-color: #555;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>

<h1>¿Quieres ser mi San Valentín? 💘</h1>

<button id="yes" onclick="yesClicked()">Sí 💖</button>
<button id="no" onmouseover="moveButton()">No 😒</button>

<script>
function yesClicked() {
    document.body.innerHTML = `
        <h1>AHHH DIJO QUE SÍ 😭💖</h1>
        <p style="color:white; font-size:24px;">
        Oficialmente eres mi San Valentín 💕<br>
        Te quiero muchísimo 🥺💗
        </p>
    `;
}

function moveButton() {
    const button = document.getElementById("no");
    button.style.top = Math.random() * (window.innerHeight - 50) + "px";
    button.style.left = Math.random() * (window.innerWidth - 100) + "px";
}
</script>

</body>
</html>
