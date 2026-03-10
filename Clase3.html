<!DOCTYPE html>
<html lang="es" class="dark scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Operaciones con Conjuntos: Del Álgebra al Código</title>
    
    <script src="https://cdn.tailwindcss.com"></script>
    
    <script defer src="https://cdn.jsdelivr.net/npm/alpinejs@3.x.x/dist/cdn.min.js"></script>
    
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.9/dist/katex.min.css">
    <script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.9/dist/katex.min.js"></script>
    <script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.9/dist/contrib/auto-render.min.js" 
        onload="renderMathInElement(document.body, {
            delimiters: [
                {left: '$$', right: '$$', display: true},
                {left: '\\(', right: '\\)', display: false}
            ],
            throwOnError: false
        });"></script>

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">
    
    <style>
        body { font-family: 'Inter', sans-serif; background-color: #0f172a; color: #cbd5e1; }
        .font-mono { font-family: 'JetBrains Mono', monospace; }
        .progress-bar { position: fixed; top: 0; left: 0; height: 4px; background: linear-gradient(to right, #3b82f6, #10b981, #ef4444, #a855f7, #f59e0b); z-index: 50; transition: width 0.1s ease-out; }
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #1e293b; }
        ::-webkit-scrollbar-thumb { background: #475569; border-radius: 4px; }
        ::-webkit-scrollbar-thumb:hover { background: #64748b; }
        
        /* Tipografía Markdown adaptada */
        .prose h1, .prose h2, .prose h3, .prose h4 { color: #f8fafc; font-weight: 700; margin-top: 2rem; margin-bottom: 1rem; }
        .prose h1 { font-size: 2.25rem; }
        .prose h2 { font-size: 1.875rem; border-bottom: 1px solid #334155; padding-bottom: 0.5rem; }
        .prose h3 { font-size: 1.5rem; }
        .prose p { margin-bottom: 1rem; line-height: 1.7; }
        .prose ul, .prose ol { margin-bottom: 1rem; padding-left: 1.5rem; }
        .prose ul { list-style-type: disc; }
        .prose code:not(pre code) { background-color: #1e293b; padding: 0.2rem 0.4rem; border-radius: 0.25rem; font-family: 'JetBrains Mono', monospace; font-size: 0.875em; color: #e2e8f0; }
        .prose pre { background-color: #1e293b; padding: 1.25rem; border-radius: 0.5rem; overflow-x: auto; margin-bottom: 1rem; border: 1px solid #334155; font-family: 'JetBrains Mono', monospace; font-size: 0.875rem; line-height: 1.5; color: #e2e8f0; }
        .prose blockquote { border-left: 4px solid #475569; padding-left: 1rem; color: #94a3b8; font-style: italic; background: #1e293b; padding: 1rem; border-radius: 0 0.5rem 0.5rem 0; margin-bottom: 1rem;}
        .prose table { width: 100%; border-collapse: collapse; margin-bottom: 1.5rem; }
        .prose th, .prose td { border: 1px solid #334155; padding: 0.75rem; text-align: left; }
        .prose th { background-color: #1e293b; font-weight: 600; color: #f8fafc; }
        .katex { color: #f8fafc; font-size: 1.1em; }
        .svg-region { transition: fill-opacity 0.4s ease-in-out; }
    </style>
</head>
<body x-data="{ scrollProgress: 0 }" @scroll.window="scrollProgress = (window.scrollY / (document.documentElement.scrollHeight - window.innerHeight)) * 100">
    
    <div class="progress-bar" :style="`width: ${scrollProgress}%`"></div>

    <main class="max-w-4xl mx-auto px-6 py-12 prose prose-invert">
        
        <header class="mb-12 text-center">
            <h1 class="text-4xl md:text-5xl bg-clip-text text-transparent bg-gradient-to-r from-blue-400 via-green-400 to-purple-400">
                🔢 Operaciones con Conjuntos:<br>Del Álgebra al Código
            </h1>
            <div class="flex flex-wrap justify-center gap-4 mt-6 text-sm font-mono text-slate-400">
                <span class="bg-slate-800 px-3 py-1 rounded-full">🎓 Nivel: Grado 10° (15-16 años)</span>
                <span class="bg-slate-800 px-3 py-1 rounded-full">⏱️ Duración: 4 horas</span>
                <span class="bg-slate-800 px-3 py-1 rounded-full">📍 Modalidad: Presencial / Híbrida</span>
            </div>
        </header>

        <div class="my-10 bg-slate-800 p-6 rounded-xl border border-slate-700">
            <h3 class="mt-0 mb-4 text-center border-none">⏱️ Planificación de la Sesión</h3>
            <div class="flex flex-col md:flex-row w-full h-auto md:h-12 rounded-lg overflow-hidden font-mono text-xs font-bold text-slate-900 shadow-inner">
                <div class="bg-slate-400 flex items-center justify-center p-2 md:w-[12.5%]" title="Intro (20m)">Intro</div>
                <div class="bg-blue-400 flex items-center justify-center p-2 md:w-[26%]" title="Unión e Intersección (35m)">Unión/Int.</div>
                <div class="bg-red-400 flex items-center justify-center p-2 md:w-[26%]" title="Dif. y Comp. (35m)">Dif/Comp</div>
                <div class="bg-slate-400 flex items-center justify-center p-2 md:w-[22%]" title="Ejercicios (30m)">Ejercicios</div>
                <div class="bg-amber-200 flex items-center justify-center p-2 md:w-[11%]" title="Descanso 1 (15m)">☕</div>
                <div class="bg-amber-500 flex items-center justify-center p-2 md:w-[22%]" title="Programación (30m)">Código</div>
                <div class="bg-purple-400 flex items-center justify-center p-2 md:w-[33%]" title="Trabajo Equipo (45m)">Equipo</div>
                <div class="bg-amber-200 flex items-center justify-center p-2 md:w-[11%]" title="Descanso 2 (15m)">☕</div>
                <div class="bg-emerald-400 flex items-center justify-center p-2 md:w-[33%]" title="Reto y Cierre (45m)">Reto/Cierre</div>
            </div>
        </div>

        <hr class="border-slate-700 my-8">

        <section id="introduccion">
            <h2>1. 🎯 ¿Qué vamos a aprender hoy?</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 10 minutos</p>
            <p>Imagina que tienes dos listas de reproducción en Spotify:</p>
            <ul>
                <li>🎵 <strong>Lista A:</strong> las canciones que escuchas cuando estudias</li>
                <li>🎵 <strong>Lista B:</strong> las canciones que escuchas cuando entrenas</li>
            </ul>
            <p>¿Qué pasa si quieres crear una nueva lista con <strong>todas</strong> esas canciones? ¿O solo las que comparten ambas listas? ¿O quieres eliminar las que ya escuchaste?</p>
            <p>Eso es exactamente lo que hacen las <strong>operaciones con conjuntos</strong>.</p>

            <h3>Objetivos de Aprendizaje</h3>
            <ul>
                <li>✅ Identificar y representar conjuntos usando notación simbólica y diagramas de Venn</li>
                <li>✅ Aplicar las operaciones de <strong>unión, intersección, diferencia y complemento</strong></li>
                <li>✅ Relacionar estas operaciones con <strong>condiciones lógicas en programación</strong></li>
                <li>✅ Resolver problemas en equipo usando el pensamiento matemático</li>
            </ul>

            <div class="bg-slate-800 p-6 rounded-lg mt-6 border border-slate-700">
                <h3 class="mt-0 text-emerald-400">🧠 Activador de Conocimiento Previo</h3>
                <p>Antes de comenzar, responde en tu cuaderno:</p>
                <ol>
                    <li>¿Qué es un conjunto? Da un ejemplo de la vida real.</li>
                    <li>¿Conoces alguna app o programa que filtre información? ¿Cómo crees que lo hace?</li>
                    <li>En programación, ¿qué significa la condición <code>AND</code> y <code>OR</code>?</li>
                </ol>
                <p class="mb-0 italic text-slate-400">💬 <strong>Comparte tu respuesta</strong> con el compañero de al lado durante 2 minutos.</p>
            </div>
        </section>

        <section id="repaso" class="mt-12">
            <h2>2. 📚 Repaso Rápido: ¿Qué es un Conjunto?</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 10 minutos</p>
            <p>Un <strong>conjunto</strong> es una colección bien definida de elementos distintos.</p>
            
            <h3>Formas de Representar un Conjunto</h3>
            <div class="grid md:grid-cols-2 gap-4 mb-6">
                <div class="bg-slate-800 p-4 rounded-lg border border-slate-700">
                    <h4 class="font-bold text-white mt-0 mb-2">1. Por extensión</h4>
                    <pre class="m-0 border-0 bg-slate-900 text-sm"><code>A = {1, 2, 3, 4, 5}
B = {perro, gato, loro, pez}</code></pre>
                </div>
                <div class="bg-slate-800 p-4 rounded-lg border border-slate-700">
                    <h4 class="font-bold text-white mt-0 mb-2">2. Por comprensión</h4>
                    <pre class="m-0 border-0 bg-slate-900 text-sm"><code>A = {x | x es natural par < 10}
A = {2, 4, 6, 8}</code></pre>
                </div>
            </div>

            <div class="bg-slate-800 p-6 rounded-lg border border-slate-700 mb-6 flex justify-center">
                <div class="w-full max-w-sm">
                    <h4 class="font-bold text-white mt-0 mb-6 text-left">3. Mediante diagrama de Venn:</h4>
                    <svg viewBox="0 0 300 200" class="w-full h-auto drop-shadow-md">
                        <rect width="300" height="200" fill="#1e293b" stroke="#475569" stroke-width="2" rx="8"/>
                        <text x="10" y="20" fill="#94a3b8" class="font-mono text-xs font-bold">Universo (U)</text>
                        
                        <circle cx="150" cy="110" r="70" fill="#334155" stroke="#64748b" stroke-width="2"/>
                        <text x="150" y="85" fill="#ffffff" class="font-bold text-xl" text-anchor="middle">A</text>
                        
                        <text x="150" y="115" fill="#cbd5e1" class="font-mono text-sm" text-anchor="middle">{1, 2, 3}</text>
                    </svg>
                </div>
            </div>

            <h3>Notación Importante</h3>
            <table>
                <thead>
                    <tr><th>Símbolo</th><th>Significado</th><th>Ejemplo</th></tr>
                </thead>
                <tbody>
                    <tr><td class="font-mono text-center">\( \in \)</td><td>"pertenece a"</td><td>\( 3 \in A \)</td></tr>
                    <tr><td class="font-mono text-center">\( \notin \)</td><td>"no pertenece a"</td><td>\( 7 \notin A \)</td></tr>
                    <tr><td class="font-mono text-center">\( \subseteq \)</td><td>"es subconjunto de"</td><td>\( \{1,2\} \subseteq A \)</td></tr>
                    <tr><td class="font-mono text-center">\( \emptyset \) o \( \{\} \)</td><td>Conjunto vacío</td><td>\( \emptyset \)</td></tr>
                    <tr><td class="font-mono text-center">\( U \)</td><td>Conjunto universal</td><td>Todos los elementos posibles</td></tr>
                    <tr><td class="font-mono text-center">\( n(A) \)</td><td>Cardinalidad</td><td>\( n(\{a,b,c\}) = 3 \)</td></tr>
                </tbody>
            </table>

            <h3>🔍 Ejemplo Real</h3>
            <p>Sea U = {todos los estudiantes del curso}</p>
            <pre><code>A = {estudiantes que practican fútbol}
B = {estudiantes que tocan algún instrumento}</code></pre>
            <p>Con estos dos conjuntos podemos hacernos preguntas interesantes... ¡y las responderemos con operaciones!</p>
        </section>

        <section id="union" class="mt-12 p-6 rounded-xl bg-blue-900/10 border border-blue-900/50">
            <h2 class="text-blue-400 border-blue-800 mt-0">3. 🔵🟡 Unión de Conjuntos \( A \cup B \)</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 17 minutos</p>
            
            <h3>Definición</h3>
            <p>La <strong>unión</strong> de dos conjuntos A y B es el conjunto formado por <strong>todos los elementos que pertenecen a A, a B, o a ambos</strong>.</p>
            
            <div class="text-center my-4 p-4 bg-blue-950/50 rounded-lg border border-blue-800">
                $$ A \cup B = \{x \mid x \in A \lor x \in B\} $$
            </div>
            
            <blockquote>🔑 <strong>Palabra clave: "O"</strong> — Para que un elemento esté en \( A \cup B \), basta con que esté en A <strong>O</strong> en B (o en los dos).</blockquote>

            <h3>Representación Gráfica</h3>
            <div class="relative w-full max-w-sm mx-auto my-8">
                <svg viewBox="0 0 300 200" class="w-full h-auto drop-shadow-lg">
                    <rect width="300" height="200" fill="#1e293b" stroke="#3b82f6" stroke-width="2" rx="8"/>
                    <text x="10" y="20" fill="#94a3b8" class="font-mono text-xs font-bold">U</text>
                    <circle cx="110" cy="100" r="60" fill="#3b82f6" fill-opacity="0.6"/>
                    <circle cx="190" cy="100" r="60" fill="#3b82f6" fill-opacity="0.6"/>
                    <circle cx="110" cy="100" r="60" fill="transparent" stroke="#60a5fa" stroke-width="2"/>
                    <circle cx="190" cy="100" r="60" fill="transparent" stroke="#60a5fa" stroke-width="2"/>
                    <text x="75" y="105" fill="#ffffff" class="font-bold text-lg">A</text>
                    <text x="215" y="105" fill="#ffffff" class="font-bold text-lg">B</text>
                    <text x="150" y="105" fill="#ffffff" class="font-bold text-sm" text-anchor="middle">A ∪ B</text>
                </svg>
            </div>

            <h3>Ejemplo Numérico</h3>
            <pre><code>A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}

A ∪ B = {1, 2, 3, 4, 5, 6, 7, 8}</code></pre>
            <p>⚠️ <strong>¡Importante!</strong> Los elementos que aparecen en los dos conjuntos (4 y 5) se escriben <strong>una sola vez</strong> en la unión.</p>

            <h3>Propiedades de la Unión</h3>
            <table>
                <tbody>
                    <tr><td>Conmutativa</td><td>\( A \cup B = B \cup A \)</td></tr>
                    <tr><td>Asociativa</td><td>\( (A \cup B) \cup C = A \cup (B \cup C) \)</td></tr>
                    <tr><td>Elemento neutro</td><td>\( A \cup \emptyset = A \)</td></tr>
                    <tr><td>Idempotente</td><td>\( A \cup A = A \)</td></tr>
                    <tr><td>Con el universo</td><td>\( A \cup U = U \)</td></tr>
                </tbody>
            </table>

            <div class="mt-6 p-4 border-l-4 border-amber-500 bg-amber-950/20">
                <h4 class="mt-0 text-amber-400">✏️ Practica Tú (Ejercicio guiado)</h4>
                <p>Sea:<br>
                <code>P = {a, e, i, o, u} (vocales)</code><br>
                <code>Q = {a, b, c, d, e} (primeras letras del alfabeto)</code></p>
                <ol>
                    <li>Halla P ∪ Q</li>
                    <li>¿Cuántos elementos tiene P ∪ Q? (Cardinalidad)</li>
                    <li>Dibuja el diagrama de Venn correspondiente</li>
                </ol>
                <p class="text-sm italic text-slate-400">💡 Pista: n(A ∪ B) = n(A) + n(B) - n(A ∩ B)</p>
            </div>
        </section>

        <section id="interseccion" class="mt-12 p-6 rounded-xl bg-green-900/10 border border-green-900/50">
            <h2 class="text-green-400 border-green-800 mt-0">4. 🟢 Intersección de Conjuntos \( A \cap B \)</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 18 minutos</p>

            <h3>Definición</h3>
            <p>La <strong>intersección</strong> de dos conjuntos A y B es el conjunto de los elementos que pertenecen <strong>a A Y también a B al mismo tiempo</strong>.</p>
            
            <div class="text-center my-4 p-4 bg-green-950/50 rounded-lg border border-green-800">
                $$ A \cap B = \{x \mid x \in A \land x \in B\} $$
            </div>
            
            <blockquote>🔑 <strong>Palabra clave: "Y"</strong> — Un elemento está en \( A \cap B \) solo si está en A <strong>Y</strong> en B simultáneamente.</blockquote>

            <h3>Representación Gráfica</h3>
            <div class="relative w-full max-w-sm mx-auto my-8">
                <svg viewBox="0 0 300 200" class="w-full h-auto drop-shadow-lg">
                    <defs><clipPath id="clipIntersectStatic"><circle cx="190" cy="100" r="60"/></clipPath></defs>
                    <rect width="300" height="200" fill="#1e293b" stroke="#10b981" stroke-width="2" rx="8"/>
                    <text x="10" y="20" fill="#94a3b8" class="font-mono text-xs font-bold">U</text>
                    <circle cx="110" cy="100" r="60" fill="transparent" stroke="#34d399" stroke-width="2"/>
                    <circle cx="190" cy="100" r="60" fill="transparent" stroke="#34d399" stroke-width="2"/>
                    <circle cx="110" cy="100" r="60" fill="#10b981" fill-opacity="0.8" clip-path="url(#clipIntersectStatic)"/>
                    <text x="75" y="105" fill="#94a3b8" class="font-bold text-lg">A</text>
                    <text x="215" y="105" fill="#94a3b8" class="font-bold text-lg">B</text>
                    <text x="150" y="105" fill="#ffffff" class="font-bold text-xs" text-anchor="middle">A ∩ B</text>
                </svg>
            </div>

            <h3>Ejemplo con Contexto Real</h3>
            <p>🎮 Videojuegos disponibles en plataformas:</p>
            <pre><code>A = {juegos en PlayStation} = {FIFA, GTA, Minecraft, Fortnite, Valorant}
B = {juegos en Xbox}        = {FIFA, GTA, Halo, Forza, Minecraft}

A ∩ B = {FIFA, GTA, Minecraft}
        ↑ Juegos disponibles en AMBAS plataformas</code></pre>

            <h3>Conjuntos Disjuntos</h3>
            <p>Cuando dos conjuntos no comparten ningún elemento: <code>A ∩ B = ∅</code></p>
            <pre><code>A = {números pares}   = {2, 4, 6, 8...}
B = {números impares} = {1, 3, 5, 7...}

A ∩ B = ∅  (ningún número es par e impar a la vez)</code></pre>

            <div class="mt-6 p-4 border-l-4 border-amber-500 bg-amber-950/20">
                <h4 class="mt-0 text-amber-400">✏️ Practica Tú</h4>
                <p>En un grupo de 30 estudiantes se sabe que:</p>
                <ul>
                    <li>18 tienen cuenta en Instagram (conjunto I)</li>
                    <li>15 tienen cuenta en TikTok (conjunto T)</li>
                    <li>8 tienen cuenta en <strong>ambas</strong> redes</li>
                </ul>
                <ol>
                    <li>Representa la situación en un diagrama de Venn</li>
                    <li>Halla I ∩ T</li>
                    <li>¿Cuántos estudiantes tienen Instagram pero <strong>no</strong> TikTok?</li>
                    <li>¿Cuántos estudiantes no tienen ninguna de las dos? *(Usa U = 30)*</li>
                </ol>
            </div>
        </section>

        <section id="diferencia" class="mt-12 p-6 rounded-xl bg-red-900/10 border border-red-900/50">
            <h2 class="text-red-400 border-red-800 mt-0">5. 🔴 Diferencia de Conjuntos \( A - B \)</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 17 minutos</p>

            <h3>Definición</h3>
            <p>La <strong>diferencia</strong> de A menos B es el conjunto de los elementos que <strong>pertenecen a A pero NO pertenecen a B</strong>.</p>
            
            <div class="text-center my-4 p-4 bg-red-950/50 rounded-lg border border-red-800">
                $$ A - B = \{x \mid x \in A \land x \notin B\} $$
            </div>
            
            <blockquote>🔑 <strong>Clave:</strong> \( A - B \neq B - A \) (¡La diferencia NO es conmutativa!)</blockquote>

            <h3>Representación Gráfica (A - B)</h3>
            <div class="relative w-full max-w-sm mx-auto my-8">
                <svg viewBox="0 0 300 200" class="w-full h-auto drop-shadow-lg">
                    <defs><mask id="maskDiffStatic"><rect width="300" height="200" fill="white"/><circle cx="190" cy="100" r="60" fill="black"/></mask></defs>
                    <rect width="300" height="200" fill="#1e293b" stroke="#ef4444" stroke-width="2" rx="8"/>
                    <text x="10" y="20" fill="#94a3b8" class="font-mono text-xs font-bold">U</text>
                    <circle cx="110" cy="100" r="60" fill="#ef4444" fill-opacity="0.7" mask="url(#maskDiffStatic)"/>
                    <circle cx="110" cy="100" r="60" fill="transparent" stroke="#f87171" stroke-width="2"/>
                    <circle cx="190" cy="100" r="60" fill="transparent" stroke="#f87171" stroke-width="2"/>
                    <text x="75" y="105" fill="#ffffff" class="font-bold text-lg">A</text>
                    <text x="215" y="105" fill="#94a3b8" class="font-bold text-lg">B</text>
                </svg>
            </div>

            <h3>Ejemplo Concreto y de la Vida Real</h3>
            <pre><code>A = {1, 2, 3, 4, 5}
B = {3, 4, 5, 6, 7}

A - B = {1, 2}         ← Lo de A que NO está en B
B - A = {6, 7}         ← Lo de B que NO está en A
A ∩ B = {3, 4, 5}      ← Lo que comparten</code></pre>

            <p>🎓 <strong>Materias:</strong></p>
            <pre><code>A = {materias que aprobó Laura} = {Matemáticas, Inglés, Historia, Arte}
B = {materias que aprobó Sofía} = {Inglés, Historia, Biología, Química}

A - B = {Matemáticas, Arte} (Aprobó Laura pero Sofía NO)
B - A = {Biología, Química} (Aprobó Sofía pero Laura NO)</code></pre>

            <div class="mt-6 p-4 border-l-4 border-amber-500 bg-amber-950/20">
                <h4 class="mt-0 text-amber-400">✏️ Practica Tú</h4>
                <p>Sea:<br>
                <code>X = {letras de la palabra "COMPUTADORA"}</code><br>
                <code>Y = {letras de la palabra "PROGRAMAR"}</code></p>
                <ol>
                    <li>Lista los elementos de X y de Y (sin repetir letras)</li>
                    <li>Halla X - Y</li>
                    <li>Halla Y - X</li>
                    <li>Verifica que X - Y ≠ Y - X</li>
                    <li>¿Qué relación existe entre A - B, B - A y A ∩ B?</li>
                </ol>
            </div>
        </section>

        <section id="complemento" class="mt-12 p-6 rounded-xl bg-purple-900/10 border border-purple-900/50">
            <h2 class="text-purple-400 border-purple-800 mt-0">6. ⚫ Complemento de un Conjunto \( A^c \)</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 18 minutos</p>

            <h3>Definición</h3>
            <p>El <strong>complemento</strong> de A (respecto al universo U) es el conjunto de <strong>todos los elementos del universo que NO pertenecen a A</strong>.</p>
            
            <div class="text-center my-4 p-4 bg-purple-950/50 rounded-lg border border-purple-800">
                $$ A^c = \{x \mid x \in U \land x \notin A\} $$
            </div>

            <p>También se escribe como: <strong>A'</strong>, <strong>Ā</strong>, <strong>~A</strong></p>
            <blockquote>🔑 <strong>Recuerda:</strong> El complemento siempre depende del <strong>Universo</strong> que definamos.</blockquote>

            <h3>Representación Gráfica</h3>
            <div class="relative w-full max-w-sm mx-auto my-8">
                <svg viewBox="0 0 300 200" class="w-full h-auto drop-shadow-lg">
                    <defs><mask id="maskCompStatic"><rect width="300" height="200" fill="white" rx="8"/><circle cx="150" cy="100" r="60" fill="black"/></mask></defs>
                    <rect width="300" height="200" fill="#a855f7" fill-opacity="0.5" mask="url(#maskCompStatic)"/>
                    <rect width="300" height="200" fill="transparent" stroke="#a855f7" stroke-width="2" rx="8"/>
                    <text x="10" y="20" fill="#ffffff" class="font-mono text-xs font-bold">U (Todo lo sombreado es Aᶜ)</text>
                    <circle cx="150" cy="100" r="60" fill="#1e293b" stroke="#c084fc" stroke-width="2"/>
                    <text x="150" y="105" fill="#94a3b8" class="font-bold text-lg" text-anchor="middle">A</text>
                </svg>
            </div>

            <h3>Ejemplo</h3>
            <pre><code>U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
A = {2, 4, 6, 8, 10}    (números pares)

Aᶜ = {1, 3, 5, 7, 9}   (números impares = los que no están en A)</code></pre>

            <h3>Propiedades y Leyes de De Morgan</h3>
            <table>
                <tbody>
                    <tr><td>Doble negación</td><td>\( (A^c)^c = A \)</td></tr>
                    <tr><td>Comp. del universo</td><td>\( U^c = \emptyset \)</td></tr>
                    <tr><td>Comp. del vacío</td><td>\( \emptyset^c = U \)</td></tr>
                    <tr class="bg-purple-900/40 text-purple-200"><td><strong>Ley de Morgan 1</strong></td><td><strong>\( (A \cup B)^c = A^c \cap B^c \)</strong></td></tr>
                    <tr class="bg-purple-900/40 text-purple-200"><td><strong>Ley de Morgan 2</strong></td><td><strong>\( (A \cap B)^c = A^c \cup B^c \)</strong></td></tr>
                </tbody>
            </table>

            <div class="mt-6 p-4 border-l-4 border-amber-500 bg-amber-950/20">
                <h4 class="mt-0 text-amber-400">✏️ Practica Tú</h4>
                <p>Sea:<br>
                <code>U = {a, b, c, d, e, f, g, h}</code><br>
                <code>A = {a, c, e, g}</code><br>
                <code>B = {b, c, d, e}</code></p>
                <ol>
                    <li>Halla Aᶜ, Bᶜ, (A ∩ B)ᶜ, y Aᶜ ∪ Bᶜ</li>
                    <li>Verifica la Segunda Ley de De Morgan: ¿Se cumple que (A ∩ B)ᶜ = Aᶜ ∪ Bᶜ?</li>
                </ol>
            </div>
        </section>

        <section id="laboratorio" class="mt-16 bg-slate-900 p-8 rounded-2xl border border-slate-600 shadow-2xl" x-data="{ op: 'none' }">
            <h2 class="mt-0 text-center border-none">🔬 Laboratorio Interactivo: Síntesis Visual</h2>
            <p class="text-center text-slate-400 text-sm mb-8">Haz clic en los botones para visualizar qué área del Universo sombrea cada operación matemática antes de ir al descanso.</p>
            
            <div class="flex flex-wrap gap-3 justify-center mb-8 font-mono text-sm">
                <button @click="op = 'union'" :class="op === 'union' ? 'bg-blue-600 text-white shadow-lg shadow-blue-500/30' : 'bg-slate-800 text-slate-400 hover:bg-slate-700'" class="px-5 py-2 rounded-lg transition-all font-bold">A ∪ B</button>
                <button @click="op = 'inter'" :class="op === 'inter' ? 'bg-green-600 text-white shadow-lg shadow-green-500/30' : 'bg-slate-800 text-slate-400 hover:bg-slate-700'" class="px-5 py-2 rounded-lg transition-all font-bold">A ∩ B</button>
                <button @click="op = 'diffA'" :class="op === 'diffA' ? 'bg-red-600 text-white shadow-lg shadow-red-500/30' : 'bg-slate-800 text-slate-400 hover:bg-slate-700'" class="px-5 py-2 rounded-lg transition-all font-bold">A - B</button>
                <button @click="op = 'diffB'" :class="op === 'diffB' ? 'bg-orange-500 text-white shadow-lg shadow-orange-500/30' : 'bg-slate-800 text-slate-400 hover:bg-slate-700'" class="px-5 py-2 rounded-lg transition-all font-bold">B - A</button>
                <button @click="op = 'compA'" :class="op === 'compA' ? 'bg-purple-600 text-white shadow-lg shadow-purple-500/30' : 'bg-slate-800 text-slate-400 hover:bg-slate-700'" class="px-5 py-2 rounded-lg transition-all font-bold">Aᶜ</button>
                <button @click="op = 'none'" class="px-5 py-2 rounded-lg transition-all font-bold bg-slate-800 text-slate-500 border border-slate-700 hover:text-white">Limpiar</button>
            </div>

            <div class="relative w-full max-w-lg mx-auto">
                <svg viewBox="0 0 400 250" class="w-full h-auto drop-shadow-2xl">
                    <defs>
                        <clipPath id="clipB"><circle cx="250" cy="125" r="80"/></clipPath>
                        <mask id="maskNotB"><rect width="400" height="250" fill="white"/><circle cx="250" cy="125" r="80" fill="black"/></mask>
                        <mask id="maskNotA"><rect width="400" height="250" fill="white"/><circle cx="150" cy="125" r="80" fill="black"/></mask>
                    </defs>
                    <rect width="400" height="250" fill="#0f172a" stroke="#334155" stroke-width="2" rx="12"/>
                    <rect width="400" height="250" class="svg-region" :fill-opacity="op === 'compA' ? '0.6' : '0'" fill="#a855f7" mask="url(#maskNotA)" rx="12"/>
                    <circle cx="150" cy="125" r="80" class="svg-region" :fill-opacity="op === 'union' ? '0.6' : '0'" fill="#3b82f6"/>
                    <circle cx="250" cy="125" r="80" class="svg-region" :fill-opacity="op === 'union' ? '0.6' : '0'" fill="#3b82f6"/>
                    <circle cx="150" cy="125" r="80" class="svg-region" :fill-opacity="op === 'inter' ? '0.8' : '0'" fill="#10b981" clip-path="url(#clipB)"/>
                    <circle cx="150" cy="125" r="80" class="svg-region" :fill-opacity="op === 'diffA' ? '0.8' : '0'" fill="#ef4444" mask="url(#maskNotB)"/>
                    <circle cx="250" cy="125" r="80" class="svg-region" :fill-opacity="op === 'diffB' ? '0.8' : '0'" fill="#f97316" mask="url(#maskNotA)"/>
                    <circle cx="150" cy="125" r="80" fill="transparent" stroke="#64748b" stroke-width="2" stroke-dasharray="4 4"/>
                    <circle cx="250" cy="125" r="80" fill="transparent" stroke="#64748b" stroke-width="2" stroke-dasharray="4 4"/>
                    <text x="15" y="25" fill="#94a3b8" class="font-mono text-sm font-bold">U</text>
                    <text x="100" y="130" fill="#ffffff" class="font-bold text-2xl drop-shadow-md">A</text>
                    <text x="280" y="130" fill="#ffffff" class="font-bold text-2xl drop-shadow-md">B</text>
                </svg>

                <div class="h-12 mt-6 text-center font-mono text-lg flex items-center justify-center">
                    <span x-show="op === 'none'" class="text-slate-500">Selecciona una operación arriba</span>
                    <span x-show="op === 'union'" x-cloak class="text-blue-400">$$ A \cup B $$</span>
                    <span x-show="op === 'inter'" x-cloak class="text-green-400">$$ A \cap B $$</span>
                    <span x-show="op === 'diffA'" x-cloak class="text-red-400">$$ A - B $$</span>
                    <span x-show="op === 'diffB'" x-cloak class="text-orange-400">$$ B - A $$</span>
                    <span x-show="op === 'compA'" x-cloak class="text-purple-400">$$ A^c $$</span>
                </div>
            </div>
        </section>

        <div class="my-16 border-l-4 border-amber-500 bg-amber-950/30 p-8 rounded-r-2xl shadow-lg relative overflow-hidden">
            <div class="absolute -right-10 -top-10 text-9xl opacity-10">☕</div>
            <h3 class="text-amber-400 mt-0 flex items-center gap-3">
                <span class="text-3xl">⏸️</span> DESCANSO 1 — 15 Minutos
            </h3>
            <p class="text-lg">🎉 ¡Buen trabajo! Han completado 2 horas de sesión.</p>
            <p>Tómate 15 minutos para:</p>
            <ul class="text-amber-200/80">
                <li>Hidratarte y comer algo</li>
                <li>Levantarte y moverte un poco</li>
                <li>Descansar la vista de la pantalla o tablero</li>
            </ul>
            <p class="font-bold text-amber-500 mb-0 mt-4">🕐 Regresamos en 15 minutos para conectar todo esto con la PROGRAMACIÓN.</p>
        </div>

        <section id="programacion" class="mt-12">
            <h2 class="text-amber-400 border-amber-800">8. 💻 Conjuntos y Lógica en Programación</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 30 minutos</p>
            <p>¡Bienvenidos de vuelta! Ahora viene la parte donde todo cobra sentido para el mundo digital. Cada vez que un programa <strong>filtra, busca o combina datos</strong>, está aplicando operaciones de conjuntos. Desde un buscador web hasta una app de música, todos usan esta lógica millones de veces por segundo.</p>
            
            <h3>Tabla de Equivalencias: Conjuntos ↔ Programación</h3>
            <table class="w-full text-sm">
                <thead>
                    <tr class="text-amber-300">
                        <th>Operación matemática</th>
                        <th>Operador Lógico</th>
                        <th>Palabra Clave</th>
                        <th>Ejemplo en Código</th>
                    </tr>
                </thead>
                <tbody class="font-mono text-xs">
                    <tr><td>Unión \( A \cup B \)</td><td class="text-blue-400">OR / ||</td><td>"O"</td><td>if (esFan || tieneBoleta)</td></tr>
                    <tr><td>Intersección \( A \cap B \)</td><td class="text-green-400">AND / &&</td><td>"Y"</td><td>if (esMayor && tieneID)</td></tr>
                    <tr><td>Complemento \( A^c \)</td><td class="text-purple-400">NOT / !</td><td>"NO"</td><td>if (!estaLogueado)</td></tr>
                    <tr><td>Diferencia \( A - B \)</td><td class="text-red-400">AND + NOT</td><td>"Y NO"</td><td>if (enListaA && !enListaB)</td></tr>
                </tbody>
            </table>

            <div class="grid md:grid-cols-2 gap-6 mt-6">
                <div class="bg-slate-800 p-4 rounded-lg border border-slate-700">
                    <h4 class="text-amber-300 mt-0">Ejemplo 1: Acceso (Intersección)</h4>
                    <pre class="text-amber-100 text-xs border-0 bg-slate-900 m-0"><code><span class="text-slate-500">// P = Premium, V = Verificada</span>
<span class="text-purple-400">SI</span> (esPremium <span class="text-green-400">AND</span> estaVerificado) <span class="text-purple-400">ENTONCES</span>
    mostrar_contenido_exclusivo()
<span class="text-purple-400">SINO</span>
    mostrar_contenido_basico()
<span class="text-purple-400">FIN SI</span></code></pre>
                </div>
                <div class="bg-slate-800 p-4 rounded-lg border border-slate-700">
                    <h4 class="text-amber-300 mt-0">Ejemplo 2: Filtro (Complemento)</h4>
                    <pre class="text-amber-100 text-xs border-0 bg-slate-900 m-0"><code><span class="text-slate-500">// Filtro: Todo EXCEPTO agotados (Sᶜ)</span>
<span class="text-purple-400">SI</span> (<span class="text-purple-400">NOT</span> estaAgotado) <span class="text-purple-400">ENTONCES</span>
    mostrar(producto)
<span class="text-purple-400">FIN SI</span></code></pre>
                </div>
            </div>

            <h3>Ejemplo 3: Bases de Datos — Consultas SQL</h3>
            <p>Las bases de datos usan operaciones de conjuntos directamente con palabras reservadas:</p>
            <pre><code><span class="text-slate-500">-- UNION: todos los clientes de Colombia O México</span>
<span class="text-purple-400">SELECT</span> nombre <span class="text-purple-400">FROM</span> clientes <span class="text-purple-400">WHERE</span> pais = <span class="text-green-300">'Colombia'</span>
<span class="text-blue-400 font-bold">UNION</span>
<span class="text-purple-400">SELECT</span> nombre <span class="text-purple-400">FROM</span> clientes <span class="text-purple-400">WHERE</span> pais = <span class="text-green-300">'México'</span>;

<span class="text-slate-500">-- EXCEPT (Diferencia): compraron en enero pero NO en febrero</span>
<span class="text-purple-400">SELECT</span> id <span class="text-purple-400">FROM</span> compras <span class="text-purple-400">WHERE</span> mes = <span class="text-green-300">'Enero'</span>
<span class="text-red-400 font-bold">EXCEPT</span>
<span class="text-purple-400">SELECT</span> id <span class="text-purple-400">FROM</span> compras <span class="text-purple-400">WHERE</span> mes = <span class="text-green-300">'Febrero'</span>;</code></pre>

            <h3>Las Leyes de De Morgan en Código</h3>
            <p><strong>JavaScript:</strong></p>
            <pre><code><span class="text-slate-500">// Condición: el usuario NO puede entrar si NO es admin O está suspendido</span>
<span class="text-slate-500">// Forma original !(A || B) :</span>
<span class="text-purple-400">if</span> ( !(esAdmin <span class="text-blue-400">||</span> estaSuspendido) ) { permitirAcceso(); }

<span class="text-slate-500">// Aplicando De Morgan !A && !B (equivalente y más legible):</span>
<span class="text-purple-400">if</span> ( !esAdmin <span class="text-green-400">&&</span> !estaSuspendido ) { permitirAcceso(); }</code></pre>

            <div class="mt-6 p-4 border-l-4 border-amber-500 bg-amber-950/20">
                <h4 class="mt-0 text-amber-400">🧩 Actividad Mental Rápida</h4>
                <p>Relaciona cada situación con la operación correcta. Escribe la expresión en tu cuaderno.</p>
                <ul>
                    <li>Usuarios que tienen Netflix <strong>O</strong> HBO</li>
                    <li>Canciones en tu playlist <strong>Y</strong> con más de 3 min</li>
                    <li>Películas del catálogo que <strong>NO</strong> están en tu historial</li>
                    <li>Amigos de FB que <strong>NO</strong> son tus seguidores en IG</li>
                </ul>
            </div>
        </section>

        <section id="equipo" class="mt-12 bg-slate-800/40 p-8 rounded-2xl border border-slate-700">
            <h2 class="mt-0 text-emerald-400 border-emerald-800">9. 👥 Trabajo Colaborativo en Equipos</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 45 minutos | Organización: Equipos de 3–4 personas</p>
            
            <p>Formen equipos y asignen roles:</p>
            <ul class="grid grid-cols-2 gap-2 text-sm">
                <li class="bg-slate-800 p-2 rounded">📐 Matemático/a</li>
                <li class="bg-slate-800 p-2 rounded">🎨 Diseñador/a visual</li>
                <li class="bg-slate-800 p-2 rounded">💻 Programador/a</li>
                <li class="bg-slate-800 p-2 rounded">🎤 Vocero/a</li>
            </ul>

            <div class="mt-8 space-y-6">
                <div class="p-6 bg-slate-900 rounded-xl border border-slate-600 shadow-lg">
                    <h4 class="text-emerald-400 mt-0 text-xl">🏆 MISIÓN 1: El Sistema de la Escuela (15 min)</h4>
                    <p class="text-sm text-slate-300"><strong>Contexto:</strong> Tu colegio tiene una plataforma digital y necesita organizar la información.</p>
                    <pre class="text-xs bg-slate-950"><code>U = {todos los 40 estudiantes del grado 10°}
D = {estudiantes que entregaron Diseño} = {Ana, Beto, Carlos, Diana, Elena, Fausto, Gina, Héctor, Iris, Juan}
M = {estudiantes que entregaron Matemáticas} = {Beto, Diana, Fausto, Héctor, Juan, Karen, Luis, Marta, Nora, Oscar}
T = {entregaron ambos a tiempo} = {Beto, Diana, Fausto, Héctor, Juan}</code></pre>
                    <p class="font-bold text-sm">El equipo debe responder:</p>
                    <ol class="text-sm space-y-1">
                        <li>Halla D ∪ M y explica qué representa.</li>
                        <li>Halla D ∩ M y compara con T. ¿Qué observan?</li>
                        <li>Halla D - M: ¿Qué estudiantes están y qué significa?</li>
                        <li>Halla Dᶜ: ¿Qué representa para el docente de Diseño?</li>
                        <li>¿Cuántos NO entregaron ningún proyecto? Muéstralo en diagrama.</li>
                        <li class="text-amber-400"><strong>Reto código:</strong> Escribe pseudocódigo para avisar a los que entregaron Diseño pero NO Matemáticas.</li>
                    </ol>
                </div>

                <div class="p-6 bg-slate-900 rounded-xl border border-slate-600 shadow-lg">
                    <h4 class="text-emerald-400 mt-0 text-xl">🏆 MISIÓN 2: La App de Streaming (15 min)</h4>
                    <p class="text-sm text-slate-300"><strong>Contexto:</strong> Análisis de datos de una app de música.</p>
                    <pre class="text-xs bg-slate-950"><code>U = {100 canciones más escuchadas}
R = {reggaetón} → n(R) = 35
P = {pop}       → n(P) = 40
E = {español}   → n(E) = 55
(R ∩ P = ∅), (R ⊆ E), n(P ∩ E) = 20</code></pre>
                    <p class="font-bold text-sm">El equipo debe responder:</p>
                    <ol class="text-sm space-y-1">
                        <li>Dibuja un diagrama de Venn con los tres conjuntos.</li>
                        <li>¿Cuántas canciones son pop en español?</li>
                        <li>¿Cuántas de pop son en otro idioma?</li>
                        <li>¿Cuántas no son ni reggaetón ni pop?</li>
                        <li>Halla n(R ∪ P ∪ E) con inclusión-exclusión.</li>
                        <li class="text-amber-400"><strong>Reto código:</strong> Filtrar: a) Solo español que NO sea reggaetón. b) Pop O reggaetón, sin importar idioma.</li>
                    </ol>
                </div>

                <div class="p-6 bg-slate-900 rounded-xl border border-slate-600 shadow-lg border-dashed">
                    <h4 class="text-emerald-400/80 mt-0 text-xl">🏆 MISIÓN 3: Torneo de Videojuegos (Opcional)</h4>
                    <pre class="text-xs bg-slate-950"><code>U={80 inscritos}, F={Fútbol}=45, L={LOL}=38, B={BattleRoyale}=30
n(F∩L)=15, n(F∩B)=10, n(L∩B)=12, n(F∩L∩B)=5</code></pre>
                    <ol class="text-sm">
                        <li>Halla n(F ∪ L ∪ B) usando la fórmula extensa.</li>
                        <li>¿Cuántos NO participan en ninguna? ¿Cuántos SOLO en Battle Royale?</li>
                        <li class="text-amber-400"><strong>Reto código:</strong> Identificar a alguien inscrito en los tres.</li>
                    </ol>
                </div>
            </div>

            <div class="mt-8 p-4 bg-emerald-900/30 rounded-lg">
                <h4 class="mt-0 text-emerald-300">📊 Socialización de Resultados</h4>
                <p class="mb-0 text-sm">Cada equipo tendrá <strong>3 minutos</strong> para compartir la respuesta más difícil y su pseudocódigo.</p>
            </div>
        </section>

        <div class="my-16 border-l-4 border-amber-500 bg-amber-950/30 p-8 rounded-r-2xl shadow-lg relative overflow-hidden">
            <div class="absolute -right-10 -top-10 text-9xl opacity-10">☕</div>
            <h3 class="text-amber-400 mt-0 flex items-center gap-3">
                <span class="text-3xl">⏸️</span> DESCANSO 2 — 15 Minutos
            </h3>
            <p class="text-lg">✨ ¡Excelente trabajo colaborativo!</p>
            <p>15 minutos de descanso bien merecidos.</p>
            <ul class="text-amber-200/80">
                <li>Levántate y estírate</li>
                <li>Hidratación y snack si tienes</li>
                <li>Comenta con tu equipo qué fue lo más interesante</li>
            </ul>
            <p class="font-bold text-amber-500 mb-0 mt-4">🎯 Al regresar: ejercicios individuales y reto final.</p>
        </div>

        <section id="ejercicios" class="mt-12">
            <h2>11. ✏️ Ejercicios de Aplicación Individual</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 30 minutos</p>
            <p>Resuelve de forma <strong>individual</strong> en tu cuaderno. Muestra todos los procedimientos. Haz clic para expandir.</p>
            
            <div class="space-y-4 mt-6">
                <div x-data="{ open: false }" class="border border-slate-700 rounded-xl bg-slate-800 overflow-hidden shadow-md">
                    <button @click="open = !open" class="w-full text-left px-6 py-4 font-bold text-lg flex justify-between items-center hover:bg-slate-700 transition">
                        <span>📝 Ejercicio 1 — Operaciones Básicas</span>
                        <span x-text="open ? '−' : '+'" class="text-2xl text-blue-400"></span>
                    </button>
                    <div x-show="open" x-collapse class="px-6 py-4 text-sm bg-slate-900 border-t border-slate-700">
                        <pre class="bg-slate-950"><code>U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
A = {1, 2, 3, 4, 6}
B = {2, 4, 6, 8, 10}
C = {1, 3, 5, 7, 9}</code></pre>
                        <p>Calcula y dibuja el diagrama de Venn para:</p>
                        <ul class="grid grid-cols-2 gap-2">
                            <li>a) \( A \cup B \)</li>
                            <li>b) \( A \cap B \)</li>
                            <li>c) \( A - B \)</li>
                            <li>d) \( B - A \)</li>
                            <li>e) \( A^c \)</li>
                            <li>f) \( (A \cup B)^c \)</li>
                            <li>g) \( A^c \cap B^c \)</li>
                        </ul>
                        <p class="mt-2 text-amber-400 font-bold">h) Verifica De Morgan comparando f y g.</p>
                    </div>
                </div>
                
                <div x-data="{ open: false }" class="border border-slate-700 rounded-xl bg-slate-800 overflow-hidden shadow-md">
                    <button @click="open = !open" class="w-full text-left px-6 py-4 font-bold text-lg flex justify-between items-center hover:bg-slate-700 transition">
                        <span>📝 Ejercicio 2 — Problema Contextualizado</span>
                        <span x-text="open ? '−' : '+'" class="text-2xl text-blue-400"></span>
                    </button>
                    <div x-show="open" x-collapse class="px-6 py-4 text-sm bg-slate-900 border-t border-slate-700">
                        <p>En una encuesta a 50 jóvenes sobre hábitos de estudio:</p>
                        <ul class="list-disc pl-5">
                            <li>28 usan YouTube (Y)</li>
                            <li>22 usan podcasts (P)</li>
                            <li>10 usan ambos</li>
                            <li>El resto no usa ninguno</li>
                        </ul>
                        <ol class="mt-4 space-y-2">
                            <li>Representa en diagrama de Venn.</li>
                            <li>Halla n(Y ∪ P).</li>
                            <li>¿Cuántos usan <strong>solo</strong> YouTube?</li>
                            <li>¿Cuántos no usan ni YT ni podcasts?</li>
                            <li>Halla Yᶜ y explica qué representa.</li>
                            <li>Verifica: n(Y ∪ P) = n(Y) + n(P) - n(Y ∩ P)</li>
                        </ol>
                    </div>
                </div>

                <div x-data="{ open: false }" class="border border-slate-700 rounded-xl bg-slate-800 overflow-hidden shadow-md">
                    <button @click="open = !open" class="w-full text-left px-6 py-4 font-bold text-lg flex justify-between items-center hover:bg-slate-700 transition">
                        <span>📝 Ejercicio 3 — Lógica y Conjuntos</span>
                        <span x-text="open ? '−' : '+'" class="text-2xl text-blue-400"></span>
                    </button>
                    <div x-show="open" x-collapse class="px-6 py-4 text-sm bg-slate-900 border-t border-slate-700">
                        <pre class="bg-slate-950"><code>U = {todos los libros digitales}
F = {libros de ficción}
E = {libros en español}
G = {libros gratuitos}</code></pre>
                        <p>Describe con palabras:</p>
                        <ul class="grid grid-cols-2 gap-2 mb-4">
                            <li>F ∩ E</li>
                            <li>F ∪ G</li>
                            <li>E - G</li>
                            <li>(F ∩ G)ᶜ</li>
                            <li>Fᶜ ∩ Eᶜ</li>
                        </ul>
                        <p class="text-amber-400 font-bold">Reto: Escribe el pseudocódigo para filtrar los libros de ficción en español que sean gratuitos.</p>
                    </div>
                </div>

                <div x-data="{ open: false }" class="border border-slate-700 rounded-xl bg-slate-800 overflow-hidden shadow-md">
                    <button @click="open = !open" class="w-full text-left px-6 py-4 font-bold text-lg flex justify-between items-center hover:bg-slate-700 transition">
                        <span>📝 Ejercicio 4 — Desafío: Leyes de De Morgan</span>
                        <span x-text="open ? '−' : '+'" class="text-2xl text-purple-400"></span>
                    </button>
                    <div x-show="open" x-collapse class="px-6 py-4 text-sm bg-slate-900 border-t border-slate-700">
                        <pre class="bg-slate-950"><code>U = {a, b, c, d, e, f, g, h, i, j}
M = {a, b, c, d, e}
N = {c, d, e, f, g}</code></pre>
                        <ol class="mt-4 grid grid-cols-2 gap-4">
                            <li>Calcula (M ∪ N)ᶜ</li>
                            <li>Calcula Mᶜ ∩ Nᶜ</li>
                            <li>¿Se cumple la 1ra Ley? Justifica.</li>
                            <li>Calcula (M ∩ N)ᶜ</li>
                            <li>Calcula Mᶜ ∪ Nᶜ</li>
                            <li>Verifica la 2da Ley.</li>
                        </ol>
                    </div>
                </div>
            </div>
        </section>

        <section id="reto" class="mt-16 bg-gradient-to-br from-indigo-900/40 to-purple-900/40 p-10 rounded-3xl border border-indigo-500/30 shadow-2xl relative overflow-hidden">
            <div class="absolute right-0 top-0 w-64 h-64 bg-indigo-500/10 rounded-full blur-3xl"></div>
            <h2 class="mt-0 text-indigo-300 border-none">12. 🏅 Reto Final: El Gran Desafío</h2>
            <p class="text-sm font-bold text-indigo-400/80 mb-6">⏱️ Opcional — Para quienes terminen antes</p>
            
            <h3 class="text-white mt-0">🌐 Diseña tu Propio Sistema</h3>
            <p>Crea un sistema digital imaginario que use operaciones de conjuntos (app de tareas, recomendación de series, torneos). Debes:</p>
            <ol class="text-indigo-100/90 space-y-2 relative z-10">
                <li>Definir el <strong>conjunto universo</strong> y al menos <strong>3 conjuntos</strong> relevantes.</li>
                <li>Describir qué representa cada conjunto.</li>
                <li>Plantear <strong>3 situaciones o consultas</strong> que un usuario podría hacer.</li>
                <li>Resolver cada situación usando operaciones de conjuntos.</li>
                <li>Escribir el <strong>pseudocódigo</strong> para al menos una de las consultas.</li>
                <li>Dibujar el <strong>diagrama de Venn</strong> correspondiente.</li>
            </ol>
            <p class="mt-6 text-sm text-indigo-300 italic">💡 Dato: Los mejores sistemas (Netflix, Spotify, Google) aplican estas operaciones millones de veces por segundo.</p>
        </section>

        <section id="cierre" class="mt-16">
            <h2>13. 🎯 Resumen y Cierre</h2>
            <p class="text-sm font-bold text-slate-400">⏱️ Tiempo estimado: 15 minutos</p>
            
            <div class="w-full bg-slate-900 p-6 rounded-xl border border-slate-700 my-8 overflow-x-auto">
                <svg viewBox="0 0 800 220" class="w-full h-auto min-w-[600px] drop-shadow-lg font-sans">
                    <rect x="250" y="10" width="300" height="40" rx="8" fill="#1e293b" stroke="#475569" stroke-width="2"/>
                    <text x="400" y="35" fill="#f8fafc" font-weight="bold" text-anchor="middle" font-size="16">OPERACIONES CON CONJUNTOS</text>

                    <path d="M400 50 v30" stroke="#475569" stroke-width="2" fill="none"/>
                    <path d="M100 80 H700" stroke="#475569" stroke-width="2" fill="none"/>

                    <path d="M100 80 v25" stroke="#475569" stroke-width="2" fill="none"/>
                    <path d="M250 80 v25" stroke="#475569" stroke-width="2" fill="none"/>
                    <path d="M400 80 v25" stroke="#475569" stroke-width="2" fill="none"/>
                    <path d="M550 80 v25" stroke="#475569" stroke-width="2" fill="none"/>
                    <path d="M700 80 v25" stroke="#475569" stroke-width="2" fill="none"/>

                    <polygon points="95,105 105,105 100,110" fill="#475569"/>
                    <polygon points="245,105 255,105 250,110" fill="#475569"/>
                    <polygon points="395,105 405,105 400,110" fill="#475569"/>
                    <polygon points="545,105 555,105 550,110" fill="#475569"/>
                    <polygon points="695,105 705,105 700,110" fill="#475569"/>

                    <rect x="40" y="110" width="120" height="90" rx="8" fill="#1e293b" stroke="#3b82f6" stroke-width="2"/>
                    <text x="100" y="135" fill="#60a5fa" font-weight="bold" text-anchor="middle">UNIÓN</text>
                    <text x="100" y="160" fill="#ffffff" text-anchor="middle" font-size="18">A ∪ B</text>
                    <text x="100" y="185" fill="#cbd5e1" font-size="13" font-family="monospace" text-anchor="middle">OR / ||</text>

                    <rect x="190" y="110" width="120" height="90" rx="8" fill="#1e293b" stroke="#10b981" stroke-width="2"/>
                    <text x="250" y="135" fill="#34d399" font-weight="bold" text-anchor="middle">INTERSECCIÓN</text>
                    <text x="250" y="160" fill="#ffffff" text-anchor="middle" font-size="18">A ∩ B</text>
                    <text x="250" y="185" fill="#cbd5e1" font-size="13" font-family="monospace" text-anchor="middle">AND / &amp;&amp;</text>

                    <rect x="340" y="110" width="120" height="90" rx="8" fill="#1e293b" stroke="#ef4444" stroke-width="2"/>
                    <text x="400" y="135" fill="#f87171" font-weight="bold" text-anchor="middle">DIFERENCIA</text>
                    <text x="400" y="160" fill="#ffffff" text-anchor="middle" font-size="18">A - B</text>
                    <text x="400" y="185" fill="#cbd5e1" font-size="13" font-family="monospace" text-anchor="middle">AND + NOT</text>

                    <rect x="490" y="110" width="120" height="90" rx="8" fill="#1e293b" stroke="#a855f7" stroke-width="2"/>
                    <text x="550" y="135" fill="#c084fc" font-weight="bold" text-anchor="middle">COMPLEMENTO</text>
                    <text x="550" y="160" fill="#ffffff" text-anchor="middle" font-size="18">Aᶜ</text>
                    <text x="550" y="185" fill="#cbd5e1" font-size="13" font-family="monospace" text-anchor="middle">NOT / !</text>

                    <rect x="640" y="110" width="120" height="90" rx="8" fill="#1e293b" stroke="#f59e0b" stroke-width="2"/>
                    <text x="700" y="135" fill="#fbbf24" font-weight="bold" text-anchor="middle">DE MORGAN</text>
                    <text x="700" y="160" fill="#ffffff" text-anchor="middle" font-size="14">Leyes</text>
                    <text x="700" y="185" fill="#cbd5e1" font-size="11" font-family="monospace" text-anchor="middle">!(A||B)=!A&amp;&amp;!B</text>
                </svg>
            </div>

            <div class="bg-slate-800 p-8 rounded-2xl border border-slate-600 shadow-xl my-8">
                <h3 class="mt-0 text-2xl text-white">✅ Lista de Verificación de Aprendizaje</h3>
                <p class="text-sm text-slate-400 mb-6">Marca con honestidad cada ítem que puedas hacer con confianza:</p>
                <ul class="space-y-3 list-none pl-0">
                    <template x-data="{ items: [
                        'Puedo listar los elementos de la unión sin repetir',
                        'Puedo identificar correctamente elementos de la intersección',
                        'Puedo calcular A - B y B - A y entender por qué son diferentes',
                        'Sé calcular el complemento dado un universo',
                        'Conozco y puedo verificar las Leyes de De Morgan',
                        'Sé dibujar diagramas de Venn para dos o tres conjuntos',
                        'Puedo relacionar operaciones con operadores lógicos en código',
                        'Puedo escribir pseudocódigo con condiciones basadas en conjuntos'
                    ] }" x-for="(item, index) in items" :key="index">
                        <li x-data="{ checked: false }" 
                            @click="checked = !checked" 
                            class="flex items-center gap-4 p-4 bg-slate-900/80 rounded-xl cursor-pointer border border-slate-700 hover:border-blue-500 transition-all select-none">
                            <div class="w-7 h-7 rounded border-2 flex items-center justify-center flex-shrink-0 transition-colors" :class="checked ? 'bg-green-500 border-green-500' : 'bg-slate-800 border-slate-500'">
                                <svg x-show="checked" class="w-5 h-5 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M5 13l4 4L19 7"></path></svg>
                            </div>
                            <span class="text-[15px]" :class="checked ? 'line-through text-slate-500' : 'text-slate-200'" x-text="item"></span>
                        </li>
                    </template>
                </ul>
            </div>

            <div class="p-6 bg-slate-800/50 rounded-xl border-l-4 border-blue-500 mb-12">
                <h3 class="mt-0 text-blue-400">🗣️ Reflexión Final</h3>
                <p class="mb-0 italic">"¿En qué aspecto de tu vida diaria o en qué tecnología que uses regularmente crees que se aplican las operaciones con conjuntos? ¿Por qué crees que los programadores necesitan dominar estas operaciones?"</p>
                <p class="text-sm mt-2 text-slate-400">Responde en tu cuaderno (3–4 oraciones).</p>
            </div>
        </section>

        <hr class="border-slate-700 my-12">
        <section class="grid md:grid-cols-2 gap-12 text-sm text-slate-400">
            <div>
                <h3 class="text-slate-300 mt-0">📖 Glosario</h3>
                <ul class="space-y-2">
                    <li><strong>Conjunto:</strong> Colección bien definida de elementos.</li>
                    <li><strong>Universo (U):</strong> Todos los elementos posibles en un contexto.</li>
                    <li><strong>Cardinalidad:</strong> Número de elementos. Se denota n(A).</li>
                    <li><strong>Conjuntos disjuntos:</strong> Intersección vacía.</li>
                    <li><strong>Operador lógico:</strong> Símbolo (AND, OR, NOT) en programación.</li>
                    <li><strong>Pseudocódigo:</strong> Descripción textual de un algoritmo.</li>
                </ul>
            </div>
            <div>
                <h3 class="text-slate-300 mt-0">📚 Referencias</h3>
                <ul class="space-y-2">
                    <li>📺 <strong>YouTube:</strong> "Operaciones con conjuntos - Khan Academy"</li>
                    <li>🌐 <strong>GeoGebra:</strong> Diagramas interactivos (geogebra.org)</li>
                    <li>📖 <strong>Libro:</strong> Matemáticas Discretas (Cap. Teoría de Conjuntos)</li>
                </ul>
                <h4 class="text-amber-400 mt-6 mb-2">🐍 Conjuntos en Python (Para casa)</h4>
                <pre class="bg-slate-900 p-3 rounded text-xs border border-slate-700"><code>A = {1, 2, 3, 4, 5}
B = {3, 4, 5, 6, 7}

print(A | B) # Unión → {1..7}
print(A & B) # Intersección → {3..5}
print(A - B) # Diferencia → {1, 2}</code></pre>
            </div>
        </section>

        <footer class="mt-16 text-center text-xs text-slate-600 border-t border-slate-800 pt-8">
            <p>Material elaborado con fines educativos. Diseñado bajo principios de aprendizaje activo y pensamiento computacional.</p>
            <p>Licencia: CC BY-NC-SA 4.0 | Versión 1.0 — Marzo 2026</p>
        </footer>

    </main>
</body>
</html>