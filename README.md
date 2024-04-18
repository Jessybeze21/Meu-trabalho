<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            font-family: 'Montserrat', sans-serif;
        }

        a {
            text-decoration: none;
        }

        .box {
            font-size: 30px;
            color: #F7DF1E;
            height: 200vh;
            width: 200vw;
            border-radius: 10px;
            background: #191919;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;    }

        button {
            height: 40px;
            width: 100px;
            background: white;
            color: black;
            font-weight: 600;
            border-radius: 5px;
            border: 2px solid black;
            cursor: pointer;
        }
    </style>
    <title>Pedido Irrecusável</title>
</head>
<body>
    <div class="box">
        <p>Me da o seu C*zinho?</p>
        <div class="buttons-container">
            <button><a href="https://gifman.net/wp-content/uploads/2019/07/bob-esponja-19.gif">Sim</a></button>
            <button id="no">Não</button>
        </div>
    </div>
</body>
<script>
    let button = document.getElementById('no');
    let height = window.innerHeight - 100;
    let width = window.innerWidth - 100;

    button.addEventListener('mouseover', function () {
        button.style.position = "absolute"
        button.style.top = Math.random() * height + "px";
        button.style.left = Math.random() * width + "px";
    })
</script>
</html>
