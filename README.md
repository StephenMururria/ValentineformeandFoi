
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f7e0e0;
            color: #8b0000;
            text-align: center;
            padding: 50px;
        }
        h1 {
            font-size: 3em;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.5em;
            margin-bottom: 40px;
        }
        .heart {
            font-size: 5em;
            color: #ff0000;
        }
        .button {
            background-color: #ff4d4d;
            color: white;
font-size: 1.2em;
            padding: 15px 30px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
            margin: 10px;
        }
        .button:hover {
            background-color: #ff3333;
        }
        img {
            width: 300px;
            height: auto;
            margin-top: 20px;
            border-radius: 15px;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>

    <h1>Will you be my Valentine?</h1>
    <p>I've been thinking about how lucky I am to have you in my life...</p>
    <div class="heart">❤️</div>

    <!-- Add your photo here -->
    <img src="our-photo.jpg" alt="Us together">

    <p>So, here's a little website to ask you the most important question...</p>

    <button class="button" onclick="valentineAnswer('yes')">Yes, I will!</button>
    <button class="button" onclick="valentineAnswer('no')">No, I won't!</button>

    <!-- Broken Heart Image (hidden initially) -->
    <img id="broken-heart" src="broken-heart.jpg" alt="Broken Heart" class="hidden">

    <script>
        function valentineAnswer(answer) {
            if (answer === 'yes') {
                alert(' I am so happy you said YES! ❤️ I miss you so much, cant wait to see you >3');
} else if (answer === 'no') {
                const sureAnswer = confirm("Are you sure you are saying no🥲🥲?Press ok if yes or cancel");
                if (sureAnswer === false) {
                    alert("GOTCHA!!! YOU ALREADY ARE MY VALENTINE BAE ❤️");
                } else {
                    document.getElementById("broken-heart").classList.remove("hidden");
                    alert("NKT,HEBU RUDI NYUMA UFINYE YES😂");
                }
            }
        }
    </script>

</body>
</html>
``
