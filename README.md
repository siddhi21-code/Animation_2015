# Animation_2015
Animation use HTML ,CSS , JAVASCRIPT
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Computer Animation</title>
    <style>
        .computer {
            width: 200px;
            height: 150px;
            border: 2px solid black;
            border-radius: 10px;
            background-color: #f0f0f0;
            position: relative;
        }
        
        .screen {
            width: 180px;
            height: 120px;
            border: 1px solid black;
            background-color: #ffffff;
            position: absolute;
            top: 15px;
            left: 10px;
            padding: 10px;
            font-family: monospace;
            font-size: 14px;
            white-space: pre;
        }
        
        .code {
            position: absolute;
            top: 10px;
            left: 10px;
            animation: coding 5s infinite;
        }
        
        @keyframes coding {
            0% {
                content: "HTML";
            }
            20% {
                content: "HTML\nCSS";
            }
            40% {
                content: "HTML\nCSS\nJavaScript";
            }
            60% {
                content: "HTML\nCSS\nJavaScript\nReact";
            }
            80% {
                content: "HTML\nCSS\nJavaScript\nReact\nNode.js";
            }
            100% {
                content: "HTML\nCSS\nJavaScript\nReact\nNode.js\n...";
            }
        }
        
        .code::before {
            content: "";
            animation: blink 1s infinite;
        }
        
        @keyframes blink {
            0% {
                opacity: 1;
            }
            50% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <div class="computer">
        <div class="screen">
            <span class="code"></span>
        </div>
    </div>
</body>
</html>

