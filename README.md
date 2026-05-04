<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>El Cuento de los Superpoderes Ocultos</title>
    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            background: linear-gradient(135deg, #0a3d62, #f39c12);
            color: white;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            padding: 10px;
        }
        .container {
            max-width: 600px;
            width: 100%;
            padding: 20px;
        }
        h1 {
            font-size: 24px;
        }
        .card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 15px;
            margin-top: 20px;
            display: none;
            animation: fadeIn 1s ease;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            border: none;
            border-radius: 10px;
            background: #f39c12;
            color: white;
            font-size: 14px;
            cursor: pointer;
            width: 100%;
        }
        button:hover {
            background: #e67e22;
        }
        @keyframes fadeIn {
            from {opacity: 0; transform: translateY(20px);}
            to {opacity: 1; transform: translateY(0);}
        }
        #contador {
            font-size: 16px;
            margin-top: 10px;
        }
        /* Confeti */
        .confeti {
            position: fixed;
            width: 10px;
            height: 10px;
            background: red;
            top: -10px;
            animation: caer 3s linear forwards;
        }
        @keyframes caer {
            to {
                transform: translateY(100vh) rotate(360deg);
            }
        }
        img {
            max-width: 100%;
            height: auto;
            margin: 10px 0;
            border-radius: 10px;
        }
        .mensaje-birthday {
            background: rgba(255, 255, 255, 0.2);
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
        }
    </style>
</head>

<body>

