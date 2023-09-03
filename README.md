# html-css-js-project-scaffolding
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tic Tac Toe</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #282c35;
            margin: 0;
            padding: 0;
        }

        header {
            text-align: center;
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            font-size: 50px;
            margin-top: 20px;
        }

        .box {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 35px;
        }

        .row {
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .btn {
            width: 75px;
            height: 75px;
            border: 2px solid white;
            border-radius: 10px;
            font-size: 50px;
            font-weight: 500;
            text-align: center;
            color: white;
            background-color: rgba(255, 255, 255, 0.7);
            cursor: pointer;
        }

        .btn:hover {
            background-color: rgba(255, 255, 255, 0.9);
            transition: background-color 0.2s;
        }

        .btn:disabled {
            color: black;
            cursor: not-allowed;
        }

        .result-container {
            background-color: rgba(255, 255, 255, 0.7);
            border: 2px solid white;
            max-width: 200px;
            margin: 20px auto;
            text-align: center;
        }

        .result {
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            font-size: 25px;
            padding: 10px;
        }

        #reset-section {
            text-align: center;
            margin-top: 20px;
        }

        #reset-button {
            display: inline-block;
            border: 2px solid white;
            border-radius: 5px;
            padding: 10px 20px;
            font-size: 20px;
            font-weight: 500;
            color: white;
            background-color: transparent;
            cursor: pointer;
            transition: background-color 0.2s, color 0.2s;
        }

        #reset-button:hover {
            background-color: white;
            color: black;
        }
    </style>
</head>
<body>
    <header>
        <h1>Tic Tac Toe</h1>
    </header>
    <div class="box">
        <!-- Your 3x3 grid with input fields (buttons) goes here -->
        <div class="row">
            <input type="button" class="btn" readonly>
            <input type="button" class="btn" readonly>
            <input type="button" class="btn" readonly>
        </div>
        <!-- Repeat the row div for the remaining rows -->
    </div>
    <div class="result-container">
        <p class="result">Current Player's Turn</p>
    </div>
    <div id="reset-section">
        <button id="reset-button">Reset</button>
    </div>
</body>
</html>