<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Love Story</title>
    <style>
        body {
            background-color: #fffafc;
            font-family: 'Arial', sans-serif;
            color: #ff79a0;
            text-align: center;
        }
        .container {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .envelope {
            width: 150px;
            height: 100px;
            background-color: #ffccd5;
            border-radius: 10px;
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
        }
        .envelope::before {
            content: '';
            position: absolute;
            width: 0;
            height: 0;
            border-style: solid;
            border-width: 0 75px 50px 75px;
            border-color: transparent transparent #ffccd5 transparent;
            top: -50px;
        }
        .heart {
            color: red;
            font-size: 24px;
        }
        button {
            background-color: #fff;
            color: #ff79a0;
            padding: 10px 20px;
            border-radius: 20px;
            border: none;
            cursor: pointer;
            margin-top: 20px;
        }
        button:hover {
            background-color: #ffccd5;
        }
        img {
            max-width: 80%;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .caption {
            font-size: 18px;
        }
    </style>
</head>
<body>

<div class="container">
    <!-- First page: Envelope with Heart -->
    <div class="envelope" onclick="nextPage()">
        <span class="heart">❤️</span>
    </div>
    <p>ลองกดดูงับ...</p>
</div>

<script>
    function nextPage() {
        window.location.href = "page2.html";
    }
</script>

</body>
</html>
