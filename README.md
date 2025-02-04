# Consiste en la creacion de un gestor de propiedad de valor
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox con Dos Columnas</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="flex-container">
        <div class="flex-item">
            <p>Pulsa en los siguientes párrafos, para cambiar los textos de la caja de la derecha</p>
            <form id="formulario" name="formulario">
                <input type="button" name ="debajo" value="Insertar nuevo elemento debajo de todos" id="debajo">
                <input type="button" value="Insertar nuevo elemento delante del segundo" name="segundo">
                <input type="button" value="Reemplazar el primer elemento de la caja por otro nuevo" name="reemplazar">
                <input type="button" value="Poner el segundo texto en último lugar" name="mover">
                <input type="button" value="Copia del segundo elemento al final" name="copia">
                <input type="button" value="Borrar el primer elemento" name="borrar">
            </form>
        </div>

        <div class="flex-item">
            <ul id="cuadro">
                <li>Texto fijo uno</li>
                <li>Texto fijo dos</li>
                <li>Texto fijo tres</li>
            </ul>
        </div>
        
    </div>
    <script src="script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <p id="miParrafo">
        Esto es un parrafo
    </p>
    <script>
        let nuevoParrafo = document.createElement("p");
        let nuevoTexto = document.createTextNode("Hola mundo");
        nuevoParrafo.appendChild(nuevoTexto);
        document.body.insertBefore(nuevoParrafo, document.getElementById("miParrafo"));
    </script>
</body>
</html>
