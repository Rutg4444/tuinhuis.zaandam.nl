<!DOCTYPE html>

<html lang="nl">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Boekingspagina Tuinhuis</title>

    <style>

        body {

            font-family: Arial, sans-serif;

            margin: 0;

            padding: 0;

            background-color: #f0f0f0;

            color: #333;

        }

        header {

            background-color: #4CAF50;

            color: white;

            text-align: center;

            padding: 20px 0;

        }

        .container {

            max-width: 800px;

            margin: 0 auto;

            padding: 20px;

            background-color: white;

            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);

        }

        h1 {

            color: #4CAF50;

        }

        label {

            display: block;

            margin-bottom: 5px;

            font-weight: bold;

        }

        input[type="text"], input[type="email"], input[type="date"], input[type="number"], textarea {

            width: 100%;

            padding: 8px;

            margin: 10px 0;

            border: 1px solid #ddd;

            border-radius: 4px;

        }

        input[type="submit"] {

            background-color: #4CAF50;

            color: white;

            border: none;

            padding: 10px 20px;

            cursor: pointer;

            font-size: 16px;

        }

        input[type="submit"]:hover {

            background-color: #45a049;

        }

        footer {

            background-color: #333;

            color: white;

            text-align: center;

            padding: 10px;

            position: fixed;

            width: 100%;

            bottom: 0;

        }

    </style>

</head>

<body>



<header>

    <h1>Boek je verblijf in het Tuinhuis</h1>

</header>



<div class="container">

    <form action="submit_form.php" method="POST">

        <label for="naam">Naam:</label>

        <input type="text" id="naam" name="naam" required>



        <label for="email">E-mail:</label>

        <input type="email" id="email" name="email" required>



        <label for="datum">Datum van verblijf:</label>

        <input type="date" id="datum" name="datum" required>



        <label for="aantal_personen">Aantal personen:</label>

        <input type="number" id="aantal_personen" name="aantal_personen" required min="1" max="5">



        <label for="speciale_verzoeken">Speciale verzoeken (optioneel):</label>

        <textarea id="speciale_verzoeken" name="speciale_verzoeken" rows="4" placeholder="Bijvoorbeeld dieetwensen, andere opmerkingen..."></textarea>



        <input type="submit" value="Boek nu">

    </form>

</div>



<footer>

    <p>&copy; 2025 Tuinhuis Boeking. Alle rechten voorbehouden.</p>

</footer>



</body>

</html>
