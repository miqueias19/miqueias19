<!DOCTYPE html>
<html>
<head>
    <title>Meu Site em JavaScript</title>
    <style>
        /* Estilos CSS */
        body {
            font-family: Arial, sans-serif;
        }
        h1 {
            color: #333;
        }
    </style>
</head>
<body>
    <h1>Bem-vindo ao Meu Site em JavaScript!</h1>

    <p id="demo">Este é um exemplo de manipulação de conteúdo com JavaScript.</p>

    <script>
        // JavaScript
        // Manipulação de conteúdo
        var element = document.getElementById("demo");
        element.innerHTML = "O conteúdo foi alterado com JavaScript!";
    </script>
</body>
</html>

