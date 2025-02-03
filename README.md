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
            background-color: pink;
            font-family: Arial, sans-serif;
        }
        .container {
            text-align: center;
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: red;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: red;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: darkred;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Will You Be My Valentine?</h1>
        <button onclick="alert('Yay! I\'m so happy! 💖')">Yes</button>
        <button onclick="alert('Oh no! Please reconsider! 😢')">No</button>
    </div>
</body>
</html>
