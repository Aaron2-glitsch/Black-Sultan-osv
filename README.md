<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Black Sultan OS - Vollautonomes KI-Metaversum</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --sultan-black: #0a0a0a;
            --sultan-gold: #FFD700;
            --sultan-purple: #6A0DAD;
            --cyber-blue: #00F7FF;
            --matrix-green: #00FF41;
            --construction-orange: #FF8C00;
            --education-blue: #1E90FF;
            --health-green: #32CD32;
            --accessibility-teal: #20B2AA;
            --ai-pink: #FF10F0;
            --neural-red: #FF3131;
            --quantum-blue: #5D3FD3;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            scroll-behavior: smooth;
        }
        
        body {
            background-color: var(--sultan-black);
            color: white;
            line-height: 1.6;
            overflow-x: hidden;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(106, 13, 173, 0.1) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(0, 247, 255, 0.1) 0%, transparent 20%),
                linear-gradient(to bottom, transparent, var(--sultan-black));
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        
        body.high-contrast {
            background-color: #000;
            color: #FFF;
            --sultan-gold: #FF0;
            --cyber-blue: #0FF;
            --matrix-green: #0F0;
            --sultan-purple: #F0F;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background: linear-gradient(90deg, rgba(10, 10, 10, 0.7), rgba(106, 13, 173, 0.7));
            padding: 15px 0;
            border-bottom: 2px solid var(--sultan-gold);
            position: sticky;
            top: 0;
            z-index: 100;
            backdrop-filter: blur(10px);
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 24px;
            font-weight: bold;
            background: linear-gradient(90deg, var(--sultan-gold), var(--cyber-blue));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            position: relative;
        }
        
        nav a:hover, nav a.active {
            color: var(--sultan-gold);
        }

        nav a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 50%;
            transform: translateX(-50%);
            background-color: var(--sultan-gold);
            transition: width 0.3s ease-in-out;
        }
        
        nav a:hover::after, nav a.active::after {
            width: 100%;
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(45deg, var(--sultan-purple), var(--sultan-gold));
            color: white;
            padding: 14px 35px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
            border: none;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(106, 13, 173, 0.4);
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 60px;
            color: var(--sultan-gold);
        }

        /* Bot-Kommando Simulator Sektion */
        .simulator-section {
            padding: 80px 0;
            text-align: center;
        }
        
        .command-simulator {
            max-width: 600px;
            margin: 0 auto;
            background: rgba(30, 30, 50, 0.7);
            padding: 30px;
            border-radius: 20px;
            border: 1px solid var(--sultan-purple);
        }
        
        .command-input {
            width: 100%;
            background: rgba(10, 10, 20, 0.8);
            border: 1px solid var(--cyber-blue);
            border-radius: 8px;
            padding: 15px;
            color: white;
            margin-bottom: 20px;
            font-family: 'Courier New', monospace;
        }
        
        .command-output {
            background: rgba(0, 0, 0, 0.5);
            border-radius: 8px;
            padding: 20px;
            min-height: 100px;
            text-align: left;
            margin-top: 20px;
            font-family: 'Courier New', monospace;
            color: var(--matrix-green);
        }
        
        footer {
            text-align: center;
            padding: 40px 20px;
            margin-top: 60px;
            border-top: 1px solid var(--sultan-gold);
        }
    </style>
</head>
<body>

    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo"><i class="fas fa-crown"></i> Black Sultan OS</div>
                <nav>
                    <ul>
                        <li><a href="#features">Features</a></li>
                        <li><a href="#bots">KI-Bots</a></li>
                        <li><a href="#demo">Demo</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <main>
        <section class="hero" style="padding: 80px 0; text-align: center;">
            <div class="container">
                <h1>Das vollautonome KI-Metaversum</h1>
                <p style="font-size: 1.2rem; max-width: 700px; margin: 20px auto 40px;">Eine revolutionäre Plattform, die 19 spezialisierte KI-Bots vereint, um deine Realität zu transformieren.</p>
                <a href="#demo" class="cta-button">Live-Demo starten</a>
            </div>
        </section>

        <section id="features" style="padding: 80px 0;">
            <div class="container">
                <h2 class="section-title">Kernfeatures</h2>
                </div>
        </section>

        <section id="bots" style="padding: 80px 0; background: rgba(20, 10, 30, 0.8);">
            <div class="container">
                <h2 class="section-title">Die 19 KI-Bots</h2>
                </div>
        </section>
        
        <section class="simulator-section" id="demo">
            <div class="container">
                <h2 class="section-title">Bot-Kommando Simulator</h2>
                <div class="command-simulator">
                    <input type="text" class="command-input" placeholder="Befehl eingeben (z.B. 'Analysiere Markttrends')">
                    <button class="cta-button" id="executeBtn">Befehl ausführen</button>
                    <div class="command-output" id="commandOutput">
                        <p>> System bereit. Befehl eingeben zum Starten.</p>
                    </div>
                </div>
            </div>
        </section>
    </main>
    
    <footer>
        <div class="container">
            <p>&copy; 2025 Black Sultan OS. Dein digitales Vermächtnis.</p>
        </div>
    </footer>

    <script>
        // Bot-Kommando Simulator Logik
        const commandInput = document.querySelector('.command-input');
        const commandOutput = document.getElementById('commandOutput');
        const executeButton = document.getElementById('executeBtn');
        
        const botResponses = {
            "default": "Befehl verstanden. Führe Analyse aus... Ergebnis: Positiver Trend im Sektor Quanten-Computing.",
            "status": "Systemstatus: Alle 19 Bots sind online. Hive-Mind-Verbindung stabil. Effizienz: 99.98%.",
            "hallo": "Hallo, Schöpfer. System bereit für deine Anweisungen.",
            "hilfe": "Mögliche Befehle: 'status', 'analysiere markttrends', 'hallo'.",
            "analysiere markttrends": "Marktanalyse gestartet... Höchstes Potential in den Bereichen Bio-Integration und dezentrale Netzwerke."
        };

        function executeCommand() {
            const command = commandInput.value.trim().toLowerCase();
            if (command === '') return;

            let output = `<p style="color: white;">> ${commandInput.value}</p>`;
            let response = botResponses[command] || botResponses["default"];
            output += `<p>${response}</p>`;
            
            commandOutput.innerHTML += output;
            commandOutput.scrollTop = commandOutput.scrollHeight; // Auto-scroll
            commandInput.value = '';
        }

        executeButton.addEventListener('click', executeCommand);
        commandInput.addEventListener('keypress', function(e) {
            if (e.key === 'Enter') {
                executeCommand();
            }
        });
    </script>

</body>
</html>

