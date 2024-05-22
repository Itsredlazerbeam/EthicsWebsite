# EthicsWebsite
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eiffel Tower</title>
    <style>
        body {
            background: linear-gradient(0deg, #ffffff 0%, #f2d2a9 100%);
            background-image: url('https://wallpapers.com/images/hd/paris-aesthetic-yi5146ugao47ztms.jpg');
            background-size: cover;
            background-position: center;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        .center {
            display: block;
            margin-left: auto;
            margin-right: auto;
        }
        .left {
            text-align: left;
            margin-left: 20px;
            width: 100%;
        }
        pRed {
            color: red;
        }
        .image-shadow {
            box-shadow: 5px 5px 18px 0px #f2d2a9, 5px 5px 10px 1px #000000;
        }
        .animate-image {
            animation: revealImage 2s ease-out forwards;
            clip-path: polygon(0 0, 100% 0, 100% 0, 0 0);
        }
        @keyframes revealImage {
            to {
                clip-path: polygon(0 0, 100% 0, 100% 100%, 0 100%);
            }
        }
        .topLeft {
            position: absolute;
            top: 50px;
            left: 50px;
            padding: 10px;
        }
        .dropdown-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 1s ease-out;
            text-align: left;
            margin: 20px auto;
            border: 1px solid #000;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 5px;
            width: 40%;
            max-width: 800px;border-radius: 5px;
        }
        .dropdown-content p {
            margin: 5px 0;
        }
        .show {
            max-height: 200px; /* Adjust as needed based on content */
        }
        h4 {
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>La Tour Eiffel</h1>
    <h2>Paris, France</h2>
    <h3>Constructed 1887-1889</h3>
    <pRed>Did you know there are 1665 steps on the Eiffel Tower?</pRed>
    <p class="topLeft">This Website is Open Source! <br> <a href="https://github.com/SkellXC/EthicsWebsite"> Contribute here<a></p>

    <h4 onclick="toggleDropdown()"><u>Laws</u></h4>
    <div id="dropdown" class="dropdown-content" onclick="toggleDropdown()">
        <p><a href="dataProtectionAct.html">The Data Protection Act 1998</a></p>
        <p><a href="ComputerMisuseAct.html">The Computer Misuse Act 1990</a></p>
        <p><a href ="copyrightLegislationAndControl.html" >The Copyright Design And Patents Act 1988</a></p>
        <p>The Regulation of Investigatory Powers Act 2000</p>
    </div>

    <h5>Ethics</h5>

    <script>
        function toggleDropdown() {
            var dropdown = document.getElementById("dropdown");
            dropdown.classList.toggle("show");
        }
    </script>
</body>
</html>
