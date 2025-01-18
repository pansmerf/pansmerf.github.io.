<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Walentynka</title>
    <style>
        body {
            background-color: red;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 20%;
            background-image: none; /* Usunięcie obrazu tła, pozostaje czyste czerwone tło */
        }
        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        .yes {
            background-color: #4CAF50;
            color: white;
        }
        .no {
            background-color: #f44336;
            color: white;
        }
    </style>
</head>
<body>
    <div id="content">
        <h1>Zostaniesz moją walentynką?</h1>
        <button class="yes" onclick="showMessage('Kocham Cię! ❤️')">Tak</button>
        <button class="no" onclick="showMessage('A to spierdalaj 😅')">Nie</button>
    </div>

    <p id="message" style="margin-top: 20px; font-size: 20px;"></p>

    <script>
        function showMessage(text) {
            document.getElementById('content').style.display = 'none';
            document.getElementById('message').textContent = text;
        }
    </script>
</body>
</html>
