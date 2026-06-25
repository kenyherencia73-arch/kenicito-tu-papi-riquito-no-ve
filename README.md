# kenicito-tu-papi-riquito-no-ve
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Burros para Burros 🐴</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Comic+Neue:wght@400;700&family=Press+Start+2P&display=swap');
        
        body {
            margin: 0;
            background: linear-gradient(135deg, #f4a261, #e76f51, #f4a261);
            font-family: 'Comic Neue', cursive;
            color: #264653;
            text-align: center;
            background-size: 400% 400%;
            animation: gradient 15s ease infinite;
        }

        @keyframes gradient {
            0% {background-position: 0% 50%;}
            50% {background-position: 100% 50%;}
            100% {background-position: 0% 50%;}
        }

        header {
            background: #2a9d8f;
            padding: 2rem 1rem;
            color: white;
            text-shadow: 0 4px 0 #1f7a6e;
        }

        h1 {
            font-size: 4rem;
            margin: 0;
        }

        .hero {
            font-size: 8rem;
            margin: 30px 0;
            animation: rebuzno 1.5s infinite;
        }

        @keyframes rebuzno {
            0%, 100% { transform: rotate(-8deg) scale(1); }
            50% { transform: rotate(8deg) scale(1.1); }
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
        }

        .card {
            background: white;
            border: 6px solid #264653;
            border-radius: 25px;
            padding: 25px;
            margin: 15px;
            width: 280px;
            display: inline-block;
            box-shadow: 0 10px 0 #1f7a6e;
        }

        button {
            background: #e76f51;
            color: white;
            border: none;
            padding: 18px 40px;
            font-size: 1.8rem;
            border-radius: 50px;
            cursor: pointer;
            box-shadow: 0 10px 0 #c15a42;
            transition: all 0.1s;
            font-family: 'Press Start 2P', cursive;
        }

        button:active {
            transform: translateY(6px);
            box-shadow: 0 4px 0 #c15a42;
        }

        .footer {
            background: #264653;
            color: #f4a261;
            padding: 3rem 1rem;
            margin-top: 4rem;
            font-size: 1.3rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>🐴 BURROS PARA BURROS 🐴</h1>
        <p style="font-size:2rem; margin:10px;">¡La web más terca de internet!</p>
    </header>

    <div class="container">
        <div class="hero">🦓</div>
        
        <h2 style="font-size:2.5rem;">¿Eres un burro de verdad?</h2>
        
        <div style="display:flex; flex-wrap:wrap; justify-content:center; gap:20px;">
            <div class="card">
                <h3>🐴 Características del burro perfecto</h3>
                <ul style="text-align:left; font-size:1.3rem;">
                    <li>✅ Terco nivel experto</li>
                    <li>✅ Le gusta el pasto</li>
                    <li>✅ Rebuzna cuando le da la gana</li>
                    <li>✅ Inteligente pero nadie lo cree</li>
                </ul>
            </div>
            <div class="card">
                <h3>🧠 Datos burros</h3>
                <p>Los burros tienen mejor memoria que los elefantes.<br>
                Pueden reconocer a sus amigos después de años.</p>
            </div>
        </div>

        <button onclick="rebuznar()">¡REBUZNA FUERTE!</button>
    </div>

    <div class="footer">
        <p>© 2026 Sindicato Nacional de Burros • Todos los derechos rebuznados</p>
        <p>Si llegaste hasta aquí... definitivamente eres uno de los nuestros 🐴</p>
    </div>

    <script>
        function rebuznar() {
            const rebuznos = [
                "¡IIIIII-AHHHHHHHH! 🐴",
                "¡REEEEEEEEEE-BUZZZZZZZ!",
                "¡SOY UN BURRO Y ME VALE MADRE!",
                "¡MÁS PASTO, HIJOS DE PUTA!",
                "¡I-A! ¡I-A! ¡I-A!"
            ];
            
            const random = rebuznos[Math.floor(Math.random() * rebuznos.length)];
            alert(random);
            
            document.querySelector('.hero').style.fontSize = '10rem';
            setTimeout(() => {
                document.querySelector('.hero').style.fontSize = '8rem';
            }, 200);
        }
    </script>
</body>
</html>
