<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Password Generator</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        .container {
            text-align: center;
        }
        .password-input {
            font-size: 18px;
            padding: 10px;
            margin-bottom: 10px;
            width: 300px;
        }
        .generate-button {
            font-size: 16px;
            padding: 10px 20px;
            cursor: pointer;
        }
        .generated-password {
            font-size: 20px;
            font-weight: bold;
            padding: 10px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Password Generator</h2>
        <input type="number" id="lengthInput" class="password-input" min="1" max="50" placeholder="비밀번호 길이 입력">
        <button onclick="generatePassword()" class="generate-button">비밀번호 생성</button>
        <div id="generatedPassword" class="generated-password">비밀번호 임시수</div>
    </div>

    <script>
        function generatePassword() {
            var length = document.getElementById("lengthInput").value;
            var password = generateRandomPassword(length);
            document.getElementById("generatedPassword").textContent = password;
        }

        function generateRandomPassword(length) {
            var charset = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#?_";
            var password = "";
            for (var i = 0; i < length; i++) {
                var randomIndex = Math.floor(Math.random() * charset.length);
                password += charset[randomIndex];
            }
            return password;
        }
    </script>
</body>
</html>
