<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Infographic: 3 Valkuilen bij het Leren</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Chart.js -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Roboto:wght@300;400;500&display=swap" rel="stylesheet">

    <style>
        /* Custom Font Settings */
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f8fafc; /* Slate 50 */
            color: #1e293b; /* Slate 800 */
        }
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Poppins', sans-serif;
        }

        /* Chart Container Rules - Strict Adherence */
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 650px; /* Limits width on large screens */
            height: 400px;    /* Default height */
            margin-left: auto;
            margin-right: auto;
        }

        @media (max-width: 768px) {
            .chart-container {
                height: 300px; /* Adjusted for mobile */
            }
        }

        /* Utility for Text-based Icons (No SVG) */
        .icon-circle {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            font-weight: bold;
            font-size: 1.5rem;
        }

        /* Custom Scrollbar for a polished look */
        ::-webkit-scrollbar {
            width: 10px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #cbd5e1;
            border-radius: 5px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #94a3b8;
        }
    </style>
    
    <!-- 
    SOURCE MATERIAL ANALYSIS & PLAN:
    The article "3 Valkuilen bij Leren" outlines three cognitive errors students/teachers make.
    
    NARRATIVE FLOW:
    1. Header: Establish the conflict (Intuition vs. Science).
    2. Pitfall 1 (Recognition): Using a Bar Chart to show the "Illusion of Competence" (Reading vs. Testing).
    3. Pitfall 2 (Forgetting): Using a Line Chart to show the Ebbinghaus Forgetting Curve vs. Spaced Repetition.
    4. Pitfall 3 (Multitasking): Using a Stacked Bar to show the "Switching Cost" in cognitive load.
    5. Solutions: A CSS-Grid based process map showing the correct behaviors.
    
    PALETTE (Vibrant Modern):
    - Background: #f8fafc
    - Primary Text: #1e293b
    - Pitfall Color: #ef4444 (Red)
    - Reality/Science Color: #3b82f6 (Blue)
    - Solution Color: #10b981 (Emerald)
    - Accent: #f59e0b (Amber)
    
    VISUALIZATION CHOICES (NO SVG):
    - Chart.js for all graphs (Bar, Line, Stacked Bar).
    - CSS Shapes/Entities for icons.
    - Tailwind Grid for layout.
    -->