<div class="container">
    <!-- Mensaje de cumpleaños -->
    <div id="mensajeBirthday">
        <div class="mensaje-birthday">
            <h2>¡Feliz cumpleaños, Jesús Esteban! 🎂✨</h2>
            <p>
                Aunque estés lejos, hoy te mandamos un regalo especial…<br>
                tu propio cuento de Los Superpoderes Ocultos 🦸‍♂️💥<br>
                Sí, así como lo lees: un cuento hecho solo para ti, porque tú tienes poderes que ni tú mismo has descubierto todavía.<br><br>
                Pero antes de que lo leas, déjanos decirte algo:<br><br>
                Aquí seguimos celebrándote como si fueras una estrella internacional…<br>
                porque en esta familia eres más famoso que los superhéroes de Marvel 😎🌟.<br><br>
                Te mandamos un abrazo tan grande que, si tuviera GPS, ya estaríamos llegando a la tienda.<br>
                Y si no llega… ya sabes, es culpa del WiFi 😂📡.<br><br>
                Deseamos que este nuevo año te traiga risas, aventuras, sueños cumplidos<br>
                y muchas historias nuevas para seguir alimentando tus superpoderes.<br>
                Que cada día encuentres algo que te haga sonreír, aprender y crecer.<br><br>
                Aunque la distancia sea grande,<br>
                nuestro cariño por ti es más grande todavía 💙🚀.<br><br>
                Ahora sí…<br>
                prepárate, porque tu cuento de superpoderes ocultos te está esperando.<br>
                Y recuerda: los héroes como tú nacen para cosas grandes.<br><br>
                Att. Los Mazatlecos
            </p>
        </div>
        <button onclick="iniciarCuento()">Inicia el viaje</button>
    </div>

    <!-- Cuento -->
    <div id="cuento" style="display: none;">
        <h1>🎉 El Cuento de los Superpoderes Ocultos 🎉</h1>
        <h2>JESÚS ESTEBAN</h2>
        <div id="contador"></div>

        <!-- CAPÍTULO 1 -->
        <div class="card" id="sec1">
            <h3>Capítulo 2013: El nacimiento del héroe</h3>
            <p>
                El 4 de mayo de 2013 nació un héroe… aunque nadie lo sabía todavía 👶✨.<br><br>
                Fue un día especial, porque llegó al mundo Jesús Esteban, con una misión secreta:
                descubrir sus superpoderes… y causar unas cuantas risas en el camino 😄🦸‍♂️.<br><br>
                Ese día el universo dijo: "¡Prepárense, que este niño viene con energía!" 🌟🚀.
            </p>
            <div style="position: relative; width: 100%; height: 0; padding-top: 103.1733%;
            padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
            border-radius: 8px; will-change: transform;">
                <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
                    src="https://www.canva.com/design/DAHItn6zdJY/K_RCnBDVQyRNLH_5zXpYRQ/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
                </iframe>
            </div>
        </div>

        <!-- CAPÍTULO 2 -->
        <div class="card" id="sec2">
            <h3>✨ Capítulo 2015: Los primeros poderes</h3>
            <p>
                Desde pequeño comenzó a descubrir habilidades que parecían mágicas.<br><br>
                Primero dio sus pasos 👣✨… luego corrió detrás de sus sueños como si el piso fuera un trampolín 🏃‍♂️💨😄.<br><br>
                Aprendió a jugar, a imaginar mundos nuevos y a crear aventuras sin límites (a veces demasiado creativas para los adultos 🤯🎨).<br><br>
                Su primer superpoder fue simple pero poderoso: la imaginación infinita 🌈🪄… capaz de convertir cualquier día normal en una misión épica.
            </p>
            <div style="position: relative; width: 100%; height: 0; padding-top: 103.1733%;
            padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
            border-radius: 8px; will-change: transform;">
                <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
                    src="https://www.canva.com/design/DAG6uAz_VlM/1Vhne33S76mtcVpOGIM3Tg/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
                </iframe>
            </div>
        </div>

        <!-- CAPÍTULO 3 -->
        <div class="card" id="sec3">
            <h3>🔍 Capítulo 2018: Curiosidad infinita</h3>
            <p>
                En 2018 desbloqueó uno de sus poderes más importantes: la curiosidad.<br><br>
                Quería entenderlo todo: cómo funcionan las cosas, por qué pasa lo que pasa, qué hay más allá… y más allá del más allá 🤔💡.<br><br>
                Exploraba, preguntaba, investigaba… su mente era un radar de descubrimientos 👀✨ que nunca se apagaba.<br><br>
                Ese año aprendió que quien pregunta, crece; y quien explora, encuentra 🌎💡… aunque a veces encontrara cosas que nadie buscaba 😂.
            </p>
            <div style="position: relative; width: 100%; height: 0; padding-top: 103.1733%;
            padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
            border-radius: 8px; will-change: transform;">
                <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
                    src="https://www.canva.com/design/DAHItn5xNl8/unS75YJsABVvMvLZCiv7CQ/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
                </iframe>
            </div>
        </div>

        <!-- CAPÍTULO 4 -->
        <div class="card" id="sec4">
            <h3>⚡ Capítulo 2020: Energía imparable</h3>
            <p>
                Su energía se volvió un motor que nunca se apagaba (ni con "ya siéntate tantito" 🤣).<br><br>
                Saltaba, corría, jugaba, inventaba… siempre en movimiento 🤸‍♂️🔥, como si tuviera baterías infinitas.<br><br>
                Descubrió su pasión por el deporte: el esfuerzo, la disciplina y la emoción del juego.<br><br>
                Ese año entendió que la energía no solo se siente… se usa para avanzar 🏅⚡… y también para cansar a todos los demás.
            </p>
            <div style="position: relative; width: 100%; height: 0; padding-top: 103.1733%;
            padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
            border-radius: 8px; will-change: transform;">
                <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
                    src="https://www.canva.com/design/DAHIt1kUvWI/YJZwVtjv3rCj44ETU5T-PQ/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
                </iframe>
            </div>
        </div>

        <!-- CAPÍTULO 5 -->
        <div class="card" id="sec5">
            <h3>🎮 Capítulo 2023: El poder de la estrategia</h3>
            <p>
                En 2023 desarrolló un superpoder nuevo: la estrategia.<br><br>
                Los videojuegos 🎮 le enseñaron a pensar rápido, tomar decisiones inteligentes y analizar cada movimiento (como mini-genio táctico 🧠⚡).<br><br>
                El fútbol ⚽ le mostró el trabajo en equipo, la precisión y la visión del juego.<br><br>
                Combinó ambos mundos y se convirtió en un estratega brillante: mente rápida, acción segura 🧠🎯… y celebraciones épicas cuando ganaba 😎🔥.
            </p>
            <div style="position: relative; width: 100%; height: 0; padding-top: 103.1733%;
            padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
            border-radius: 8px; will-change: transform;">
                <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
                    src="https://www.canva.com/design/DAHIt132ihU/AObkX-aiHVJqCCbwWMyCbg/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
                </iframe>
            </div>
        </div>

        <!-- CAPÍTULO 6 -->
        <div class="card" id="sec6">
            <h3>🎉 Capítulo 2026: Hoy</h3>
            <p>
                Hoy cumple 13 años… y ya no es solo un niño.<br><br>
                Es un joven con historia, con fuerza, con sueños y con muchos superpoderes 🌟💫 (algunos todavía en modo secreto).<br><br>
                Hoy celebramos no solo su cumpleaños… celebramos todo lo que es y todo lo que será 🎉🎂✨… porque este nivel apenas empieza.
            </p>
            <div style="position: relative; width: 100%; height: 0; padding-top: 103.1733%;
            padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
            border-radius: 8px; will-change: transform;">
                <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
                    src="https://www.canva.com/design/DAHIty7cVCA/MKijmMleHSatqe0jSJ5oNA/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
                </iframe>
            </div>
        </div>

        <!-- CAPÍTULO 7 -->
        <div class="card" id="sec7">
            <h3>🔮 Capítulo 2027: El futuro lo escribes tú</h3>
            <p>
                Lo que viene no está escrito… pero seguro será emocionante.<br><br>
                Cada decisión, cada sueño, cada paso será parte de su propia historia.<br><br>
                Tiene los poderes, la energía, la curiosidad y la estrategia.<br><br>
                Ahora solo falta lo más importante: atreverse a crear su futuro 🚀🌈📖… y hacerlo tan épico que hasta el universo aplauda.
            </p>
            <div style="position: relative; width: 100%; height: 0; padding-top: 103.1733%;
            padding-bottom: 0; box-shadow: 0 2px 8px 0 rgba(63,69,81,0.16); margin-top: 1.6em; margin-bottom: 0.9em; overflow: hidden;
            border-radius: 8px; will-change: transform;">
                <iframe loading="lazy" style="position: absolute; width: 100%; height: 100%; top: 0; left: 0; border: none; padding: 0;margin: 0;"
                    src="https://www.canva.com/design/DAHIt38Mhzs/41sDAAm6phXH5prGw1lBQQ/view?embed" allowfullscreen="allowfullscreen" allow="fullscreen">
                </iframe>
            </div>
        </div>

        <div id="final" style="display: none;">
            <h3>FIN</h3>
            <button onclick="reiniciar()">VOLVER A EMPEZAR</button>
        </div>

        <button id="continuarBtn" onclick="siguiente()">Continuar</button>
    </div>

