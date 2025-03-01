<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DailyKnowledge.com</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            text-align: center;
        }
        header {
            background: #333;
            color: white;
            padding: 20px;
            font-size: 24px;
        }
        .container {
            padding: 20px;
        }
        .fact {
            background: white;
            padding: 20px;
            margin: 20px auto;
            max-width: 600px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .subscribe {
            margin-top: 20px;
        }
        .subscribe-button {
            background: red;
            color: white;
            font-size: 20px;
            padding: 15px 30px;
            border: none;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <header>Daily Knowledge</header>
    <div class="container">
        <div class="fact">
            <h2>Did You Know?</h2>
            <p id="fact-text">Loading a fun fact...</p>
        </div>
        <div class="subscribe">
            <p>Expand your knowledge daily by subscribing to Daily Knowledge.</p>
            <a href="https://www.youtube.com/channel/UCFPLNCACoyaKumaE8bi6Kzg" class="subscribe-button" target="_blank">Subscribe</a>
        </div>
    </div>
    <script>
        const facts = [
            "Honey never spoils.",
            "Bananas are berries, but strawberries aren't.",
            "Octopuses have three hearts.",
            "A day on Venus is longer than a year on Venus.",
            "Water can boil and freeze at the same time."
        ];
        
        document.getElementById("fact-text").innerText = facts[Math.floor(Math.random() * facts.length)];
    </script>
</body>
</html>

