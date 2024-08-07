# Good-morning-Vanshika-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Good Morning Vanshika</title>
    <style>
        body, html {
            height: 100%;
            margin: 0;
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #87CEEB;
            overflow: hidden;
        }
        .container {
            text-align: center;
            position: relative;
        }
        .message {
            font-size: 2em;
            font-weight: bold;
            color: white;
            position: absolute;
            top: 20%;
            left: 50%;
            transform: translate(-50%, -50%);
            animation: popIn 2s ease-out;
        }
        @keyframes popIn {
            0% { transform: translate(-50%, -50%) scale(0); opacity: 0; }
            100% { transform: translate(-50%, -50%) scale(1); opacity: 1; }
        }
        .sun {
            width: 100px;
            height: 100px;
            background: yellow;
            border-radius: 50%;
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            animation: rise 5s ease-out forwards;
        }
        @keyframes rise {
            0% { bottom: -20%; }
            100% { bottom: 60%; }
        }
        .lavenders {
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 10px;
            animation: grow 3s ease-out forwards;
            animation-delay: 2s;
        }
        .lavender {
            width: 20px;
            height: 100px;
            background: purple;
            border-radius: 10px 10px 0 0;
            transform: scaleY(0);
            animation: grow 3s ease-out forwards;
        }
        @keyframes grow {
            0% { transform: scaleY(0); }
            100% { transform: scaleY(1); }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="message">Good Morning Vanshika</div>
        <div class="sun"></div>
        <div class="lavenders">
            <div class="lavender"></div>
            <div class="lavender"></div>
            <div class="lavender"></div>
            <div class="lavender"></div>
        </div>
    </div>
</body>
</html>
