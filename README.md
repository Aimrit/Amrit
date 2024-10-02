<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Do You Love Me?</title>
    <style>
        body {
            text-align: center;
            margin-top: 50px;
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
        }

        .container {
            width: 50%;
            margin: auto;
            border: 2px solid #ccc;
            padding: 20px;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h1 {
            font-size: 24px;
            margin-bottom: 30px;
        }

        .btn {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
        }

        #no {
            position: relative;
        }

        #message {
            font-size: 24px;
            color: red;
            margin-top: 20px;
            display: none;
        }

        #footer {
            font-size: 18px;
            margin-top: 20px;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Do you love me?</h1>
        <button class="btn" id="yes" onclick="loveConfirmed()">Yes</button>
        <button class="btn" id="no" onmouseover="moveNoButton()">No</button>
        <p id="message">I Love You Too ♥️😘</p>
        <p id="footer">From your lovely Amrit</p>
    </div>

    <script>
        function loveConfirmed() {
            document.getElementById("message").style.display = "block"; // Show the "I Love You Too" message
            document.getElementById("footer").style.display = "block"; // Show "from your lovely Amrit"
        }

        function moveNoButton() {
            const noButton = document.getElementById('no');
            const x = Math.floor(Math.random() * (window.innerWidth - 100));
            const y = Math.floor(Math.random() * (window.innerHeight - 50));
            noButton.style.position = 'absolute';
            noButton.style.left = x + 'px';
            noButton.style.top = y + 'px';
        }
    </script>
</body>
</html>
