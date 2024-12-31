<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Funny Yes-No Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom, #a8e063, #56ab2f); /* Gradient background */
            color: white;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        h1 {
            font-size: 36px;
            margin-bottom: 30px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.4);
        }
        button {
            font-size: 20px;
            padding: 15px 30px;
            margin: 15px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
            transition: transform 0.2s, box-shadow 0.2s;
        }
        #yesButton {
            background-color: #4CAF50;
            color: white;
        }
        #noButton {
            background-color: #f44336;
            color: white;
        }
        button:hover {
            transform: scale(1.1);
            box-shadow: 0 6px 8px rgba(0, 0, 0, 0.3);
        }
    </style>
</head>
<body>
    <h1>Are you gay?</h1>
    <button id="yesButton">Yes</button>
    <button id="noButton">No</button>

    <script>
        const yesButton = document.getElementById("yesButton");
        const noButton = document.getElementById("noButton");

        // Handle the "No" button click
        noButton.addEventListener("click", () => {
            noButton.textContent = "Yes";
            noButton.style.backgroundColor = "#4CAF50";
            noButton.style.color = "white";
            alert("Changed your answer to Yes!");
        });

        // Handle the "Yes" button click
        yesButton.addEventListener("click", () => {
            alert("You answered Yes. Thank you for your honesty!");
        });
    </script>
</body>
</html>