<script>
    let actual = 1;
    document.getElementById("sec1").style.display = "block";
    actualizarContador();

    function iniciarCuento() {
        document.getElementById("mensajeBirthday").style.display = "none";
        document.getElementById("cuento").style.display = "block";
    }

    function siguiente() {
        document.getElementById("sec" + actual).style.display = "none";
        actual++;

        if (actual <= 7) {
            document.getElementById("sec" + actual).style.display = "block";
            actualizarContador();
        } else {
            document.getElementById("continuarBtn").style.display = "none";
            document.getElementById("final").style.display = "block";
            lanzarConfeti();
        }
    }

    function actualizarContador() {
        const fechas = [
            new Date(2013, 4, 4), // Capítulo 1
            new Date(2015, 4, 4), // Capítulo 2
            new Date(2018, 3, 4), // Capítulo 3
            new Date(2020, 3, 4), // Capítulo 4
            new Date(2023, 3, 4), // Capítulo 5
            new Date(2026, 4, 4), // Capítulo 6
            new Date(2027, 3, 4)  // Capítulo 7
        ];

        const diasDesdeNacimiento = Math.floor((new Date() - fechas[actual - 1]) / (1000 * 60 * 60 * 24));
        document.getElementById("contador").innerText = `La magia de este capítulo vive desde hace ${diasDesdeNacimiento} días`;
    }

    function reiniciar() {
        actual = 1;
        document.getElementById("continuarBtn").style.display = "block";
        document.getElementById("final").style.display = "none";
        for (let i = 1; i <= 7; i++) {
            document.getElementById("sec" + i).style.display = "none";
        }
        document.getElementById("sec1").style.display = "block";
        actualizarContador();
    }

    function lanzarConfeti() {
        for (let i = 0; i < 120; i++) {
            let c = document.createElement("div");
            c.classList.add("confeti");
            c.style.left = Math.random() * 100 + "vw";
            c.style.backgroundColor = randomColor();
            c.style.animationDuration = (Math.random() * 3 + 2) + "s";
            document.body.appendChild(c);
            setTimeout(() => c.remove(), 5000);
        }
    }

    function randomColor() {
        const colores = ["#f39c12", "#3498db", "#e74c3c", "#2ecc71"];
        return colores[Math.floor(Math.random() * colores.length)];
    }
</script>

</body>
</html>
