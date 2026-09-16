
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CODEX BELLATOR - ARS UNIFIED | Ciencia de Combate Unificado</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        gold: {
                            50: '#fffbeb',
                            100: '#fef3c7',
                            400: '#fbbf24',
                            500: '#f59e0b',
                            600: '#d97706',
                            700: '#b45309',
                        },
                        amberGold: '#d4af37',
                        tactical: {
                            900: '#0b0f19',
                            800: '#111827',
                            700: '#1f2937',
                            600: '#374151',
                            accent: '#f59e0b',
                            cyan: '#06b6d4',
                            red: '#ef4444'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace']
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0b0f19;
            color: #f3f4f6;
        }
        .glow-amber {
            box-shadow: 0 0 25px -5px rgba(245, 158, 11, 0.3);
        }
        .glow-cyan {
            box-shadow: 0 0 25px -5px rgba(6, 182, 212, 0.3);
        }
        .border-gradient {
            border-image: linear-gradient(to right, #f59e0b, #06b6d4) 1;
        }
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0b0f19;
        }
        ::-webkit-scrollbar-thumb {
            background: #374151;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #f59e0b;
        }
    </style>
</head>
<body class="bg-tactical-900 text-gray-100 antialiased selection:bg-amber-500 selection:text-black overflow-x-hidden">

    <!-- Sticky Navigation Header -->
    <header class="sticky top-0 z-50 bg-tactical-900/90 backdrop-blur-md border-b border-tactical-700/60 transition-all">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-9 h-9 rounded-lg bg-gradient-to-br from-amber-500 to-amber-700 flex items-center justify-center text-black font-black text-lg group-hover:scale-105 transition-transform">
                    <i class="fa-solid fa-shield-halved"></i>
                </div>
                <div>
                    <span class="font-bold tracking-wider text-sm sm:text-base text-gray-100 block leading-none">CODEX BELLATOR</span>
                    <span class="text-xs text-amber-500 font-mono tracking-widest block leading-tight">ARS UNIFIED</span>
                </div>
            </a>

            <!-- Quick Navigation Links -->
            <nav class="hidden lg:flex items-center gap-6 text-xs font-semibold tracking-wider uppercase text-gray-300">
                <a href="#que-es" class="hover:text-amber-400 transition-colors">¿Qué es?</a>
                <a href="#para-que-sirve" class="hover:text-amber-400 transition-colors">¿Para qué sirve?</a>
                <a href="#objetivo" class="hover:text-amber-400 transition-colors">Objetivo</a>
                <a href="#como-funciona" class="hover:text-amber-400 transition-colors">Funcionamiento</a>
                <a href="#realmente-funciona" class="hover:text-amber-400 transition-colors">Evidencia</a>
                <a href="#diferencias" class="hover:text-amber-400 transition-colors">Comparativa</a>
                <a href="#cualidades" class="hover:text-amber-400 transition-colors">Cualidades</a>
            </nav>

            <div class="flex items-center gap-3">
                <a href="#conocer" class="px-4 py-2 text-xs font-bold uppercase tracking-wider bg-amber-500 text-black rounded-lg hover:bg-amber-400 transition-all shadow-lg shadow-amber-500/20 flex items-center gap-2">
                    <i class="fa-solid fa-book-bookmark"></i>
                    <span class="hidden sm:inline">Explorar Codex</span>
                </a>
                <button id="mobile-menu-btn" class="lg:hidden p-2 text-gray-400 hover:text-white">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Mobile dropdown menu -->
        <div id="mobile-menu" class="hidden lg:hidden bg-tactical-800 border-b border-tactical-700 px-4 py-4 space-y-3 text-sm">
            <a href="#que-es" class="block text-gray-300 hover:text-amber-400 font-medium">¿Qué es el Codex?</a>
            <a href="#para-que-sirve" class="block text-gray-300 hover:text-amber-400 font-medium">¿Para qué sirve?</a>
            <a href="#objetivo" class="block text-gray-300 hover:text-amber-400 font-medium">¿Cuál es su objetivo?</a>
            <a href="#como-funciona" class="block text-gray-300 hover:text-amber-400 font-medium">¿Cómo funciona?</a>
            <a href="#realmente-funciona" class="block text-gray-300 hover:text-amber-400 font-medium">¿Realmente funciona?</a>
            <a href="#diferencias" class="block text-gray-300 hover:text-amber-400 font-medium">Diferencias Metodológicas</a>
            <a href="#cualidades" class="block text-gray-300 hover:text-amber-400 font-medium">Cualidades Distintivas</a>
        </div>
    </header>

    <!-- MAIN BLOGGER HERO HEADER BLOCK -->
    <section class="relative pt-12 pb-16 px-4 sm:px-6 lg:px-8 max-w-5xl mx-auto text-center" id="conocer">
        <div class="absolute inset-0 -z-10 bg-[radial-gradient(ellipse_at_top,_var(--tw-gradient-stops))] from-amber-500/10 via-tactical-900/60 to-transparent"></div>
        
        <!-- Hero Box Frame -->
        <div class="border-2 border-amber-500/80 bg-tactical-800/90 rounded-2xl p-6 sm:p-10 md:p-12 shadow-2xl glow-amber relative overflow-hidden backdrop-blur-sm">
            <div class="absolute top-0 right-0 w-32 h-32 bg-amber-500/10 rounded-full blur-2xl pointer-events-none"></div>
            <div class="absolute bottom-0 left-0 w-32 h-32 bg-cyan-500/10 rounded-full blur-2xl pointer-events-none"></div>

            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-amber-500/10 border border-amber-500/30 text-amber-400 text-xs font-mono mb-6">
                <span class="w-2 h-2 rounded-full bg-amber-400 animate-pulse"></span>
                Marco de Validación Doctrinal | C.C.U.
            </div>

            <h1 class="text-3xl sm:text-5xl md:text-6xl font-black tracking-tight text-white uppercase mb-3 leading-tight">
                CODEX BELLATOR
            </h1>
            <h2 class="text-xl sm:text-2xl md:text-3xl font-extrabold text-amber-400 tracking-wider uppercase mb-4 font-mono leading-tight">
                ARS UNIFIED
            </h2>
            <p class="text-lg sm:text-xl text-gray-300 font-medium mb-8 max-w-2xl mx-auto">
                Ciencia de Combate Unificado
            </p>

            <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                <a href="#que-es" class="w-full sm:w-auto px-8 py-4 bg-amber-500 hover:bg-amber-400 text-black font-black uppercase tracking-widest text-sm rounded-xl transition-all shadow-xl hover:scale-105 flex items-center justify-center gap-3">
                    <span>[ CONOCER EL CODEX ]</span>
                    <i class="fa-solid fa-arrow-down"></i>
                </a>
            </div>

            <div class="mt-8 pt-6 border-t border-tactical-700/80 flex flex-wrap justify-center gap-4 text-xs text-gray-400 font-mono">
                <span><i class="fa-solid fa-shield text-amber-500 mr-1"></i>Arquitectura Metodológica Canónica</span>
                <span>•</span>
                <span><i class="fa-solid fa-code-branch text-amber-500 mr-1"></i>Doctrina Versión 4.0 (Sistémica Avanzada)</span>
                <span>•</span>
                <span><i class="fa-solid fa-microchip text-amber-500 mr-1"></i>P.A.O. v6.0 & S.M.V.</span>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl animate-bounce">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 1: ¿QUÉ ES EL CODEX BELLATOR ARS UNIFIED? -->
    <section id="que-es" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    1
                </div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                    ¿QUÉ ES EL CODEX BELLATOR ARS UNIFIED?
                </h2>
            </div>

            <div class="prose prose-invert max-w-none text-gray-300 text-base sm:text-lg leading-relaxed space-y-6">
                <p class="font-medium text-amber-200/90 text-lg sm:text-xl border-l-4 border-amber-500 pl-4 py-1">
                    El <strong>Codex Bellator – Ars Unified</strong> es la <strong>Ciencia de Combate Unificado (C.C.U.)</strong>: un sistema cerrado de alta ingeniería humana, neurofisiología aplicada, biomecánica y telemetría biológica concebido para eliminar la entropía metodológica y la improvisación en las artes marciales y deportes de contacto.
                </p>

                <p>
                    A diferencia del entrenamiento tradicional basado en la acumulación ciega de fatiga muscular y dogmas históricos, el Codex concibe el combate como un <strong>proceso dinámico de control de lazo cerrado</strong>. Su fin es transformar al atleta en un operador capaz de anular la latencia reactiva del oponente y ejecutar intercepciones en <strong>Tiempo Cero ($T0$)</strong>.
                </p>

                <!-- 3 Levels of Abstraction Grid -->
                <div class="mt-8 grid grid-cols-1 md:grid-cols-3 gap-4 pt-4">
                    <div class="bg-tactical-900/80 p-5 rounded-xl border border-tactical-700 hover:border-amber-500/50 transition-colors">
                        <div class="text-amber-500 font-mono text-xs uppercase font-bold mb-1">Nivel 1 • Límite Constitucional</div>
                        <h3 class="text-lg font-bold text-white mb-2"><i class="fa-solid fa-gavel text-amber-500 mr-2"></i>La Regla</h3>
                        <p class="text-xs text-gray-400">Establece el límite biomecánico e inmutable que garantiza la seguridad del chasis y la pureza del engrama motor del combatiente. Define el <em>"qué debe cumplirse"</em>.</p>
                    </div>

                    <div class="bg-tactical-900/80 p-5 rounded-xl border border-tactical-700 hover:border-cyan-500/50 transition-colors">
                        <div class="text-cyan-400 font-mono text-xs uppercase font-bold mb-1">Nivel 2 • Telemetría</div>
                        <h3 class="text-lg font-bold text-white mb-2"><i class="fa-solid fa-table text-cyan-400 mr-2"></i>La Plantilla</h3>
                        <p class="text-xs text-gray-400">Receptáculo físico estructurado donde se registran metadatos y telemetría biológica del atleta, desterrando notas libres y subjetividades. Define el <em>"dónde se registra"</em>.</p>
                    </div>

                    <div class="bg-tactical-900/80 p-5 rounded-xl border border-tactical-700 hover:border-amber-500/50 transition-colors">
                        <div class="text-amber-500 font-mono text-xs uppercase font-bold mb-1">Nivel 3 • Hoja de Ruta Algorítmica</div>
                        <h3 class="text-lg font-bold text-white mb-2"><i class="fa-solid fa-diagram-project text-amber-500 mr-2"></i>El P.A.O.</h3>
                        <p class="text-xs text-gray-400">Protocolo de Aplicación Operativa: guía procedimental paso a paso que instruye al operador sobre cómo rellenar plantillas y aplicar reglas sin sesgo. Define el <em>"cómo se procede"</em>.</p>
                    </div>
                </div>

                <!-- Principle of Flow Continuity callout -->
                <div class="bg-amber-500/10 border border-amber-500/30 rounded-xl p-5 mt-6">
                    <h4 class="text-amber-400 font-bold uppercase text-sm flex items-center gap-2 mb-2">
                        <i class="fa-solid fa-arrows-spin text-lg"></i>
                        Principio Rector Supremo: Regla de Continuidad de Flujo
                    </h4>
                    <p class="text-xs sm:text-sm text-gray-300">
                        La famosa expresión <code class="bg-tactical-900 px-2 py-0.5 rounded text-amber-300 font-mono">A+D+A = 1</code> constituye un modelo paradigmático de integración temporal y funcional (Ataque + Defensa + Continuidad sin bloques independientes), y <strong>NO una secuencia fija u obligatoria</strong>. En el Codex, toda retracción o transición de masa es la defensa activa y la precarga bioeléctrica del siguiente ataque, erradicando los tiempos muertos.
                    </p>
                </div>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 2: ¿PARA QUÉ SIRVE? -->
    <section id="para-que-sirve" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    2
                </div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                    ¿PARA QUÉ SIRVE?
                </h2>
            </div>

            <p class="text-gray-300 text-base sm:text-lg mb-8 leading-relaxed">
                El Codex Bellator sirve como una <strong>plataforma de soberanía y optimización biomecánica integral</strong>. Sus aplicaciones abarcan desde la preparación física de alta precisión hasta el combate real en todas las distancias.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <!-- Card 1 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-amber-500/40 transition-all flex gap-4">
                    <div class="text-amber-500 text-2xl shrink-0">
                        <i class="fa-solid fa-stopwatch-20"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Anulación de Latencia Reactiva (Tiempo Cero)</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Permite al peleador detectar las microseñales biomecánicas del oponente antes de que su golpe madure, disparando el vector de intercepción en la génesis ($FF1$) e invalidando el tiempo de respuesta convencional (~200ms).
                        </p>
                    </div>
                </div>

                <!-- Card 2 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-cyan-500/40 transition-all flex gap-4">
                    <div class="text-cyan-400 text-2xl shrink-0">
                        <i class="fa-solid fa-shield-virus"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Protección del Chasis y Prevención de Lesiones</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Mediante el <strong>Umbral de Velocidad Crítica (UVC 10%)</strong> y el protocolo de Chasis Seguro, aborta de forma automática las series cuando la velocidad cae, erradicando el "volumen basura" que degrada las articulaciones y corrompe el engrama.
                        </p>
                    </div>
                </div>

                <!-- Card 3 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-amber-500/40 transition-all flex gap-4">
                    <div class="text-amber-500 text-2xl shrink-0">
                        <i class="fa-solid fa-person-ripping"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Unificación Striking & Grappling / Suelo</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Aplica de manera idéntica en combate de pie y combate de agarre (Judo, Lucha, BJJ). Rige la presión gravitacional cohesiva ($PFM-2$) y las cuñas mecánicas ($PFM-3$) para neutralizar barridos y derribos sin perder la plomada.
                        </p>
                    </div>
                </div>

                <!-- Card 4 -->
                <div class="bg-tactical-900/90 p-6 rounded-xl border border-tactical-700/80 hover:border-cyan-500/40 transition-all flex gap-4">
                    <div class="text-cyan-400 text-2xl shrink-0">
                        <i class="fa-solid fa-chart-line"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-white mb-2">Auditoría Cuantitativa Transparente</h3>
                        <p class="text-xs sm:text-sm text-gray-400 leading-relaxed">
                            Proporciona a entrenadores y atletas indicadores matemáticos inexpugnables ($IGD$, $I.I.S.$, $I.P.F.$) para evaluar la frescura neural y tomar decisiones adaptativas con el algoritmo <strong>IA-P1</strong>.
                        </p>
                    </div>
                </div>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 3: ¿CUÁL ES SU OBJETIVO? -->
    <section id="objetivo" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl relative overflow-hidden">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    3
                </div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                    ¿CUÁL ES SU OBJETIVO?
                </h2>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-6 items-center">
                <div class="lg:col-span-2 space-y-4 text-gray-300 text-base leading-relaxed">
                    <p class="text-lg font-semibold text-white">
                        La finalidad suprema perseguida por la Ciencia de Combate Unificado es alcanzar la <span class="text-amber-400 underline decoration-amber-500/50">Soberanía Neural y la Inevitabilidad Táctica</span> en la contienda.
                    </p>
                    <p>
                        El objetivo no es simplemente ganar un asalto mediante desgaste aleatorio, sino <strong>dominar el espacio-tiempo de la pelea (Kairós)</strong>, erradicando la duda, la vacilación y los tiempos muertos a través de las 5 dimensiones del engrama motor subcortical (Estado de Integración $EI-5$).
                    </p>
                    <ul class="space-y-2 text-xs sm:text-sm font-mono text-gray-300 pt-2">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-500"></i> Desatar el reclutamiento voluntario instantáneo de Fibras Rápidas Tipo IIa y IIx.</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-500"></i> Reprogramar las respuestas reactivas para ser procesadas en el cerebelo en silencio cognitivo.</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-amber-500"></i> Maximizar la rentabilidad biológica del entrenamiento mediante el Índice de Costo-Beneficio ($ICB$).</li>
                    </ul>
                </div>

                <!-- Goal Pillar Highlight Box -->
                <div class="bg-gradient-to-br from-amber-500/20 to-tactical-900 border border-amber-500/40 p-6 rounded-xl text-center glow-amber">
                    <i class="fa-solid fa-bullseye text-4xl text-amber-400 mb-3 block"></i>
                    <h3 class="font-black text-white text-lg uppercase tracking-wider mb-2">Meta Final</h3>
                    <p class="text-xs text-amber-200/80 leading-relaxed font-mono">
                        "Convertir la respuesta defensiva y ofensiva en una sola vibración cinemática indivisible en Tiempo Cero (Lin Sil Die Dar)."
                    </p>
                </div>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 4: ¿CÓMO FUNCIONA? -->
    <section id="como-funciona" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    4
                </div>
                <div>
                    <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                        ¿CÓMO FUNCIONA?
                    </h2>
                    <p class="text-xs text-amber-400 font-mono uppercase">Estructura algorítmica y arquitectura de lazo cerrado</p>
                </div>
            </div>

            <!-- Interactive Component Tabs -->
            <div class="mb-6 grid grid-cols-2 gap-2 border-b border-tactical-700 pb-4 sm:flex sm:flex-wrap">
                <button onclick="switchTab('vafp')" id="tab-vafp" class="tab-btn active whitespace-nowrap px-4 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-amber-500 text-black shadow-md">
                    1. Motor V.A.F.P.
                </button>
                <button onclick="switchTab('pfm')" id="tab-pfm" class="tab-btn whitespace-nowrap px-4 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-tactical-700 text-gray-300 hover:bg-tactical-600">
                    2. Leyes P.F.M.
                </button>
                <button onclick="switchTab('lazo')" id="tab-lazo" class="tab-btn whitespace-nowrap px-4 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-tactical-700 text-gray-300 hover:bg-tactical-600">
                    3. CNS & MCC
                </button>
                <button onclick="switchTab('fase0')" id="tab-fase0" class="tab-btn whitespace-nowrap px-4 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-tactical-700 text-gray-300 hover:bg-tactical-600">
                    4. Filtro Fase 0
                </button>
                <button onclick="switchTab('mdo')" id="tab-mdo" class="tab-btn whitespace-nowrap px-4 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-tactical-700 text-gray-300 hover:bg-tactical-600">
                    5. M.D.O. (9 Campos)
                </button>
                <button onclick="switchTab('paci')" id="tab-paci" class="tab-btn whitespace-nowrap px-4 py-2 rounded-lg text-xs font-bold uppercase transition-all bg-tactical-700 text-gray-300 hover:bg-tactical-600">
                    6. Protocolo P.A.C.I.
                </button>
            </div>

            <!-- Tab Content Containers -->
            <div id="tab-content" class="bg-tactical-900/90 rounded-xl p-6 border border-tactical-700/80 min-h-[300px]">
                
                <!-- V.A.F.P Content -->
                <div id="content-vafp" class="tab-pane space-y-4">
                    <div class="flex items-center justify-between border-b border-tactical-700 pb-3">
                        <h3 class="text-xl font-bold text-amber-400">Vector de Anticipación Fisiológica Proyectiva (V.A.F.P.)</h3>
                        <span class="text-xs font-mono bg-amber-500/20 text-amber-300 px-2 py-1 rounded">Motor Neuronal Principal</span>
                    </div>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Es la interfaz neurobiológica encargada de comprimir el tiempo de procesamiento y ejecutar intercepciones sin latencia reactiva ($T0$).
                    </p>
                    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-3 pt-2">
                        <div class="p-3 bg-tactical-800 rounded-lg border border-amber-500/30">
                            <div class="font-mono font-bold text-amber-400 text-sm">V • Vector</div>
                            <p class="text-xs text-gray-400 mt-1">Selección instantánea de la trayectoria de menor resistencia sin movimientos parásitos.</p>
                        </div>
                        <div class="p-3 bg-tactical-800 rounded-lg border border-amber-500/30">
                            <div class="font-mono font-bold text-amber-400 text-sm">A • Anticipación</div>
                            <p class="text-xs text-gray-400 mt-1">Escaneo automático subcortical de microseñales biomecánicas (hombro, fijación ocular).</p>
                        </div>
                        <div class="p-3 bg-tactical-800 rounded-lg border border-amber-500/30">
                            <div class="font-mono font-bold text-amber-400 text-sm">F • Focalización</div>
                            <p class="text-xs text-gray-400 mt-1">Silencio cognitivo y barrido de la duda; colapso neuromuscular coordinado.</p>
                        </div>
                        <div class="p-3 bg-tactical-800 rounded-lg border border-amber-500/30">
                            <div class="font-mono font-bold text-amber-400 text-sm">P • Proyección</div>
                            <p class="text-xs text-gray-400 mt-1">Materialización de la fuerza proyectada a través del eje enemigo sin desaceleración previa.</p>
                        </div>
                    </div>
                </div>

                <!-- P.F.M. Content -->
                <div id="content-pfm" class="tab-pane hidden space-y-4">
                    <div class="flex items-center justify-between border-b border-tactical-700 pb-3">
                        <h3 class="text-xl font-bold text-cyan-400">Principios Fundamentales del Movimiento (P.F.M.)</h3>
                        <span class="text-xs font-mono bg-cyan-500/20 text-cyan-300 px-2 py-1 rounded">Leyes Biomecánicas Inmutables</span>
                    </div>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Las 3 leyes físicas rectoras que gobiernan la geometría corporal tanto en Golpeo (Striking) como en Agarre/Suelo (Grappling/Lucha/BJJ):
                    </p>
                    <div class="space-y-3 pt-2">
                        <div class="p-4 bg-tactical-800 rounded-lg border border-tactical-700">
                            <div class="text-amber-400 font-bold text-sm font-mono">PFM-1: Eje Estructural</div>
                            <p class="text-xs text-gray-300 mt-1">Mantenimiento de la plomada vertical (cabeza-columna-cadera). En lucha/suelo opera como el pivote soberano que impide el colapso del centro de gravedad.</p>
                        </div>
                        <div class="p-4 bg-tactical-800 rounded-lg border border-tactical-700">
                            <div class="text-amber-400 font-bold text-sm font-mono">PFM-2: Transferencia de Masa Cohesiva</div>
                            <p class="text-xs text-gray-300 mt-1">Inercia unificada del chasis. En el tapiz se transmutación en presión gravitacional sin espacios intersticiales sobre el oponente.</p>
                        </div>
                        <div class="p-4 bg-tactical-800 rounded-lg border border-tactical-700">
                            <div class="text-amber-400 font-bold text-sm font-mono">PFM-3: Vectorización de Palancas y Cuñas</div>
                            <p class="text-xs text-gray-300 mt-1">Cambios angulares de fuerza perpendiculares a los límites articulares rivales y ocupación agresiva de líneas centrales con codos/rodillas.</p>
                        </div>
                    </div>
                </div>

                <!-- Lazo Cerrado Content -->
                <div id="content-lazo" class="tab-pane hidden space-y-4">
                    <div class="flex items-center justify-between border-b border-tactical-700 pb-3">
                        <h3 class="text-xl font-bold text-amber-400">C.N.S. & M.C.C. • Arquitectura de Control Dinámico</h3>
                        <span class="text-xs font-mono bg-amber-500/20 text-amber-300 px-2 py-1 rounded">Lazo Cerrado Desacoplado</span>
                    </div>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Ningún mecanismo ejecutor debe supervisarse a sí mismo. Por ello, el Codex separa la vigilancia de la ejecución:
                    </p>
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-2">
                        <div class="p-4 bg-tactical-800 rounded-lg border border-amber-500/30">
                            <h4 class="font-bold text-amber-400 text-sm mb-1"><i class="fa-solid fa-eye mr-2"></i>C.N.S. (Centro de Supervisión Neuronal)</h4>
                            <p class="text-xs text-gray-400">Módulo supervisor independiente. Vigila en segundo plano desviaciones mecánicas sin intervenir en el flujo voluntario.</p>
                        </div>
                        <div class="p-4 bg-tactical-800 rounded-lg border border-cyan-500/30">
                            <h4 class="font-bold text-cyan-400 text-sm mb-1"><i class="fa-solid fa-wrench mr-2"></i>M.C.C. (Mecanismo de Compensación Continua)</h4>
                            <p class="text-xs text-gray-400">Inyecta micro-ajustes reflejos en pleno vuelo (MCC-V, A, F o P) ante la señal del C.N.S., salvando la estructura antes del colapso.</p>
                        </div>
                    </div>
                </div>

                <!-- Fase 0 Content -->
                <div id="content-fase0" class="tab-pane hidden space-y-4">
                    <div class="flex items-center justify-between border-b border-tactical-700 pb-3">
                        <h3 class="text-xl font-bold text-cyan-400">Fase 0: Formulario de Viabilidad Doctrinal (Filtro de Ingesta)</h3>
                        <span class="text-xs font-mono bg-cyan-500/20 text-cyan-300 px-2 py-1 rounded">7 Preguntas de Control</span>
                    </div>
                    <p class="text-sm text-gray-300 leading-relaxed">
                        Cortafuegos obligatorio antes de invertir recursos en diseñar un drill. Evalúa si la idea es VIABLE o NO VIABLE:
                    </p>
                    <ol class="grid grid-cols-1 sm:grid-cols-2 gap-2 text-xs font-mono text-gray-300 pt-2">
                        <li class="p-2 bg-tactical-800 rounded border border-amber-500/30"><span class="text-amber-400 font-bold">1. Principio Mecánico (Gate #1):</span> ¿Respeta las leyes físicas de los P.F.M.?</li>
                        <li class="p-2 bg-tactical-800 rounded"><span class="text-amber-400 font-bold">2. Objetivo V.A.F.P.:</span> Propósito de aceleración/ anticipación.</li>
                        <li class="p-2 bg-tactical-800 rounded"><span class="text-amber-400 font-bold">3. Función:</span> Clasificación A-D de la A.F.E.</li>
                        <li class="p-2 bg-tactical-800 rounded"><span class="text-amber-400 font-bold">4. Adaptación:</span> Reclutamiento de Fibras IIa/IIx.</li>
                        <li class="p-2 bg-tactical-800 rounded"><span class="text-amber-400 font-bold">5. Datos:</span> F-Codes diagnosticables (F1-F4).</li>
                        <li class="p-2 bg-tactical-800 rounded"><span class="text-amber-400 font-bold">6. Medición:</span> Control por S.M.V. & 10% UVC.</li>
                        <li class="p-2 bg-tactical-800 rounded border border-cyan-500/30 sm:col-span-2"><span class="text-cyan-400 font-bold">7. Decisión & Optimización:</span> Reglas IA-P1 & ratio ICB.</li>
                    </ol>
                </div>

                <!-- MDO Content -->
                <div id="content-mdo" class="tab-pane hidden space-y-4">
                    <div class="flex items-center justify-between border-b border-tactical-700 pb-3">
                        <h3 class="text-xl font-bold text-amber-400">M.D.O. • Modelo de Diseño Operativo</h3>
                        <span class="text-xs font-mono bg-amber-500/20 text-amber-300 px-2 py-1 rounded">Ficha Técnica de 9 Campos</span>
                    </div>
                    <p class="text-sm text-gray-300">
                        Ningún ejercicio ingresa a la base de datos de las Series P sin completar estos 9 parámetros de ingeniería:
                    </p>
                    <div class="grid grid-cols-2 sm:grid-cols-3 gap-2 text-xs font-mono pt-2">
                        <div class="p-2 bg-tactical-800 rounded"><span class="text-amber-400">1.</span> Objetivo V.A.F.P.</div>
                        <div class="p-2 bg-tactical-800 rounded"><span class="text-amber-400">2.</span> Perturbación Inducida</div>
                        <div class="p-2 bg-tactical-800 rounded"><span class="text-amber-400">3.</span> Fallo Esperado (F1-F4)</div>
                        <div class="p-2 bg-tactical-800 rounded"><span class="text-amber-400">4.</span> Criterio de Éxito</div>
                        <div class="p-2 bg-tactical-800 rounded border border-amber-500/40"><span class="text-amber-400">5.</span> Intensidad (Caos I-V)*</div>
                        <div class="p-2 bg-tactical-800 rounded"><span class="text-amber-400">6.</span> Variabilidad Vectorial</div>
                        <div class="p-2 bg-tactical-800 rounded"><span class="text-amber-400">7.</span> Transferencia S.C.I.T.O.</div>
                        <div class="p-2 bg-tactical-800 rounded"><span class="text-amber-400">8.</span> Métrica Cuantitativa</div>
                        <div class="p-2 bg-tactical-800 rounded border border-cyan-500/40"><span class="text-cyan-400">9.</span> Principio Mecánico PFM</div>
                    </div>
                    <p class="text-xs text-amber-300/80 italic mt-2">
                        *Aclaración Doctrinal: La escala de Intensidad I al V mide el nivel de caos ambiental y sobrecarga cognitiva, NO el esfuerzo concéntrico muscular (el cual es SIEMPRE 100% máximo voluntario).
                    </p>
                </div>

                <!-- PACI Content -->
                <div id="content-paci" class="tab-pane hidden space-y-4">
                    <div class="flex items-center justify-between border-b border-tactical-700 pb-3">
                        <h3 class="text-xl font-bold text-cyan-400">Protocolo P.A.C.I. (Microciclo SCA-1 de 7 Días)</h3>
                        <span class="text-xs font-mono bg-cyan-500/20 text-cyan-300 px-2 py-1 rounded">Día 0 de Inicialización</span>
                    </div>
                    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-2 text-xs pt-2">
                        <div class="p-2 bg-tactical-800 rounded border-l-2 border-amber-500"><b class="text-amber-400">Día 1:</b> Potencia (Floor Press/ front squat)</div>
                        <div class="p-2 bg-tactical-800 rounded border-l-2 border-amber-500"><b class="text-amber-400">Día 2:</b> Reacción (TR estocástico ms)</div>
                        <div class="p-2 bg-tactical-800 rounded border-l-2 border-amber-500"><b class="text-amber-400">Día 3:</b> Cinética (Fugas rotacionales)</div>
                        <div class="p-2 bg-tactical-800 rounded border-l-2 border-amber-500"><b class="text-amber-400">Día 4:</b> Toma de Decisión (Ratio vacilación)</div>
                        <div class="p-2 bg-tactical-800 rounded border-l-2 border-cyan-500"><b class="text-cyan-400">Día 5:</b> Reactividad (Contacto muelle ms)</div>
                        <div class="p-2 bg-tactical-800 rounded border-l-2 border-cyan-500"><b class="text-cyan-400">Día 6:</b> Lazo Cerrado (Guardia ósea)</div>
                        <div class="p-2 bg-tactical-800 rounded border-l-2 border-cyan-500 sm:col-span-2"><b class="text-cyan-400">Día 7:</b> Auditoría S.M.V. (Cálculo IGD inicial & UVC)</div>
                    </div>
                </div>

            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 5: ¿REALMENTE FUNCIONA? -->
    <section id="realmente-funciona" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    5
                </div>
                <div>
                    <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                        ¿REALMENTE FUNCIONA?
                    </h2>
                    <p class="text-xs text-amber-400 font-mono uppercase">Evidencia, Neurofisiología y Criterios Matemáticos de Comprobación</p>
                </div>
            </div>

            <!-- Scientific Foundations Grid -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-8">
                <div class="p-5 bg-tactical-900 rounded-xl border border-tactical-700">
                    <div class="text-amber-500 font-bold text-sm mb-2"><i class="fa-solid fa-microscope mr-2"></i>Principio de Henneman</div>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Anula el reclutamiento lento mediante la <strong>Intención de Movimiento Absoluta y Rate Coding</strong>, forzando la activación inmediata de Fibras Rápidas Tipo IIa y IIx.
                    </p>
                </div>

                <div class="p-5 bg-tactical-900 rounded-xl border border-tactical-700">
                    <div class="text-cyan-400 font-bold text-sm mb-2"><i class="fa-solid fa-bolt mr-2"></i>PAP & Regla del 10% UVC</div>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Usa Potenciación Post-Activación y detiene la serie en el milisegundo en que la velocidad concéntrica cae un 10% (Umbral de Velocidad Crítica).
                    </p>
                </div>

                <div class="p-5 bg-tactical-900 rounded-xl border border-tactical-700">
                    <div class="text-amber-500 font-bold text-sm mb-2"><i class="fa-solid fa-bug mr-2"></i>Taxonomía F-Codes</div>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Clasifica errores: <b>F1 Vector</b> (contenido), <b>F2 Anticipación</b>, <b>F3 Focalización</b> (CATASTRÓFICO por desencadenar Cascada Sistémica), y <b>F4 Proyección</b>.
                    </p>
                </div>
            </div>

            <!-- INTERACTIVE SIMULATOR: IGD CALCULATOR & SOFTWARE VETO CLAUSE -->
            <div class="bg-tactical-900/90 rounded-2xl p-6 border border-amber-500/40 glow-amber">
                <div class="flex items-center justify-between border-b border-tactical-700 pb-3 mb-4">
                    <h3 class="font-bold text-white text-base sm:text-lg flex items-center gap-2">
                        <i class="fa-solid fa-calculator text-amber-400"></i>
                        Simulador S.M.V.: Calculador de IGD y Cláusula de Voto de Censura
                    </h3>
                    <span class="text-xs font-mono text-amber-400 bg-amber-500/10 px-2 py-1 rounded">Interactive Tool</span>
                </div>

                <p class="text-xs text-gray-400 mb-6">
                    Ajusta los niveles de cada dimensión para evaluar el Índice Global de Desarrollo ($IGD$). Observa cómo opera la <strong>Cláusula de Voto de Censura de Software</strong> si Técnica o Táctica caen por debajo de 5.0:
                </p>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                    <div class="space-y-4">
                        <!-- Slider 1 -->
                        <div>
                            <div class="flex justify-between text-xs font-mono mb-1">
                                <span class="text-gray-300">1. Hardware Físico (20%)</span>
                                <span id="val-hf" class="text-amber-400 font-bold">8.0</span>
                            </div>
                            <input type="range" id="input-hf" min="1" max="10" step="0.5" value="8" oninput="calculateIGD()" class="w-full accent-amber-500 bg-tactical-700 h-2 rounded-lg cursor-pointer">
                        </div>

                        <!-- Slider 2 -->
                        <div>
                            <div class="flex justify-between text-xs font-mono mb-1">
                                <span class="text-gray-300">2. Hardware Neural (20%)</span>
                                <span id="val-hn" class="text-amber-400 font-bold">8.0</span>
                            </div>
                            <input type="range" id="input-hn" min="1" max="10" step="0.5" value="8" oninput="calculateIGD()" class="w-full accent-amber-500 bg-tactical-700 h-2 rounded-lg cursor-pointer">
                        </div>

                        <!-- Slider 3 (Software) -->
                        <div class="bg-amber-500/10 p-2 rounded border border-amber-500/30">
                            <div class="flex justify-between text-xs font-mono mb-1">
                                <span class="text-amber-300 font-bold">3. Software Técnico (20%) *</span>
                                <span id="val-st" class="text-amber-400 font-bold">4.5</span>
                            </div>
                            <input type="range" id="input-st" min="1" max="10" step="0.5" value="4.5" oninput="calculateIGD()" class="w-full accent-amber-500 bg-tactical-700 h-2 rounded-lg cursor-pointer">
                        </div>

                        <!-- Slider 4 (Software) -->
                        <div class="bg-amber-500/10 p-2 rounded border border-amber-500/30">
                            <div class="flex justify-between text-xs font-mono mb-1">
                                <span class="text-amber-300 font-bold">4. Software Táctico (20%) *</span>
                                <span id="val-ste" class="text-amber-400 font-bold">7.0</span>
                            </div>
                            <input type="range" id="input-ste" min="1" max="10" step="0.5" value="7" oninput="calculateIGD()" class="w-full accent-amber-500 bg-tactical-700 h-2 rounded-lg cursor-pointer">
                        </div>

                        <!-- Slider 5 -->
                        <div>
                            <div class="flex justify-between text-xs font-mono mb-1">
                                <span class="text-gray-300">5. Gobierno Mental (20%)</span>
                                <span id="val-gm" class="text-amber-400 font-bold">8.0</span>
                            </div>
                            <input type="range" id="input-gm" min="1" max="10" step="0.5" value="8" oninput="calculateIGD()" class="w-full accent-amber-500 bg-tactical-700 h-2 rounded-lg cursor-pointer">
                        </div>
                    </div>

                    <!-- Output Status Screen -->
                    <div class="bg-tactical-800 p-6 rounded-xl border border-tactical-700 flex flex-col justify-between text-center">
                        <div>
                            <span class="text-xs font-mono text-gray-400 uppercase tracking-widest block mb-1">Resultado de Auditoría S.M.V.</span>
                            <div id="igd-score" class="text-4xl sm:text-5xl font-black font-mono text-amber-400 my-2">7.10</div>
                            <span class="text-xs text-gray-400 font-mono">IGD Ponderado Bruto</span>
                        </div>

                        <div id="status-box" class="p-4 rounded-xl border mt-4 transition-all bg-red-500/20 border-red-500 text-red-300">
                            <div class="font-black text-sm uppercase flex items-center justify-center gap-2 mb-1">
                                <i class="fa-solid fa-ban"></i> PROGRESIÓN BLOQUEADA
                            </div>
                            <p class="text-xs leading-relaxed">
                                VOTO DE CENSURA ACTIVO: Software Técnico &lt; 5.0. Se anula la Regla ALFA sin importar la potencia física.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 6: ¿QUÉ LO DIFERENCIA DE LAS METODOLOGÍAS ACTUALES? -->
    <section id="diferencias" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    6
                </div>
                <div>
                    <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                        ¿QUÉ LO DIFERENCIA DE LAS METODOLOGÍAS ACTUALES?
                    </h2>
                    <p class="text-xs text-amber-400 font-mono uppercase">Comparación Conceptual y Paradigmática</p>
                </div>
            </div>

            <!-- Detailed Comparison Table -->
            <div class="overflow-x-auto rounded-lg">
                <table class="min-w-[700px] w-full text-left text-xs sm:text-sm text-gray-300 border-collapse">
                    <thead>
                        <tr class="bg-tactical-900 text-gray-400 font-mono uppercase border-b border-tactical-700">
                            <th class="p-4">Dimensión</th>
                            <th class="p-4 text-red-400">Metodologías Tradicionales</th>
                            <th class="p-4 text-amber-400 font-bold">Codex Bellator – Ars Unified</th>
                        </tr>
                    </thead>
                    <tbody class="divide-y divide-tactical-700/60 font-medium">
                        <tr class="hover:bg-tactical-800/50">
                            <td class="p-4 text-white font-mono">Temporalidad</td>
                            <td class="p-4 text-gray-400">Secuencial / Serie (Bloqueo T1 → Golpe T2). Latencia reactiva alta (~200ms).</td>
                            <td class="p-4 text-amber-300 font-semibold">Paralelo / Kairós (Tiempo Cero $T0$). Intercepción simultánea ($Lin\ Sil\ Die\ Dar$).</td>
                        </tr>
                        <tr class="hover:bg-tactical-800/50">
                            <td class="p-4 text-white font-mono">Control de Fatiga</td>
                            <td class="p-4 text-gray-400">Acumulación de fatiga metabólica y "sufrir la serie". Genera volumen basura.</td>
                            <td class="p-4 text-amber-300 font-semibold">Regla del 10% UVC (Umbral de Velocidad Crítica). Aborto automático de serie.</td>
                        </tr>
                        <tr class="hover:bg-tactical-800/50">
                            <td class="p-4 text-white font-mono">Evaluación</td>
                            <td class="p-4 text-gray-400">Criterio subjetivo del entrenador ("se ve bien") y notas de texto libre.</td>
                            <td class="p-4 text-amber-300 font-semibold">Telemetría S.M.V. ($IGD$, $I.I.S.$, $I.P.F.$) e IA-P1 adaptativa por algoritmos.</td>
                        </tr>
                        <tr class="hover:bg-tactical-800/50">
                            <td class="p-4 text-white font-mono">Reclutamiento Motor</td>
                            <td class="p-4 text-gray-400">Henneman convencional (activa primero Fibras Lentas Tipo I).</td>
                            <td class="p-4 text-amber-300 font-semibold">Henneman Modificado: Intención Absoluta y Rate Coding (Fibras IIa y IIx).</td>
                        </tr>
                        <tr class="hover:bg-tactical-800/50">
                            <td class="p-4 text-white font-mono">Estructura del Drill</td>
                            <td class="p-4 text-gray-400">Repetición ciega de secuencias fijas de 3 pasos sin contexto.</td>
                            <td class="p-4 text-amber-300 font-semibold">Continuidad de Flujo ($A+D+A=1$ como modelo flexible sin pausas pasivas).</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>

        <div class="my-8 text-amber-500/80 text-3xl text-center">
            <i class="fa-solid fa-chevron-down"></i>
        </div>
    </section>

    <!-- SECTION 7: ¿QUÉ CUALIDADES LO DIFERENCIAN? -->
    <section id="cualidades" class="py-12 max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 border-t border-tactical-800">
        <div class="bg-tactical-800/60 border border-tactical-700/80 rounded-2xl p-6 sm:p-10 shadow-xl">
            <div class="flex items-center gap-3 mb-6">
                <div class="w-10 h-10 rounded-lg bg-amber-500/20 text-amber-400 flex items-center justify-center text-lg font-bold">
                    7
                </div>
                <div>
                    <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-tight leading-tight">
                        ¿QUÉ CUALIDADES LO DIFERENCIAN?
                    </h2>
                    <p class="text-xs text-amber-400 font-mono uppercase">Características Fundamentales y Sinergia del Orden</p>
                </div>
            </div>

            <!-- The 7 Pillars Grid -->
            <h3 class="text-lg font-bold text-white mb-4 flex items-center gap-2">
                <i class="fa-solid fa-cubes text-amber-400"></i>
                Los 7 Pilares de la Sinergia del Orden
            </h3>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-3 mb-8">
                <div class="p-3 bg-tactical-900 rounded-lg border border-tactical-700 text-xs">
                    <span class="text-amber-400 font-mono font-bold block mb-1">1. Metodología (S.C.I.T.O.)</span>
                    La causa rectora que define las leyes del tiempo y simultaneidad.
                </div>
                <div class="p-3 bg-tactical-900 rounded-lg border border-tactical-700 text-xs">
                    <span class="text-amber-400 font-mono font-bold block mb-1">2. Técnica Geométrica</span>
                    Ejecución inexpugnable basada en las leyes universales biomecánicas.
                </div>
                <div class="p-3 bg-tactical-900 rounded-lg border border-tactical-700 text-xs">
                    <span class="text-amber-400 font-mono font-bold block mb-1">3. Prep. Física (V.A.F.P.)</span>
                    Suministro de alto voltaje bioeléctrico y hardware de fibras rápidas.
                </div>
                <div class="p-3 bg-tactical-900 rounded-lg border border-tactical-700 text-xs">
                    <span class="text-amber-400 font-mono font-bold block mb-1">4. Táctica Inmediata</span>
                    Resolución en milisegundos sin vacilación en la toma de decisión.
                </div>
                <div class="p-3 bg-tactical-900 rounded-lg border border-tactical-700 text-xs">
                    <span class="text-amber-400 font-mono font-bold block mb-1">5. Estrategia Macro</span>
                    Conducción inteligente del combate y gestión del ring.
                </div>
                <div class="p-3 bg-tactical-900 rounded-lg border border-tactical-700 text-xs">
                    <span class="text-amber-400 font-mono font-bold block mb-1">6. Mentalidad & Silencio</span>
                    Escudo espiritual e inquebrantable silencio cognitivo bajo pánico.
                </div>
                <div class="p-3 bg-tactical-900 rounded-lg border border-tactical-700 text-xs sm:col-span-2">
                    <span class="text-amber-400 font-mono font-bold block mb-1">7. Sistema de Medición (S.M.V.)</span>
                    Lazo cerrado matemático para auditar y purgar el sistema de forma objetiva.
                </div>
            </div>

            <!-- BTU 15 Metadata callout -->
            <div class="bg-gradient-to-r from-tactical-900 via-tactical-800 to-tactical-900 p-6 rounded-xl border border-amber-500/30">
                <h4 class="text-amber-400 font-bold text-sm uppercase font-mono mb-2 flex items-center gap-2">
                    <i class="fa-solid fa-database"></i>
                    Biblioteca Técnica Universal (BTU-First) • 15 Metadatos Inmutables
                </h4>
                <p class="text-xs text-gray-300 leading-relaxed mb-3">
                    Cada técnica registrada en la BTU debe declarar sus 15 metadatos de eficiencia (Código SCITO, Nivel Dificultad, Objetivo Fisiológico, Nivel Transferencia, Fatiga Generada, Restricciones A.F.E., Fase de Mayor Valor, Ratio ICB, Sinergias PAP, etc.) antes de ingresar a cualquier plan semanal.
                </p>
                <div class="flex flex-wrap gap-2 text-[10px] font-mono text-amber-300">
                    <span class="bg-tactical-900 px-2 py-1 rounded border border-tactical-700">ICB = Transferencia / Fatiga Neural + Metabólica</span>
                    <span class="bg-tactical-900 px-2 py-1 rounded border border-tactical-700">Motor IA-P1 (Reglas Alfa, Beta, Gamma, Delta)</span>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER CREDITS BLOCK -->
    <footer class="bg-tactical-950 border-t border-tactical-800 py-12 px-4 sm:px-6 lg:px-8 text-center relative overflow-hidden">
        <div class="max-w-4xl mx-auto space-y-6">
            <div class="w-16 h-16 rounded-2xl bg-gradient-to-br from-amber-500 to-amber-700 text-black flex items-center justify-center text-2xl font-black mx-auto shadow-lg shadow-amber-500/20">
                <i class="fa-solid fa-shield-halved"></i>
            </div>

            <div>
                <h2 class="text-2xl sm:text-3xl font-black text-white uppercase tracking-widest leading-tight">
                    CODEX BELLATOR
                </h2>
                <h3 class="text-lg font-bold text-amber-400 tracking-wider font-mono uppercase">
                    ARS UNIFIED
                </h3>
            </div>

            <div class="border-t border-b border-tactical-800 py-4 max-w-md mx-auto">
                <p class="text-base font-bold text-white">
                    Henry R. Ruiz Huyke
                </p>
                <p class="text-xs text-amber-400/90 font-mono uppercase tracking-wider mt-0.5">
                    Investigador y desarrollador
                </p>
            </div>

            <div class="text-xs text-gray-500 font-mono space-y-1">
                <p>Ciencia de Combate Unificado (C.C.U.)</p>
                <p>Fase I y II Canónica — Sistema Cerrado de Ingeniería Humana</p>
                <p class="text-gray-600 pt-2">© 2026 CODEX BELLATOR ARS UNIFIED. Todos los derechos reservados.</p>
            </div>
        </div>
    </footer>

    <!-- JavaScript Interactions -->
    <script>
        const mobileBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        function switchTab(tabId) {
            // Hide all tab panes
            const panes = document.querySelectorAll('.tab-pane');
            panes.forEach(pane => pane.classList.add('hidden'));

            // Deactivate all buttons
            const btns = document.querySelectorAll('.tab-btn');
            btns.forEach(btn => {
                btn.classList.remove('bg-amber-500', 'text-black', 'shadow-md');
                btn.classList.add('bg-tactical-700', 'text-gray-300');
            });

            // Show target pane
            const targetPane = document.getElementById('content-' + tabId);
            if (targetPane) targetPane.classList.remove('hidden');

            // Activate target button
            const targetBtn = document.getElementById('tab-' + tabId);
            if (targetBtn) {
                targetBtn.classList.remove('bg-tactical-700', 'text-gray-300');
                targetBtn.classList.add('bg-amber-500', 'text-black', 'shadow-md');
            }
        }

        function calculateIGD() {
            const hf = parseFloat(document.getElementById('input-hf').value);
            const hn = parseFloat(document.getElementById('input-hn').value);
            const st = parseFloat(document.getElementById('input-st').value);
            const ste = parseFloat(document.getElementById('input-ste').value);
            const gm = parseFloat(document.getElementById('input-gm').value);

            // Update UI value labels
            document.getElementById('val-hf').innerText = hf.toFixed(1);
            document.getElementById('val-hn').innerText = hn.toFixed(1);
            document.getElementById('val-st').innerText = st.toFixed(1);
            document.getElementById('val-ste').innerText = ste.toFixed(1);
            document.getElementById('val-gm').innerText = gm.toFixed(1);

            // Calculate Weighted Average
            const igdRaw = (0.20 * hf) + (0.20 * hn) + (0.20 * st) + (0.20 * ste) + (0.20 * gm);
            document.getElementById('igd-score').innerText = igdRaw.toFixed(2);

            const statusBox = document.getElementById('status-box');

            // Software Veto Clause check (Software Técnico < 5.0 OR Software Táctico < 5.0)
            if (st < 5.0 || ste < 5.0) {
                statusBox.className = "p-4 rounded-xl border mt-4 transition-all bg-red-500/20 border-red-500 text-red-300";
                statusBox.innerHTML = `
                    <div class="font-black text-sm uppercase flex items-center justify-center gap-2 mb-1">
                        <i class="fa-solid fa-ban"></i> PROGRESIÓN BLOQUEADA (VOTO DE CENSURA)
                    </div>
                    <p class="text-xs leading-relaxed">
                        Cláusula de Voto de Censura de Software Activa: ${st < 5.0 ? 'Software Técnico' : 'Software Táctico'} &lt; 5.0. Se veta el avance a una nueva campaña independientemente de las notas de Hardware.
                    </p>
                `;
            } else if (igdRaw >= 8.0) {
                statusBox.className = "p-4 rounded-xl border mt-4 transition-all bg-emerald-500/20 border-emerald-500 text-emerald-300";
                statusBox.innerHTML = `
                    <div class="font-black text-sm uppercase flex items-center justify-center gap-2 mb-1">
                        <i class="fa-solid fa-circle-check"></i> PROGRESIÓN AUTORIZADA (REGLA ALFA)
                    </div>
                    <p class="text-xs leading-relaxed">
                        IGD Sobresaliente. Se incrementa la carga y la complejidad técnica en un +10% para el siguiente microciclo.
                    </p>
                `;
            } else {
                statusBox.className = "p-4 rounded-xl border mt-4 transition-all bg-amber-500/20 border-amber-500 text-amber-300";
                statusBox.innerHTML = `
                    <div class="font-black text-sm uppercase flex items-center justify-center gap-2 mb-1">
                        <i class="fa-solid fa-triangle-exclamation"></i> CONSOLIDACIÓN (REGLA BETA)
                    </div>
                    <p class="text-xs leading-relaxed">
                        IGD Estable. Se mantiene la carga actual y se prioriza el arsenal con mayor ratio Costo-Beneficio (ICB ≥ 8).
                    </p>
                `;
            }
        }

        // Initialize calculator on page load
        window.onload = function() {
            calculateIGD();
        };
    </script>
</body>
</html>
