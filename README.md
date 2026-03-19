# Birthday-Bash-Fred-Lex
<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RSVP: Frederique & Alexander</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital@0;1&family=Lato:wght@300;400&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Lato', sans-serif;
            background-color: #f9fbf2; /* Zachte lentekleur */
            background-image: url('https://www.transparenttextures.com/patterns/cubes.png'); /* Subtiel patroontje */
            color: #4a4a4a;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
        }
        .container {
            background: white;
            padding: 50px 40px;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
            max-width: 450px;
            width: 100%;
            text-align: center;
            border: 1px solid #e0eec6;
        }
        h1 { 
            font-family: 'Playfair Display', serif;
            color: #8da47e; 
            font-size: 2.2em;
            margin-bottom: 10px; 
        }
        .subtitle {
            font-style: italic;
            color: #aaa;
            margin-bottom: 30px;
            display: block;
        }
        p { line-height: 1.6; margin-bottom: 30px; font-size: 1.1em; }
        
        .form-group { text-align: left; margin-bottom: 25px; }
        label { display: block; margin-bottom: 8px; font-weight: 400; color: #6d7a5f; }
        
        input, select, textarea {
            width: 100%;
            padding: 14px;
            border: 1px solid #d1d9c5;
            border-radius: 10px;
            box-sizing: border-box;
            background-color: #fff;
            font-size: 16px;
            outline: none;
            transition: border 0.3s;
        }
        input:focus, select:focus, textarea:focus {
            border: 1px solid #8da47e;
        }

        button {
            background-color: #8da47e;
            color: white;
            border: none;
            padding: 16px 30px;
            border-radius: 10px;
            cursor: pointer;
            font-size: 18px;
            font-weight: bold;
            width: 100%;
            transition: background 0.3s, transform 0.2s;
            box-shadow: 0 4px 10px rgba(141, 164, 126, 0.3);
        }
        button:hover { 
            background-color: #7a8f6d; 
            transform: translateY(-2px);
        }
        button:active { transform: translateY(0); }

        .footer {
            margin-top: 25px;
            font-size: 0.9em;
            color: #bdc3c7;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>Frederique & Alexander</h1>
    <span class="subtitle">Save the date · Mei 2024</span>
    
    <p>Wij gaan een feestje vieren! De exacte datum volgt nog, maar we horen graag of je erbij kunt zijn.</p>

    <form action="https://formspree.io/f/meernokq" method="POST">
        
        <div class="form-group">
            <label for="naam">Naam / Namen</label>
            <input type="text" id="naam" name="naam" placeholder="Wie mogen we verwachten?" required>
        </div>

        <div class="form-group">
            <label for="rsvp">Ben je erbij?</label>
            <select id="rsvp" name="aanwezigheid" required>
                <option value="" disabled selected>Maak een keuze...</option>
                <option value="Ja, ik/wij komen graag!">Ja, ik/wij komen graag!</option>
                <option value="Helaas, ik/wij kunnen niet">Helaas, ik/wij kunnen niet</option>
            </select>
        </div>

        <div class="form-group">
            <label for="allergie">Allergieën of dieetwensen</label>
            <textarea id="allergie" name="allergie" rows="3" placeholder="Bijv. vegetarisch, glutenvrij, geen noten..."></textarea>
        </div>

        <input type="hidden" name="_subject" value="Nieuwe RSVP voor het feestje!">

        <button type="submit">Antwoord versturen</button>
    </form>
    
    <div class="footer">
        Tot snel!
    </div>
</div>

</body>
</html>