</head>
<body class="antialiased selection:bg-blue-100 selection:text-blue-900">

    <!-- Header Section -->
    <header class="bg-gradient-to-r from-slate-900 to-slate-800 text-white pt-20 pb-16 px-4 shadow-xl">
        <div class="max-w-5xl mx-auto text-center">
            <div class="inline-block bg-blue-600 text-xs font-bold px-3 py-1 rounded-full mb-4 tracking-wide uppercase">Cognitieve Psychologie</div>
            <h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">
                3 Valkuilen <span class="text-blue-400">bij het Leren</span>
            </h1>
            <p class="text-xl md:text-2xl text-slate-300 max-w-3xl mx-auto font-light">
                Waarom je gevoel je vaak bedriegt tijdens het studeren. Een wetenschappelijke kijk op hoe ons brein écht werkt.
            </p>
        </div>
    </header>

    <main class="max-w-6xl mx-auto px-4 -mt-10 relative z-10 pb-20">

        <!-- Intro Card -->
        <div class="bg-white rounded-xl shadow-lg p-8 mb-12 border-l-8 border-blue-500">
            <h2 class="text-2xl font-bold mb-4 text-slate-800">De Illusie van Competentie</h2>
            <p class="text-lg text-slate-600 leading-relaxed">
                Veel traditionele leermethoden voelen goed aan, maar leveren weinig resultaat op. Onderzoekers noemen dit de <strong>illusie van competentie</strong>. We denken dat we iets beheersen omdat het bekend voorkomt, maar in werkelijkheid slaan we het niet op in ons langetermijngeheugen. Hieronder ontleden we de drie grootste valkuilen.
            </p>
        </div>

        <!-- Section 1: Valkuil 1 -->
        <section class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center mb-24">
            <div class="order-2 md:order-1">
                <div class="flex items-center mb-4">
                    <span class="icon-circle bg-red-100 text-red-600 w-12 h-12 mr-4">1</span>
                    <h3 class="text-3xl font-bold text-slate-800">Herkennen ≠ Kennen</h3>
                </div>
                <h4 class="text-xl font-semibold text-red-500 mb-4">De Valkuil: "Ik zie het, dus ik weet het."</h4>
                <p class="text-slate-600 mb-4 leading-relaxed">
                    Als je een tekst keer op keer herleest, wordt deze voorspelbaar. Dit 'vloeiende' gevoel (fluency) wordt vaak onterecht aangezien voor beheersing. Het is als kijken naar een schilder: het ziet er makkelijk uit totdat je zelf de kwast pakt.
                </p>
                <div class="bg-blue-50 p-4 rounded-lg border border-blue-100">
                    <h5 class="font-bold text-blue-800 mb-2">Het Bewijs</h5>
                    <p class="text-sm text-blue-700">
                        Onderzoek toont aan dat studenten die herlezen hun eigen kennis hoog inschatten (voorspelling), maar laag scoren op de toets. Studenten die zichzelf testen voelen zich onzekerder, maar scoren aanzienlijk hoger.
                    </p>
                </div>
            </div>
            <div class="order-1 md:order-2 bg-white p-6 rounded-xl shadow-md">
                <h4 class="text-center font-bold text-slate-700 mb-2">Gevoel vs. Werkelijkheid</h4>
                <div class="chart-container">
                    <canvas id="chartRecognition"></canvas>
                </div>
                <p class="text-center text-xs text-slate-400 mt-2">Gebaseerd op principes van Roediger & Karpicke (2006)</p>
            </div>
        </section>

        <!-- Section 2: Valkuil 2 -->
        <section class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center mb-24">
            <div class="bg-white p-6 rounded-xl shadow-md">
                <h4 class="text-center font-bold text-slate-700 mb-2">De Vergeetcurve (Ebbinghaus)</h4>
                <div class="chart-container">
                    <canvas id="chartForgetting"></canvas>
                </div>
                <p class="text-center text-xs text-slate-400 mt-2">Percentage onthouden kennis over tijd zonder herhaling</p>
            </div>
            <div>
                <div class="flex items-center mb-4">
                    <span class="icon-circle bg-red-100 text-red-600 w-12 h-12 mr-4">2</span>
                    <h3 class="text-3xl font-bold text-slate-800">Het Geheugen Lekt</h3>
                </div>
                <h4 class="text-xl font-semibold text-red-500 mb-4">De Valkuil: "Ik vergeet dit nooit meer."</h4>
                <p class="text-slate-600 mb-4 leading-relaxed">
                    Net na een les is de informatie vers en helder. We gaan ervan uit dat dit zo blijft. Helaas is ons brein geprogrammeerd om 'onnuttige' informatie snel te wissen. Zonder actieve herhaling ben je na een week tot wel 80% kwijt.
                </p>
                <div class="bg-emerald-50 p-4 rounded-lg border border-emerald-100">
                    <h5 class="font-bold text-emerald-800 mb-2">De Oplossing: Spreiden</h5>
                    <p class="text-sm text-emerald-700">
                        Door leermomenten te spreiden in de tijd (spaced repetition) dwing je je brein om de informatie opnieuw op te diepen. Dit vertraagt het vergeetproces aanzienlijk.
                    </p>
                </div>
            </div>
        </section>

        <!-- Section 3: Valkuil 3 -->
        <section class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center mb-24">
            <div class="order-2 md:order-1">
                <div class="flex items-center mb-4">
                    <span class="icon-circle bg-red-100 text-red-600 w-12 h-12 mr-4">3</span>
                    <h3 class="text-3xl font-bold text-slate-800">De Mythe van Multitasking</h3>
                </div>
                <h4 class="text-xl font-semibold text-red-500 mb-4">De Valkuil: "Ik kan leren én appen."</h4>
                <p class="text-slate-600 mb-4 leading-relaxed">
                    Ons werkgeheugen is beperkt. Echte multitasking bestaat niet; we 'task-switchen' razendsnel. Elke wissel kost cognitieve energie (switching cost). Hierdoor wordt de informatie niet diepgaand verwerkt en begrijp je de stof slechts oppervlakkig.
                </p>
                <ul class="space-y-2 text-slate-600">
                    <li class="flex items-start">
                        <span class="text-red-500 mr-2 font-bold">&times;</span>
                        <span>Minder diepgang in begrip.</span>
                    </li>
                    <li class="flex items-start">
                        <span class="text-red-500 mr-2 font-bold">&times;</span>
                        <span>Meer tijd nodig voor dezelfde taak.</span>
                    </li>
                    <li class="flex items-start">
                        <span class="text-red-500 mr-2 font-bold">&times;</span>
                        <span>Hogere foutgevoeligheid.</span>
                    </li>
                </ul>
            </div>
            <div class="order-1 md:order-2 bg-white p-6 rounded-xl shadow-md">
                <h4 class="text-center font-bold text-slate-700 mb-2">Cognitieve Belasting bij Afleiding</h4>
                <div class="chart-container">
                    <canvas id="chartMultitasking"></canvas>
                </div>
                <p class="text-center text-xs text-slate-400 mt-2">Effectieve leertijd vs. verlies door 'switching cost'</p>
            </div>
        </section>

        <!-- Solution Strategy Section (CSS Diagram) -->
        <section class="bg-slate-900 rounded-3xl p-8 md:p-12 text-center shadow-2xl">
            <h2 class="text-3xl font-bold text-white mb-8">Van Valkuil naar <span class="text-emerald-400">Successtrategie</span></h2>
            <p class="text-slate-300 mb-12 max-w-2xl mx-auto">
                Om effectief te leren, moeten we de werking van ons brein omarmen in plaats van ertegen te vechten. Dit zijn de drie pijlers van effectief leren.
            </p>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-left">
                
                <!-- Strategy 1 -->
                <div class="bg-slate-800 rounded-xl p-6 border-t-4 border-blue-500 transform transition hover:-translate-y-2 duration-300">
                    <div class="w-12 h-12 bg-blue-500 rounded-lg flex items-center justify-center text-white text-2xl font-bold mb-4 shadow-lg shadow-blue-500/50">
                        ?
                    </div>
                    <h3 class="text-xl font-bold text-white mb-2">Retrieval Practice</h3>
                    <p class="text-slate-400 text-sm mb-4">
                        Stop met herlezen. Start met jezelf te toetsen.
                    </p>
                    <div class="bg-slate-700/50 p-3 rounded text-xs text-slate-300">
                        <span class="text-blue-400 font-bold">&rarr;</span> Sluit je boek en schrijf op wat je nog weet.
                    </div>
                </div>

                <!-- Strategy 2 -->
                <div class="bg-slate-800 rounded-xl p-6 border-t-4 border-amber-500 transform transition hover:-translate-y-2 duration-300">
                    <div class="w-12 h-12 bg-amber-500 rounded-lg flex items-center justify-center text-white text-2xl font-bold mb-4 shadow-lg shadow-amber-500/50">
                        &circlearrowright;
                    </div>
                    <h3 class="text-xl font-bold text-white mb-2">Spaced Repetition</h3>
                    <p class="text-slate-400 text-sm mb-4">
                        Spreid het leren over meerdere dagen of weken.
                    </p>
                    <div class="bg-slate-700/50 p-3 rounded text-xs text-slate-300">
                        <span class="text-amber-400 font-bold">&rarr;</span> Herhaal stof net voordat je het dreigt te vergeten.
                    </div>
                </div>

                <!-- Strategy 3 -->
                <div class="bg-slate-800 rounded-xl p-6 border-t-4 border-emerald-500 transform transition hover:-translate-y-2 duration-300">
                    <div class="w-12 h-12 bg-emerald-500 rounded-lg flex items-center justify-center text-white text-2xl font-bold mb-4 shadow-lg shadow-emerald-500/50">
                        !
                    </div>
                    <h3 class="text-xl font-bold text-white mb-2">Monotasking</h3>
                    <p class="text-slate-400 text-sm mb-4">
                        Focus op één ding. Elimineer alle afleidingen.
                    </p>
                    <div class="bg-slate-700/50 p-3 rounded text-xs text-slate-300">
                        <span class="text-emerald-400 font-bold">&rarr;</span> Telefoon weg. Eén taak tegelijk. Diepe focus.
                    </div>
                </div>

            </div>
        </section>

    </main>

    <footer class="bg-slate-100 py-8 text-center border-t border-slate-200">
        <p class="text-slate-500 text-sm">
            Gebaseerd op inzichten van <a href="https://vernieuwenderwijs.nl" class="text-blue-600 hover:underline font-bold">Vernieuwenderwijs.nl</a> | Cognitieve Leerstrategieën
        </p>
        <p class="text-slate-400 text-xs mt-2">
            Gegenereerd voor educatieve doeleinden.
        </p>
    </footer>

    <!-- JavaScript for Charts -->
    <script>
        // ---------------------------------------------------------
        // Utility: Label Wrapping for Chart.js
        // Splits long strings into arrays of strings for multi-line labels
        // ---------------------------------------------------------
        function wrapLabel(label, maxChars = 16) {
            if (label.length <= maxChars) return label;
            
            const words = label.split(' ');
            const lines = [];
            let currentLine = words[0];

            for (let i = 1; i < words.length; i++) {
                if ((currentLine + " " + words[i]).length <= maxChars) {
                    currentLine += " " + words[i];
                } else {
                    lines.push(currentLine);
                    currentLine = words[i];
                }
            }
            lines.push(currentLine);
            return lines;
        }

        // Apply wrapping to array of labels
        function processLabels(labels) {
            return labels.map(l => wrapLabel(l));
        }

        // ---------------------------------------------------------
        // Shared Chart Configuration
        // ---------------------------------------------------------
        Chart.defaults.font.family = "'Roboto', sans-serif";
        Chart.defaults.color = '#64748b'; // slate-500
        Chart.defaults.font.size = 12;
        Chart.defaults.maintainAspectRatio = false; // Critical for container responsiveness

        // Mandatory Tooltip Callback for Multi-line Labels
        const tooltipConfig = {
            callbacks: {
                title: function(tooltipItems) {
                    const item = tooltipItems[0];
                    let label = item.chart.data.labels[item.dataIndex];
                    if (Array.isArray(label)) {
                        return label.join(' ');
                    } else {
                        return label;
                    }
                }
            }
        };

        // ---------------------------------------------------------
        // CHART 1: Recognition vs. Recall (Bar Chart)
        // Comparison of "Predicted Score" vs "Actual Score"
        // ---------------------------------------------------------
        const ctx1 = document.getElementById('chartRecognition').getContext('2d');
        const labels1 = processLabels(['Passief Herlezen (Fluency)', 'Actief Testen (Retrieval)']);
        
        new Chart(ctx1, {
            type: 'bar',
            data: {
                labels: labels1,
                datasets: [
                    {
                        label: 'Gevoel van beheersing (Voorspelling)',
                        data: [85, 55],
                        backgroundColor: '#ef4444', // Red - The Trap
                        borderRadius: 4,
                        borderWidth: 0
                    },
                    {
                        label: 'Daadwerkelijke Toetsscore',
                        data: [40, 80],
                        backgroundColor: '#3b82f6', // Blue - The Reality
                        borderRadius: 4,
                        borderWidth: 0
                    }
                ]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: { padding: 20 }
                    },
                    tooltip: tooltipConfig,
                    title: {
                        display: true,
                        text: 'Verwachting vs. Resultaat',
                        font: { size: 16, weight: 'bold', family: 'Poppins' },
                        padding: { bottom: 20 }
                    }
                },
                scales: {
                    y: {
                        beginAtZero: true,
                        max: 100,
                        title: { display: true, text: 'Score (%)' }
                    }
                }
            }
        });

        // ---------------------------------------------------------
        // CHART 2: The Forgetting Curve (Line Chart)
        // Change over time with vs without repetition
        // ---------------------------------------------------------
        const ctx2 = document.getElementById('chartForgetting').getContext('2d');
        const labels2 = ['Direct', '20 min', '1 uur', '9 uur', '1 dag', '2 dagen', '6 dagen'];

        new Chart(ctx2, {
            type: 'line',
            data: {
                labels: labels2,
                datasets: [
                    {
                        label: 'Zonder Herhaling (Valkuil)',
                        data: [100, 58, 44, 36, 33, 28, 25],
                        borderColor: '#ef4444', // Red
                        backgroundColor: 'rgba(239, 68, 68, 0.1)',
                        fill: true,
                        tension: 0.4,
                        pointRadius: 4
                    },
                    {
                        label: 'Met Gespreide Herhaling',
                        data: [100, 100, 95, 90, 85, 95, 90], // Spikes indicate review sessions
                        borderColor: '#10b981', // Emerald
                        backgroundColor: 'rgba(16, 185, 129, 0.05)',
                        fill: false,
                        borderDash: [5, 5],
                        tension: 0.2,
                        pointRadius: 4
                    }
                ]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: { position: 'bottom' },
                    tooltip: tooltipConfig,
                    title: {
                        display: false
                    }
                },
                scales: {
                    y: {
                        beginAtZero: true,
                        max: 110,
                        title: { display: true, text: 'Kennis Retentie (%)' }
                    }
                }
            }
        });

        // ---------------------------------------------------------
        // CHART 3: Multitasking Cost (Stacked Bar / Composition)
        // Showing Composition of time
        // ---------------------------------------------------------
        const ctx3 = document.getElementById('chartMultitasking').getContext('2d');
        const labels3 = processLabels(['Monotasking (Focus)', 'Multitasking (Afleiding)']);

        new Chart(ctx3, {
            type: 'bar',
            data: {
                labels: labels3,
                datasets: [
                    {
                        label: 'Productieve Leertijd',
                        data: [95, 60],
                        backgroundColor: '#3b82f6', // Blue
                    },
                    {
                        label: 'Switching Cost (Verloren Tijd)',
                        data: [5, 40],
                        backgroundColor: '#f59e0b', // Amber/Orange
                    }
                ]
            },
            options: {
                indexAxis: 'y', // Horizontal bar for better label reading
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: { position: 'bottom' },
                    tooltip: tooltipConfig,
                    title: { display: false }
                },
                scales: {
                    x: {
                        stacked: true,
                        max: 100,
                        title: { display: true, text: 'Cognitieve Capaciteit (%)' }
                    },
                    y: {
                        stacked: true
                    }
                }
            }
        });

    </script>
</body>
</html>
