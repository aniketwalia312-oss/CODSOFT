# CODSOFT
                                          LEVEL-1
My third and final task is done as a web-developer intern at codsoft. throught out this time I feel the work teaches me a lot of things like dedication, hard work, perfect use of AI and all. The tasks are so fun and enjoyable too. I learnt many things like better coding, animation and theme selections, All of this make the summer internship very cool and productive.....
                                        
                                          QUESTION:
To create a basic calculator using CSS, HTML, and JavaScript, you'll need to implement an
interactive interface with buttons for addition, subtraction, multiplication, and division
operations. The calculator should have a display screen to show user input and results. Utilize
CSS grid system for button alignments. Use event listeners, if-else statements, operators, and
loops to handle user input and perform calculations. This project requires some skill but can be
done with basic knowledge of these technologies..

                                     TASK-3(CALCULATOR):
FILE: [index.html](https://github.com/user-attachments/files/28966370/index.html)

FILE FOR PHONE:  https://herocalculate.netlify.app/


CODE:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HeroCalc - The Action Figure & Comic Book Calculator</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Bangers&family=Orbitron:wght@500;700;900&family=Plus+Jakarta+Sans:wght@400;600;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body class="skin-spidey">
    <!-- Halftone Overlay Pattern -->
    <div class="halftone-overlay"></div>

    <div class="app-container">
        <!-- Header & Skin Selector -->
        <header class="app-header">
            <h1 class="logo-title">HERO<span class="highlight">CALC</span></h1>
            <div class="skin-selector-panel">
                <span class="selector-label">CHOOSE YOUR HERO:</span>
                <div class="skins-container">
                    <button class="skin-btn btn-spidey active" data-skin="spidey" title="Web-Slinger (Spider-Man)">
                        <span class="icon">🕸️</span> <span class="btn-text">SPIDEY</span>
                    </button>
                    <button class="skin-btn btn-batman" data-skin="batman" title="Dark Knight (Batman)">
                        <span class="icon">🦇</span> <span class="btn-text">BATMAN</span>
                    </button>
                    <button class="skin-btn btn-ironman" data-skin="ironman" title="Arc Avenger (Iron Man)">
                        <span class="icon">🚀</span> <span class="btn-text">IRON MAN</span>
                    </button>
                    <button class="skin-btn btn-hulk" data-skin="hulk" title="Gamma Monster (Hulk)">
                        <span class="icon">☣️</span> <span class="btn-text">HULK</span>
                    </button>
                </div>
            </div>
            <!-- Settings controls -->
            <div class="quick-settings">
                <button id="toggle-sound" class="settings-btn active" title="Toggle Sound FX">
                    <span class="icon">🔊</span>
                </button>
                <button id="toggle-voice" class="settings-btn" title="Toggle Voice Readout">
                    <span class="icon">🗣️</span>
                </button>
            </div>
        </header>

        <!-- Main Dashboard Grid -->
        <main class="dashboard-grid">
            
            <!-- LEFT PANEL: Battle History Log -->
            <aside class="panel history-panel">
                <h2 class="panel-heading">BATTLE LOG</h2>
                <div class="panel-content history-list-container">
                    <ul id="history-list" class="history-list">
                        <!-- Populated dynamically -->
                        <li class="empty-history">No missions recorded yet...</li>
                    </ul>
                </div>
                <div class="panel-footer">
                    <button id="clear-history" class="action-btn text-btn">WIPE LOGS</button>
                </div>
            </aside>

            <!-- CENTER PANEL: The Main Comic Calculator -->
            <section class="panel calculator-panel">
                <div class="calculator-container">
                    <!-- Calculator Display -->
                    <div class="calc-display-wrapper">
                        <div class="calc-screen-indicator">
                            <span class="hero-name-indicator">ACTIVE HERO: SPIDEY</span>
                            <span class="mode-indicator">SYSTEM: READY</span>
                        </div>
                        <div id="calc-expression" class="calc-expression"></div>
                        <div id="calc-output" class="calc-output">0</div>
                    </div>

                    <!-- Comic pop-up text container (inside the calc panel for relative placement) -->
                    <div id="popups-container" class="popups-container"></div>

                    <!-- Calculator Keyboard Grid -->
                    <div class="calc-keyboard">
                        <!-- Row 1: Actions -->
                        <button class="btn btn-action" data-action="clear">C</button>
                        <button class="btn btn-action" data-action="backspace">⌫</button>
                        <button class="btn btn-scientific" data-val="sqrt">√</button>
                        <button class="btn btn-op" data-val="/">÷</button>

                        <!-- Row 2: Sci / Numbers -->
                        <button class="btn btn-scientific" data-val="^">xʸ</button>
                        <button class="btn btn-num" data-val="7">7</button>
                        <button class="btn btn-num" data-val="8">8</button>
                        <button class="btn btn-num" data-val="9">9</button>
                        <button class="btn btn-op" data-val="*">×</button>

                        <!-- Row 3: Sci / Numbers -->
                        <button class="btn btn-scientific" data-val="sin">sin</button>
                        <button class="btn btn-num" data-val="4">4</button>
                        <button class="btn btn-num" data-val="5">5</button>
                        <button class="btn btn-num" data-val="6">6</button>
                        <button class="btn btn-op" data-val="-">−</button>

                        <!-- Row 4: Sci / Numbers -->
                        <button class="btn btn-scientific" data-val="cos">cos</button>
                        <button class="btn btn-num" data-val="1">1</button>
                        <button class="btn btn-num" data-val="2">2</button>
                        <button class="btn btn-num" data-val="3">3</button>
                        <button class="btn btn-op" data-val="+">+</button>

                        <!-- Row 5: Scientific, Zero, Dot, Equal -->
                        <button class="btn btn-scientific" data-val="tan">tan</button>
                        <button class="btn btn-num" data-val="0">0</button>
                        <button class="btn btn-num" data-val=".">.</button>
                        <button class="btn btn-scientific" data-val="log">log</button>
                        <button class="btn btn-equal" data-action="calculate">=</button>
                    </div>
                </div>
            </section>

            <!-- RIGHT PANEL: Utilities (Graph HUD & Stats Converter) -->
            <aside class="right-column">
                
                <!-- TOP RIGHT: Graphing Visualizer HUD -->
                <div class="panel visualizer-panel">
                    <h2 class="panel-heading">TACTICAL RADAR (GRAPH)</h2>
                    <div class="panel-content radar-content">
                        <div class="hud-canvas-container">
                            <canvas id="hud-radar-canvas" width="260" height="200"></canvas>
                            <div class="hud-grid-overlay"></div>
                            <div class="hud-crosshair"></div>
                        </div>
                        <div class="graph-input-group">
                            <span class="y-label">y = </span>
                            <input type="text" id="graph-equation" class="graph-input" placeholder="x^2 or sin(x)" value="sin(x)">
                            <button id="btn-plot" class="action-btn plot-btn">PLOT</button>
                        </div>
                    </div>
                </div>

                <!-- BOTTOM RIGHT: Arsenal Converter (Unit Converter) -->
                <div class="panel converter-panel">
                    <h2 class="panel-heading">ARSENAL CONVERTER</h2>
                    <div class="panel-content converter-content">
                        <div class="converter-type-selector">
                            <button class="conv-tab active" data-type="distance">DISTANCE</button>
                            <button class="conv-tab" data-type="force">FORCE/WT</button>
                            <button class="conv-tab" data-type="energy">TEMP</button>
                        </div>
                        
                        <div class="converter-fields">
                            <div class="input-field">
                                <label for="conv-input" id="lbl-conv-input">From Value</label>
                                <input type="number" id="conv-input" class="conv-input-box" value="1">
                                <select id="conv-from" class="conv-select"></select>
                            </div>
                            
                            <div class="conv-direction">⇄</div>
                            
                            <div class="input-field">
                                <label for="conv-output" id="lbl-conv-output">Result</label>
                                <input type="text" id="conv-output" class="conv-input-box" readonly value="0">
                                <select id="conv-to" class="conv-select"></select>
                            </div>
                        </div>
                    </div>
                </div>

            </aside>

        </main>
    </div>

    <!-- Scripts -->
    <script src="script.js"></script>
</body>
</html>
