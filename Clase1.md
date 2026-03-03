# Módulo: Herramientas Lógico Matemáticas
## Sesión 1: El Código Oculto del Software (Introducción a la Lógica y los Números)

**Duración total:** 2 horas y 15 minutos (135 minutos)
**Público:** Estudiantes de desarrollo de software (aprox. 15 años)

---

### 📋 Tabla de Contenido de la Sesión

| Actividad | Descripción | Tiempo |
| :--- | :--- | :--- |
| **0. Introducción** | ¿Por qué un programador necesita lógica? | 15 min |
| **1. Lectura Guiada** | El origen de los números y el conteo. | 30 min |
| **2. Socialización** | Lógica en la vida cotidiana. | 30 min |
| **3. Pausa Activa** | Descanso mental. | 10 min |
| **4. Taller Diagnóstico** | Retos de pensamiento computacional. | 40 min |
| **5. Cierre** | Conclusiones y próximos pasos. | 10 min |

---

### 0. Introducción: ¿Por qué estamos aquí? (15 min)

Bienvenidos al mundo del desarrollo de software. Probablemente están aquí porque quieren crear aplicaciones, videojuegos o páginas web. Pero antes de escribir código en lenguajes como Python, JavaScript o Rust, necesitamos entender el "idioma" real de las computadoras: **La Lógica**.

La computadora no es inteligente por sí sola; es una máquina que sigue instrucciones de forma extremadamente rápida. Nuestro trabajo como desarrolladores es darle esas instrucciones de forma lógica y sin ambigüedades. Las **matemáticas discretas** nos enseñan a pensar de esta manera. Nos ayudan a tomar decisiones (si pasa esto, haz aquello), a contar, a agrupar datos y a diseñar los algoritmos que mueven el mundo digital.

---

### 1. Actividad 1: Lectura Guiada - El Origen de los Números (30 min)

**Instrucción para el profesor:** Leer el siguiente texto de forma compartida con los alumnos, haciendo pausas para asegurar la comprensión.

> **De los Huesos a los Bits: Una breve historia del conteo**
>
> Imagina que eres un pastor hace 20,000 años. Necesitas saber si todas tus ovejas regresaron a salvo. No conoces el número "50", ni tienes palabras para describirlo. ¿Qué haces?
> 
> Nuestros antepasados resolvieron esto con el **principio de correspondencia uno a uno**. Por cada oveja que entraba, hacían una marca en un hueso o guardaban una piedra en una bolsa.
>
> 
> 
> Con el tiempo, las civilizaciones crecieron. Los babilonios, los egipcios y los romanos inventaron símbolos para representar cantidades mayores sin tener que cargar bolsas llenas de piedras. 
> 
> Más adelante en la historia, en la India, se consolidó uno de los mayores inventos de la humanidad: **el número cero (0)**. Antes de esto, el vacío o la "ausencia de cantidad" no se consideraba un número. El cero permitió crear el sistema decimal (Base 10) que usamos hoy en día.
>
> **¿Y qué tiene que ver esto con las computadoras?**
> Años más tarde, los matemáticos se dieron cuenta de que no necesitábamos 10 símbolos (0 al 9) para contar. Podíamos hacerlo solo con dos: el **0** y el **1**. Así nació el **sistema binario**. La electrónica moderna funciona abriendo y cerrando circuitos (encendido = 1, apagado = 0). Toda la información en tu teléfono (mensajes, fotos, videos, juegos) en su nivel más profundo, es solo una inmensa combinación de ceros y unos viajando a la velocidad de la luz.

**Preguntas para reflexionar en clase:**
* ¿Por qué creen que el ser humano adoptó el sistema de Base 10 para la vida diaria? (Pista: miren sus manos).
* ¿Qué pasaría si intentáramos programar computadoras usando un sistema de 10 voltajes diferentes en lugar de solo 2 (encendido/apagado)?

---

### 2. Actividad 2: Socialización - Lógica en la Vida Cotidiana (30 min)

**Instrucción:** Dividir a los estudiantes en grupos de 3 o 4. 

La programación no es solo matemáticas; es encontrar la secuencia lógica correcta para resolver un problema. A esto lo llamamos **Algoritmo**. Sin saberlo, ustedes ejecutan algoritmos complejos todos los días.

**El Reto:**
Discutan en su grupo y escriban los "pasos lógicos" (el algoritmo) para una de las siguientes situaciones cotidianas. Deben ser tan precisos que hasta un robot sin sentido común pueda seguirlos sin equivocarse.

* *Opción A:* Preparar un sándwich de mantequilla de maní y mermelada (o fruta).
* *Opción B:* El proceso mental y las condiciones para decidir qué ropa ponerse antes de salir de casa (evaluando el clima, si hay educación física, etc.).
* *Opción C:* Cómo ganar una partida en su videojuego favorito paso a paso.

**Socialización:**
Cada grupo compartirá su algoritmo. El resto de la clase jugará a ser la "computadora" y buscará errores de lógica (bugs) en las instrucciones de sus compañeros. (Por ejemplo: *"¡Error! Dijiste poner la mantequilla de maní en el pan, pero nunca dijiste que había que abrir el frasco primero"*).



---

### 3. Pausa Activa (10 min)
Espacio para estirarse, tomar agua y despejar la mente antes del reto final.

---

### 4. Actividad 3: Taller Diagnóstico de Lógica (40 min)

**Instrucción:** Este taller no tiene nota evaluativa; su propósito es conocer cómo razonan ante problemas nuevos. Pueden resolverlo de forma individual o en parejas. ¡No busquen las respuestas en internet, confíen en su cerebro!

**Reto 1: Reconocimiento de Patrones**
Los programadores son, ante todo, buscadores de patrones. Observa la siguiente secuencia y determina qué número sigue. Explica tu razonamiento.
* 2, 4, 8, 16, __, __

**Reto 2: Lógica Condicional (Verdadero / Falso)**
Estás desarrollando un sistema de seguridad para una página web. Tienes tres usuarios sospechosos (A, B y C) y sabes las siguientes reglas:
1. Si A es un hacker, entonces B también lo es.
2. C nunca trabaja con B.
3. Sabemos con certeza que C es un hacker.
*Pregunta:* ¿Es A un hacker? (Escribe el porqué de tu deducción paso a paso).

**Reto 3: El problema del río (Secuenciación)**
Un campesino debe cruzar un río en una pequeña balsa con un zorro, una gallina y un saco de maíz. 
* La balsa solo soporta al campesino y a un elemento más.
* Si el campesino los deja solos, el zorro se comerá a la gallina.
* Si el campesino los deja solos, la gallina se comerá el maíz.
*Pregunta:* Diseña la secuencia exacta de viajes (ida y vuelta) que el campesino debe hacer para pasar todo al otro lado intacto.

---

### 5. Cierre y Conclusiones (10 min)

* **Puesta en común:** Revisión rápida de las soluciones del taller diagnóstico.
* **Conclusión del día:** Escribir código es fácil, la sintaxis se aprende en internet. Lo verdaderamente valioso de un desarrollador de software es su capacidad analítica y lógica. Las matemáticas que veremos aquí son sus herramientas para construir una mente estructurada.
* **Preparación para la próxima clase:** Piensen en cuántos dispositivos a su alrededor usan sistemas digitales (binarios) frente a sistemas analógicos.