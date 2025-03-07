<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono&display=swap" rel="stylesheet">
    <style>
        body {
        background-color: black;
        margin: 0;
        font-family: Arial, sans-serif;
        }
        section header {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 100%;
        }
        section header p {
        color: white;
        border-radius: 5px;
        text-transform: uppercase;
        font-size: 1.5em;
        font-weight: bold;
        font-family: 'JetBrains Mono', monospace;
        }
        .contributions_container {
        background-color: #333;
        display: grid;
        grid-template-columns: 2fr 1fr;
        padding: 10px;
        border-radius: 10px;
        box-shadow: inset 0 0 15px rgb(0, 0, 0);
        margin: auto;
        max-width: 900px;
        }
        .contributions_list {
        color: white;
        }
        .contributions_list a {
        color: #00ff00;
        font-family: Consolas, Courier, monospace;
        font-size: 1.1em;
        text-decoration: none;
        display: block;
        margin: 10px 15px;
        }
        .contributions_list a:hover {
        color: lightgreen;
        text-decoration: underline;
        }
        .contributions_list p{
            font-size: 0.8em; 
            font-style: italic;
        }
        .contributions_container img {
        width: 100%;
        max-width: 180px;
        height: auto;
        }
        .contributions_image{
            display: flex;
            grid-row: 1;
            grid-column: 2;
            justify-content: center;
            align-self: center;
            transform: scale(1);  
            transition: transform 0.2s ease-in-out;
        }
        .contributions_image:hover{
            transform: scale(1.1);  
            transition: transform 0.2s ease-in-out;
        } 
        @media (max-width: 768px) {
        .contributions_container {
            grid-template-columns: 1fr;
        }
        .contributions_list{
            text-align: center;
        }
        .contributions_image{
            grid-row: 2;
            grid-column: 1;
        }
        .contributions_list {
            margin: 3mm 0;
        }
        .contributions_container img {
            width: 90%;
            max-width: 150px;
            transition: opacity 0.5s ease-in-out;
        }
    }
    </style>
</head>
<body>

<section id="contributions">
<header>
<p>Recent contributions</p>
</header>

<div class="contributions_container">
<div class="contributions_list">
<a href="https://github.com/as-mi/site-cariere-nou">
Cariere v14 Web Application
<p>Full-Stack Development @ ASMI</p>
</a>

<a href="https://gitlab.com/users/nitronlp/project">
NitroNLP Competition Platform
<p>Front-End Development @ NitroNLP</p>
</a>

<a href="https://github.com/vlaxcs/FMI-INFO-S15-2024-2027">
Olympics' Class Materials
<p>Fueling academic excellence @ FMI.UNIBUC.RO</p>
</a>
</div>

<div class="contributions_image">
<img src="./res/action.gif" alt="Action">
</div>
</div>
</section>

</body>
</html>
