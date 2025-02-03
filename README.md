<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Will You Be My Valentine?</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: rgb(98, 165, 114);
            font-family: Arial, sans-serif;
        }
        .container {
            text-align: center;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            position: relative;
            width: 90%;
            max-width: 400px;
        }
        h1 {
            color: rgb(255, 141, 179);
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            border: none;       
            border-radius: 5px;
            cursor: pointer;
            margin: 5px;
        }
        button:hover {
            opacity: 0.8;
        }
        #yesButton {
            background-color: green;
        }
        #yesButton:hover {
            background-color: darkgreen;
        }
        #noButton {
            background-color: red;
            transition: transform 0.5s ease;
        }
        #noButton:hover {
            background-color: darkred;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://i.pinimg.com/736x/07/0c/1d/070c1d0703fa4374389580c71885fbe1.jpg">
        <h1>Can we try again cinta??</h1>
        <button id="yesButton" onclick="alert('Yay!💖')">Yes</button>
        <button id="noButton" onclick="moveButton()">No</button>
    </div>

    <script>
        function moveButton() {
            const noButton = document.getElementById('noButton');
            const container = document.querySelector('.container');
            const containerRect = container.getBoundingClientRect();

            // Generate random positions within the container
            const randomX = Math.random() * (containerRect.width - noButton.offsetWidth);
            const randomY = Math.random() * (containerRect.height - noButton.offsetHeight);

            // Apply new position using transform for smoother animation
            noButton.style.transform = `translate(${randomX}px, ${randomY}px)`;
        }
    </script>
</body>
</html>
