<!-- Violentómetro Psicológico — versión glassy, pastel premium, SVG minimalista y animación fluida -->
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Violentómetro Psicológico — Glassy</title>
    <style>
        :root {
            --bg-1: #f6f3ff;
            --card: #ffffffcc;
            --glass-border: rgba(255, 255, 255, 0.6);
            --shadow: 0 8px 24px rgba(46, 32, 89, 0.08);
            --accent-1: #6ad4cd; /* nivel 1 */
            --accent-2: #b57acb; /* nivel 2 */
            --accent-3: #ff7a85; /* nivel 3 */
            --accent-4: #ffcc00; /* nivel 4 - amarillo */
            --muted: #6b5b82;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
            background: radial-gradient(1200px 600px at 10% 10%, #f4efff 0%, #fbfbff 35%, #f6fbff 100%);
            color: var(--muted);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 28px;
        }

        .container {
            width: 100%;
            max-width: 1100px;
            background: linear-gradient(180deg, rgba(255, 255, 255, 0.85), rgba(255, 255, 255, 0.72));
            border-radius: 20px;
            border: 1px solid var(--glass-border);
            box-shadow: var(--shadow);
            padding: 22px;
            backdrop-filter: blur(6px) saturate(120%);
        }

        .header {
            display: flex;
            align-items: flex-start;
            gap: 18px;
            margin-bottom: 14px;
        }

        .brand {
            background: linear-gradient(90deg, #6a3fb4, #b565d3);
            color: white;
            padding: 10px 14px;
            border-radius: 12px;
            font-weight: 700;
            box-shadow: 0 6px 18px rgba(110, 64, 164, 0.18);
        }

        .title-wrap {
            flex: 1;
        }

        .title {
            font-size: 1.35rem;
            color: #3b2158;
            font-weight: 800;
        }

        .subtitle {
            font-size: 0.92rem;
            color: #6d5d8f;
            margin-top: 6px;
        }

        .layout {
            display: grid;
            grid-template-columns: 1fr 380px 1fr;
            gap: 20px;
            align-items: start;
        }

        .col {
            background: rgba(255, 255, 255, 0.6);
            border-radius: 14px;
            padding: 14px;
            border: 1px solid rgba(215, 210, 255, 0.55);
            box-shadow: 0 8px 20px rgba(87, 63, 150, 0.06);
        }

        .col .h {
            font-weight: 700;
            margin-bottom: 8px;
            color: #3b2a58;
        }

        .chips {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 8px 0;
        }

        .chip {
            background: rgba(255, 255, 255, 0.8);
            padding: 6px 10px;
            border-radius: 999px;
            font-size: 0.82rem;
            border: 1px solid rgba(200, 190, 255, 0.6);
        }

        .quote {
            font-style: italic;
            margin-top: 10px;
            color: #5b486f;
        }

        /* Thermometer column */
        .thermo-wrap {
            display: flex;
            gap: 22px;
            align-items: center;
            justify-content: center;
        }

        .levels {
            display: flex;
            flex-direction: column;
            gap: 0; /* Eliminado espacio entre niveles */
            height: 520px;
            justify-content: space-between;
            width: 100%;
        }

        .level-card {
            border-radius: 12px;
            padding: 12px;
            background: linear-gradient(180deg, rgba(255, 255, 255, 0.6), rgba(255, 255, 255, 0.45));
            border: 1px solid rgba(200, 190, 255, 0.5);
            box-shadow: 0 6px 18px rgba(82, 60, 145, 0.06);
            display: flex;
            gap: 12px;
            align-items: flex-start;
        }

        .level-card h4 {
            margin: 0;
            font-size: 0.98rem;
        }

        .level-card p {
            margin: 6px 0 0 0;
            color: #6d5d8f;
            font-size: 0.9rem;
        }

        .level-1 { border-left: 6px solid var(--accent-1); }
        .level-2 { border-left: 6px solid var(--accent-2); }
        .level-3 { border-left: 6px solid var(--accent-3); }
        .level-4 { border-left: 6px solid var(--accent-4); }

        /* Thermometer visual — classic bulb */
        .thermo {
            width: 110px;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 12px;
            height: 520px;
            justify-content: center;
        }

        .thermo-shell {
            position: relative;
            width: 40px;
            height: 360px;
            border-radius: 30px;
            background: linear-gradient(180deg, #fff 0%, #f3f3ff 100%);
            border: 1px solid rgba(120, 100, 160, 0.12);
            box-shadow: inset 0 6px 18px rgba(255, 255, 255, 0.6), 0 6px 18px rgba(75, 50, 120, 0.06);
            overflow: hidden;
        }

       .thermo-bulb {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    margin-top: 8px;
    background: #F5E9D3; /* beige pastel */
    border: 1px solid rgba(160, 140, 110, 0.18);
    box-shadow: 0 12px 28px rgba(240, 200, 150, 0.18);
}


        /* Fill layers — segmented to match levels */
        .fill {
            position: absolute;
            left: 0;
            right: 0;
            bottom: 0;
            height: 0;
            display: flex;
            flex-direction: column;
        }

        .fill > .seg {
            flex: 1;
            width: 100%;
        }

        .seg1 { background: linear-gradient(180deg, var(--accent-1), rgba(90, 200, 190, 0.9)); }
        .seg2 { background: linear-gradient(180deg, var(--accent-2), rgba(180, 120, 200, 0.9)); }
        .seg3 { background: linear-gradient(180deg, var(--accent-3), rgba(255, 110, 130, 0.95)); }
        .seg4 { background: linear-gradient(180deg, var(--accent-4), rgba(255, 200, 100, 0.95)); }

        /* Smooth animation to reveal segments sequentially */
        .fill.animate {
            animation: rise 3.2s cubic-bezier(.2, .9, .2, 1) forwards;
        }

        @keyframes rise {
            0% { height: 0%; }
            33% { height: 33.34%; }
            66% { height: 66.67%; }
            100% { height: 100%; }
        }

        /* Icons (SVG) */
        .icon {
            width: 36px;
            height: 36px;
            display: inline-block;
        }

        .icon svg {
            width: 100%;
            height: 100%;
            display: block;
        }

        /* Responsive */
        @media (max-width: 980px) {
            .layout {
                grid-template-columns: 1fr;
            }
            .thermo {
                order: 2;
                margin: 16px 0;
            }
            .levels {
                order: 1;
                height: auto;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="brand">VIOLENTÓMETRO</div>
            <div class="title-wrap">
                <div class="title">Identifica la violencia psicológica</div>
                <div class="subtitle">Herramienta visual para reconocer señales y actuar a tiempo</div>
            </div>
        </div>

        <div class="layout">

            <!-- Columna izquierda: señales -->
            <div class="col">
                <div class="h">👁️ Señales que puedes estar normalizando</div>
                <div class="chips">
                    <div class="chip">Bromas hirientes</div>
                    <div class="chip">Sarcasmo constante</div>
                    <div class="chip">Minimizar emociones</div>
                    <div class="chip">Celos disfrazados</div>
                </div>
                <div class="quote">“La violencia incluye el uso intencional de la fuerza o del poder —amenazado o real— que puede causar daño psicológico” (Organización Mundial de la Salud, 2002).
</div>
            </div>

            <!-- Centro: niveles + termómetro -->
            <div class="thermo-wrap">

                <!-- Niveles a la izquierda, alineados -->
                <div class="levels">
                    <div class="level-card level-1">
                        <div class="icon" aria-hidden>
                            <!-- SVG minimalista: corazón -->
                            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M12 21s-7-4.5-9-8.5C0 7.5 4 4 7 6c1 1 2 2 5 5 3-3 4-4 5-5 3-2-7 1.5-8 6.5C19 16.5 12 21 12 21z" stroke="#2f4858" stroke-width="0.8" opacity="0.9"/>
                            </svg>
                        </div>
                        <div>
                            <h4>💜 Nivel 1 · Advertencia leve</h4>
                            <p>Comentarios que parecen broma, minimizar lo que sientes, correcciones constantes.</p>
                        </div>
                    </div>

                    <div class="level-card level-2">
                        <div class="icon" aria-hidden>
                            <!-- SVG minimalista: corazón roto -->
                            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M12 21s-4.5-3.5-7-7C1.5 9.5 4 5.5 7.5 7c1.5.6 2.5 1.6 4.5 3.5 2-2 3-2.9 4.5-3.5C20 5.5 22.5 9.5 19 14c-2.5 3.5-7 7-7 7z" stroke="#3b2a58" stroke-width="0.8"/>
                            </svg>
                        </div>
                        <div>
                            <h4>💔 Nivel 2 · Desgaste emocional</h4>
                            <p>Culparte por su estado anímico, controlar amistades, alternar cariño con frialdad.</p>
                        </div>
                    </div>

                    <div class="level-card level-3">
                        <div class="icon" aria-hidden>
                            <!-- SVG minimalista: triángulo de alerta -->
                            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M12 3l9 16H3L12 3z" stroke="#3b2a58" stroke-width="0.9" fill="none"/>
                                <path d="M12 9v6" stroke="#3b2a58" stroke-width="1"/>
                                <circle cx="12" cy="18" r="0.6" fill="#3b2a58"/>
                            </svg>
                        </div>
                        <div>
                            <h4>🚨 Nivel 3 · Alto riesgo</h4>
                            <p>Insultos, humillaciones, aislamiento social, amenazas y conducta peligrosa.</p>
                        </div>
                    </div>

                    <div class="level-card level-4">
                        <div class="icon" aria-hidden>
                            <!-- SVG minimalista: signo de peligro círculo -->
                            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M12 21s-4.5-3.5-7-7C1.5 9.5 4 5.5 7.5 7c1.5.6 2.5 1.6 4.5 3.5 2-2 3-2.9 4.5-3.5C20 5.5 22.5 9.5 19 14c-2.5 3.5-7 7-7 7z" stroke="#3b2a58" stroke-width="0.8"/>
                            </svg>
                        </div>
                        <div>
                            <h4>⛔ Nivel 4 · Crítico extremo</h4>
                            <p>Busca ayuda ahora: riesgo de daño grave, amenazas de muerte, aislamiento total o inducir al suicidio.</p>
                        </div>
                    </div>
                </div>

                <!-- Termómetro clásico a la derecha -->
                <div class="thermo">
                    <div class="thermo-shell" role="img" aria-label="Termómetro de niveles">
                        <div class="fill animate">
                            <div class="seg seg4"></div>
                            <div class="seg seg3"></div>
                            <div class="seg seg2"></div>
                            <div class="seg seg1"></div>
                        </div>
                    </div>
                    <div class="thermo-bulb"></div>
                </div>

            </div>

            <!-- Columna derecha: acciones y efectos -->
            <div class="col">
                <div class="h">📌 Efectos en tu bienestar</div>
                <p style="color: #6d5d8f;">Baja autoestima, ansiedad, aislamiento, fatiga emocional y riesgo de trastornos mentales.</p>
                <div style="height: 18px;"></div>
                <div class="h">🛟 ¿Qué puedes hacer?</div>
                <ul style="margin: 8px 0 0 18px; color: #6d5d8f;">
                    <li>Habla con alguien de confianza.</li>
                    <li>Establece límites claros y consistentes.</li>
                    <li>Busca asesoría profesional si es necesario.</li>
                    <li>Aléjate si tu seguridad está en riesgo.</li>
                </ul>
            </div>

        </div>

       <p style="text-align: left; margin-top: 16px; color: #8a789d; font-size: 0.85rem; padding-left: 20px; text-indent: -20px; line-height: 1.4;">
<strong>Referencias:</strong><br>
<span style="display:block; padding-left:20px; text-indent:-20px;">Gobierno de México, Ciencia y Tecnología, UNRC. (2025). <em>Contenido nuclear: Perspectiva de género para el diseño social — Módulo 2: Género y sociedad</em> [Material de curso]. Plataforma Universidad Nacional Rosario Castellanos. https://www.plataforma.unrc.edu.mx/pluginfile.php/8970/mod_resource/content/7/TRIPEG_Contenido_Nuclear%20UNRC%20%281%29.pdf</span>
<span style="display:block; padding-left:20px; text-indent:-20px;">Organización Mundial de la Salud. (2002). <em>World report on violence and health</em>. https://www.who.int/violence_injury_prevention/violence/world_report/en/</span>
</p>
    </div>
</body>
</html>
