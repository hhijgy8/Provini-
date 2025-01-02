<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mini App - Doppiaggio</title>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 20px;
            background-color: #f9f9f9;
        }
        h1 {
            color: #005f88;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }
        .image-card {
            width: 150px;
            text-align: center;
        }
        .image-card img {
            width: 100%;
            border-radius: 10px;
            cursor: pointer;
            transition: transform 0.2s;
            border: 2px solid transparent;
        }
        .image-card img:hover {
            transform: scale(1.1);
            border-color: #0088cc;
        }
        button {
            margin-top: 30px;
            background-color: #005f88;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #004466;
        }
    </style>
</head>
<body>
    <h1>Mini App - Doppiaggio</h1>
    <p>Clicca su un'immagine per registrare il tuo doppiaggio!</p>

    <!-- Container per le immagini -->
    <div class="container">
        <!-- Card per il primo personaggio -->
        <div class="image-card">
            <img src="https://via.placeholder.com/150" alt="Personaggio 1" onclick="startRecording('Personaggio 1')">
            <p>Personaggio 1</p>
        </div>

        <!-- Card per il secondo personaggio -->
        <div class="image-card">
            <img src="https://via.placeholder.com/150" alt="Personaggio 2" onclick="startRecording('Personaggio 2')">
            <p>Personaggio 2</p>
        </div>

        <!-- Card per il terzo personaggio -->
        <div class="image-card">
            <img src="https://via.placeholder.com/150" alt="Personaggio 3" onclick="startRecording('Personaggio 3')">
            <p>Personaggio 3</p>
        </div>
    </div>

    <button onclick="endSession()">Termina Sessione</button>

    <script>
        const tg = window.Telegram.WebApp;

        // Funzione per avviare una registrazione
        function startRecording(character) {
            alert(`Inizia a registrare il doppiaggio per: ${character}`);
            tg.sendData(`Registrazione avviata per: ${character}`);
        }

        // Funzione per chiudere la sessione
        function endSession() {
            tg.close();
        }
    </script>
</body>
</html>
