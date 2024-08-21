<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <title>¿Quieres ser mi novio?</title>
    <link rel="stylesheet" href="main.css">
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
    <script>
        $(document).ready(function(){
            $('.p1').hover(function(){
                var arriba = Math.random() * (400 - 1) + 1;
                var abajo = Math.random() * (609 - 1) + 1;
                $(this).css('top', arriba + 'px');
                $(this).css('left', abajo + 'px');
            });
        });

        function dijoSi(){
            document.getElementById('si').style.display = 'block';
        }
    </script>
</head>
<body>
    <div class="contenedor">
        <div class="titulo">
            <h1>¿Quieres ser mi novio?</h1>
        </div>
        <div class="opciones">
            <p class="p1">No</p>
            <p onclick="dijoSi()" class="p2">Sí</p>
            <div id="si">
                <h2>Gracias chetito, lo sabía. Feliz primer día de novios :3</h2>
            </div>
        </div>
    </div>
</body>
</html>
