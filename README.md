<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>STAR STRIKE</title>
        <style>
            html, body {
                margin: 0;
                width: 100%;
                height: 100%;
                background: white;
            }

            body {
                display: flex;
                justify-content: center;
                align-items: center;
            }

            canvas {
                display: block;
                border-radius: 20px;
                touch-action: none;
            }
        </style>
    </head>
    <body>
        <canvas id="canvas"></canvas>
        <script>
            const canvas = document.getElementById("canvas");
            const ctx = canvas.getContext("2d");
            const GAME_RATIO = 9/19.5;
            canvas.height = window.innerHeight;
            canvas.width = canvas.height*GAME_RATIO;
            window.onload = () => {
                ctx.font = "50px Sans-serif";
                ctx.textAlign = "center";
                ctx.textBaseline = "middle";
                ctx.fillStyle = "black";
                ctx.fillText(canvas.height,canvas.width/2,canvas.height/2);
            };
        </script>
    </body>
</html>
