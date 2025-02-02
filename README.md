<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
            color: #d63384;
            padding: 50px;
        }
        .container {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            display: inline-block;
        }
        h1 {
            font-size: 2em;
        }
        .heart {
            font-size: 50px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            background-color: #ff4d6d;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            border-radius: 5px;
            cursor: pointer;
            margin: 10px;
        }
        button:hover {
            background-color: #e6004c;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>¿Quieres ser mi San Valentín? ❤️</h1>
        <p>Mi desde que llegaste a mi, le devolviste la alegria a mi vida y ahora todo es hermoso a tu lado </p>
        <div class="heart">💖💞💖</div>
        <div class="buttons">
            <button onclick="respuesta('Sí')">Sí, ¡acepto! 💕</button>
            <button onclick="respuesta('No')">No, pero sigues siendo increíble 😊</button>
        </div>
    </div>

    <script>
        function respuesta(res) {
            if (res === 'Sí') {
                alert('¡Yay! No sabes cuánto me haces feliz 💖');
            } else {
                alert('Bueno... seguiré intentándolo 💔');
            }
        }
    </script>

</body>
</html>
