<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Confession to Yna</title>
    <style>
        /* Background styling */
        body {
            font-family: 'Poppins', sans-serif;
            background-color: white; /* White background */
            color: pink; /* Default text color set to pink */
            text-align: center;
            padding: 50px;
        }

        /* Font styling */
        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 50px;
            color: pink; /* Pink color for h1 */
        }

        p {
            font-size: 22px;
            margin-bottom: 20px;
            color: pink; /* Pink color for paragraph */
        }

        input[type="text"] {
            padding: 10px;
            font-size: 18px;
            border: 2px solid pink; /* Pink border */
            border-radius: 5px;
            background-color: rgba(255, 255, 255, 0.7);
            color: pink; /* Pink text inside input */
        }

        button {
            padding: 10px 20px;
            font-size: 20px;
            background-color: pink; /* Pink background for button */
            border: none;
            border-radius: 5px;
            color: white;
            cursor: pointer;
        }

        button:hover {
            background-color: #ff3385; /* Darker pink on hover */
        }

        /* Styling for messages */
        #confession, #goodbye {
            display: none;
            font-size: 24px;
            margin-top: 30px;
            font-weight: bold;
        }

        #confession {
            color: pink; /* Pink color for confession */
        }

        #goodbye {
            color: pink; /* Pink color for goodbye */
        }

        /* Responsive styling */
        @media (max-width: 768px) {
            h1 {
                font-size: 35px;
            }

            p {
                font-size: 18px;
            }

            input[type="text"] {
                font-size: 16px;
            }

            button {
                font-size: 18px;
            }

            #confession, #goodbye {
                font-size: 20px;
            }
        }

    </style>
    <!-- Adding Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&family=Poppins:wght@300&display=swap" rel="stylesheet">
</head>
<body>

    <h1>Hi Yna!</h1>
    <p>There's something special I want to share with you. Please respond with <strong>yes</strong> or <strong>no</strong> if you want to proceed.</p>
    
    <label for="response">Please response: </label>
    <input type="text" id="response" placeholder="yes/no">
    <button onclick="showConfession()">Submit</button>

    <p id="confession"> Happy valentines Yna. Maamin na ako kan feelings ko saimo. Gusto taka mayo nang iba. Happy Valentine's againn.</p>
    <p id="goodbye">Thank you sa seen.</p>

    <script>
        function showConfession() {
            var response = document.getElementById("response").value.toLowerCase();
            
            if (response === "yes") {
                document.getElementById("confession").style.display = "block";
                document.getElementById("goodbye").style.display = "none";
            } else if (response === "no") {
                document.getElementById("confession").style.display = "none";
                document.getElementById("goodbye").style.display = "block";
            } else {
                alert("Please type 'yes' or 'no'.");
            }
        }
    </script>

</body>
</html>
