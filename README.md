<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Skincare</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #e0c9a6;
            padding: 50px;
        }
        h1 {
            color: #5a3e2b;
        }
        button {
            background-color: #8b5e3b;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #6d4b33;
        }
        #result {
            margin-top: 20px;
            font-size: 18px;
            color: #4b2e1a;
        }
    </style>
</head>
<body>
    <h1>Skincare</h1>
    <button onclick="showTip()">Get a Skincare Tip</button>
    <p id="result"></p>

    <script>
        const tips = [
            "Mix honey and yogurt for a soothing face mask!",
            "Mash avocado and banana for a hydrating skin treatment!",
            "Drink at least 8 glasses of water daily for glowing skin!",
            "Always wear sunscreen to protect your skin from UV damage!",
            "Use aloe vera for a natural skin-soothing remedy!",
            "Exfoliate your skin twice a week to remove dead skin cells!",
            "Apply coconut oil before bedtime for deep hydration!"
        ];
        
        function showTip() {
            const randomIndex = Math.floor(Math.random() * tips.length);
            document.getElementById("result").textContent = tips[randomIndex];
        }
    </script>
</body>
</html>
