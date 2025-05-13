<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sube tu CV</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #e3f2fd; /* Azul pastel suave */
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container {
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            width: 90%;
            max-width: 500px;
            padding: 40px;
            text-align: center;
        }

        h1 {
            color: #1976d2; /* Azul más fuerte para el título */
            font-size: 28px;
            margin-bottom: 20px;
        }

        p {
            color: #4f8aef; /* Azul suave para el texto */
            font-size: 16px;
            margin-bottom: 25px;
        }

        .button {
            background-color: #64b5f6; /* Azul pastel para el botón */
            color: #fff;
            padding: 15px 25px;
            font-size: 18px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .button:hover {
            background-color: #42a5f5; /* Azul más oscuro al pasar el ratón */
        }

        input[type="file"] {
            display: none; /* Ocultamos el botón de carga estándar */
        }

        label {
            background-color: #64b5f6; /* Azul pastel */
            color: white;
            padding: 15px 25px;
            font-size: 18px;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            margin-top: 20px;
        }

        label:hover {
            background-color: #42a5f5;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Sube tu CV aquí</h1>
        <p>Haz clic en el botón a continuación para cargar tu CV en formato PDF o Word.</p>
        <form action="tu_script_de_subida.php" method="post" enctype="multipart/form-data">
            <label for="cv">Seleccionar archivo</label>
            <input type="file" id="cv" name="cv" accept=".pdf,.docx,.doc" required>
            <button class="button" type="submit">Subir CV</button>
        </form>
    </div>
</body>
</html>
