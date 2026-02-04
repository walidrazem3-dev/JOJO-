# JOJO-
Merhba biiik in "JOJO Question !"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JOJO Question</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            background-color: #f0f8ff;
            margin: 0;
        }
        img {
            width: 200px;
            height: auto;
            margin-bottom: 20px;
            border-radius: 10px;
        }
        h2 {
            color: #333;
            margin-bottom: 30px;
        }
        .buttons {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: transform 0.3s ease;
        }
        #yes {
            background-color: #4CAF50;
            color: white;
        }
        #no {
            background-color: #f44336;
            color: white;
        }
        #message {
            font-size: 14px;
            color: #666;
            margin-top: 10px;
            text-align: center;
        }
    </style>
</head>
<body>
    <img src="https://preview.redd.it/tiny-head-big-body-teddy-bear-aka-pip-the-bear-v0-mlh1k8p5lqk91.jpg?width=750&format=pjpg&auto=webp&s=bb219303ebce2f3ba005fbfbfa861d827077d1d1" alt="Teddy Bear with Big Head">
    <h2>JOJO Rasso Kbir ? ❤️ </h2>
    <div class="buttons">
        <div>
            <button id="yes">Ih</button>
            <button id="no">Lala</button>
        </div>
        <p id="message"></p>
    </div>

    <script>
        let yesScale = 1;
        let noScale = 1;
        let clickCount = 0;

        document.getElementById('no').addEventListener('click', function() {
            clickCount++;
            yesScale *= 1.2;
            noScale *= 0.8;
            document.getElementById('yes').style.transform = `scale(${yesScale})`;
            document.getElementById('no').style.transform = `scale(${noScale})`;

            const messageElement = document.getElementById('message');
            if (clickCount === 1) {
                messageElement.textContent = "Oooh Binetna rena ngessro";
            } else if (clickCount === 2) {
                messageElement.textContent = "Ayaa Chwiiiya kbir nrml iiih";
            } else if (clickCount === 3) {
                messageElement.textContent = "Khlas raso sghir w Nifek Kbiir mliha ?";
            } else {
                messageElement.textContent = "Khlas raso sghir c bn, Click sur Ih"; // Répète après le 3ème
            }
        });

        document.getElementById('yes').addEventListener('click', function() {
            alert('Hakaa Nhebeek Ma Vie ❤️❤️');
        });
    </script>
</body>
</html>
