# La Lógica en Mi Vida Cotidiana

*Ensayo para estudiantes de desarrollo de software (15-17 años)*

---

## Introducción

Cuando pensamos en "lógica", quizás lo primero que nos viene a la mente son fórmulas complicadas, tablas de verdad o ejercicios de matemáticas que parecían no tener fin. Sin embargo, la lógica no vive solo en el pizarrón: **está presente en cada decisión que tomamos cada día**. Desde decidir si llevar paraguas hasta elegir qué aplicación usar para enviar un mensaje, nuestro cerebro procesa condiciones, evalúa opciones y llega a conclusiones. En este ensayo quiero compartir cómo la lógica discreta — aquella que estudiamos en clase — ha cambiado mi forma de ver el mundo que me rodea.

---

## 1. Teoría de conjuntos: clasificar y organizar

La teoría de conjuntos es quizás uno de los conceptos más poderosos y a la vez más intuitivos que aprendimos. Un **conjunto** es simplemente una colección de elementos con características comunes.

**Ejemplos cotidianos:**

- El conjunto de mis amigos cercanos
- El conjunto de aplicaciones en mi teléfono
- El conjunto de números pares

**Operaciones con conjuntos:**

| Operación | Símbolo | Ejemplo en la vida real |
|:---:|:---:|:---|
| **Unión** | ∪ | "Quiero pizza o hamburguesa" → elementos de ambos conjuntos |
| **Intersección** | ∩ | "Amigos que juegan fútbol Y programan" → solo los que cumplen ambas |
| **Complemento** | A' o Ā | "Todos los colores EXCEPTO el negro" |
| **Diferencia** | − | "Frutas que NO son cítricas" |

**¿Por qué es importante en software?**

Cada vez que creamos una lista, un menú, un filtro o una base de datos, estamos trabajando con conjuntos. Cuando YouTube me recomienda videos basados en "usuarios que vieron esto también vieron...", está usando operaciones de intersección y unión entre conjuntos de preferencias. Cuando filtras tweets por hashtag y por fecha, estás haciendo una intersección de conjuntos.

En programación, los conjuntos se convierten en:
- **Arrays y listas** (estructuras de datos)
- **Filtros de búsqueda** (base de datos)
- **Permisos de usuario** (¿este usuario pertenece al conjunto de admins?)

```python
# Ejemplo en Python
admins = {"juan", "maria", "pedro"}
editores = {"ana", "pedro", "luis"}

# Intersección: ¿quiénes son admins Y editores?
admins_y_editores = admins & editores  # Resultado: {"pedro"}

# Unión: ¿quiénes son admins O editores?
todos_los_roles = admins | editores   # Resultado: {"juan", "maria", "pedro", "ana", "luis"}
```

---

## 2. Condicionales: "Si pasa esto, entonces hago aquello"

Los condicionales son quizás la estructura lógica más natural que usamos sin darnos cuenta. Un condicional tiene la forma **"Si A, entonces B"** (A → B).

**Ejemplo en mi vida:**

- *Si no llueve mañana, entonces voy a la playa con mis amigos.*
- *Si mi equipo favorito pierde, entonces no veo el partido completo.*
- *Si estudio para el examen, entonces tendré mejores probabilidades de aprobar.*

Cuando analizo un condicional, entiendo que no importa el resultado final, sino la relación entre la causa y la consecuencia. En programación, estos condicionales son la base de estructuras como `if` y `else`. Cuando escribo:

```javascript
if (llueve == true) {
    llevarParaguas();
} else {
    irAPlaya();
}
```

Estoy aplicando exactamente la misma lógica que uso cuando decido mi outfit por la mañana según el clima.

---

## 3. Conectores lógicos: Y, O, NO

En matemáticas discretas aprendimos tres conectores fundamentales: **Y (∧), O (∨) y NO (¬)**. Estos también aparecen constantemente en nuestra vida diaria.

**Conector Y (ambos deben cumplirse):**
> "Puedo ir al cine *y* comprar palomitas *si* tengo dinero *y* tiempo libre."
> Ambas condiciones deben ser verdaderas para que la acción ocurra.

**Conector O (al menos uno debe cumplirse):**
> "Para el cumpleaños puedo regalar un juego *o* un libro *o* una camiseta."
> No necesito ambos, con cualquiera de las opciones es suficiente.

**Conector NO (niega la condición):**
> "NO voy a la fiesta si no termino mi proyecto."
> Invierte la condición: lo que era verdadero se vuelve falso y viceversa.

Estos conectores son los mismos que usamos para construir consultas en bases de datos, filtros en redes sociales o condiciones en nuestro código.

---

## 4. Tablas de verdad: anticipar resultados

Antes de escribir código, un buen desarrollador piensa en **todos los posibles casos** que pueden ocurrir. Las tablas de verdad nos enseñan a hacer exactamente eso.

Pensemos en la siguiente situación:

> **"Puedo salir de casa si tengo permiso de mis papás Y hace buen tiempo"**

| Tengo permiso | Hace buen tiempo | Puedo salir |
|:---:|:---:|:---:|
| V | V | **V** |
| V | F | **F** |
| F | V | **F** |
| F | F | **F** |

Solo cuando **ambas condiciones son verdaderas**, el resultado es verdadero. Esto es exactamente lo que hace un sistema cuando verifica que un usuario esté autenticado Y tenga permisos de administrador antes de mostrar cierta información.

---

## 5. El poder del razonamiento inverso

Una de las habilidades más útiles que nos da la lógica es el **razonamiento inverso**: si queremos un resultado específico, ¿qué condiciones deben cumplirse?

**Ejemplo:** Si quiero que mi mamá me deje ir a la fiesta:
- Debo haber cumplido con mis tareas → Tarea completada = V
- Debo haber llegado a tiempo en las últimas ocasiones → Puntual = V
- Debo ofrecer algo a cambio (lavar los trastes por una semana) → Ofrezco algo = V

Si alguna de estas es falsa, la conclusión también lo será. En programación, esto se traduce en validar todos los campos de un formulario antes de enviarlo: si algún dato es inválido, **no se cumple la condición de éxito**.

---

## 6. Lógica y pensamiento crítico

La lógica también nos protege de los **razonamientos incorrectos** que encontramos a diario, especialmente en redes sociales. Nos enseñan a preguntar:

- ¿Esta información es realmente correcta o es una falacia?
- Si "todos lo están haciendo", ¿significa que está bien? (No: *ad populum* es una falácia)
- Si algo pasó después de un evento, ¿realmente lo causó? (No confundir correlación con causalidad)

Ser capaz de evaluar argumentos con las herramientas de la lógica nos hace mejores desarrolladores *y* mejores ciudadanos.

---

## Conclusión

La lógica no es solo un tema de un examen: es **la herramienta que nuestro cerebro usa para navegar el mundo**. Cada vez que tomamos una decisión, evaluamos una situación o resolvemos un problema, estamos aplicando principios lógicos — quizás sin escribirlos en símbolos formales.

Como futuros desarrolladores de software, entender la lógica formalmente nos da un superpoder: podemos expresar nuestros pensamientos de manera precisa, anticipar errores y construir programas que funcionen correctamente bajo **cualquier** combinación de condiciones.

Así que la próxima vez que pienses "si estudio, entonces aprobo", recuerda: estás pensando como un lógico. Y eso, amigo desarrollador, es algo muy importante.

---

## Taller de Ejercicios

**Instrucciones:** Resuelve cada ejercicio mostrando tu razonamiento. Los ejercicios combinan situaciones de la vida cotidiana con situaciones de programación.

---

### Ejercicio 1 — Teoría de conjuntos (10 puntos)

Dado los siguientes conjuntos:

```
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}
C = {2, 4, 6, 8}
```

Calcula:

a) A ∪ B = _______________

b) A ∩ B = _______________

c) B ∩ C = _______________

d) A − B = _______________

e) C' (complemento de C, considerando el universo U = {1, 2, 3, 4, 5, 6, 7, 8}) = _______________

---

### Ejercicio 2 — Condicionales (10 puntos)

Traduce las siguientes situaciones a código usando `if / else`:

a) "Si tengo al menos 18 años, puedo crear una cuenta en la plataforma; de lo contrario, necesito permiso de mis padres."
   ```javascript
   // Tu código aquí
   ```

b) "Si el usuario existe Y la contraseña es correcta, mostrar 'Bienvenido'; de lo contrario, mostrar 'Acceso denegado'."
   ```javascript
   // Tu código aquí
   ```

---

### Ejercicio 3 — Tablas de verdad (10 puntos)

Construye la tabla de verdad para cada una de las siguientes expresiones:

a) **(A ∧ B) → C**

| A | B | C | A ∧ B | (A ∧ B) → C |
|:---:|:---:|:---:|:---:|:---:|
| V | V | V | | |
| V | V | F | | |
| V | F | V | | |
| V | F | F | | |
| F | V | V | | |
| F | V | F | | |
| F | F | V | | |
| F | F | F | | |

b) **¬(A ∨ B)**

| A | B | A ∨ B | ¬(A ∨ B) |
|:---:|:---:|:---:|:---:|
| V | V | | |
| V | F | | |
| F | V | | |
| F | F | | |

---

### Ejercicio 4 — Conectores lógicos en contexto (10 puntos)

Une cada situación de la vida real con la expresión lógica correcta:

| Situación | Expresión lógica |
|---|---|
| 1. "Para graduarse se necesita inglés Y matemáticas" | a) A ∨ B |
| 2. "El evento es gratis para niños O para adultos mayores" | b) A ∧ B |
| 3. "No puedes entrar si no tienes boleto" | c) ¬A → ¬B |
| 4. "Si no estudias, no apruebas" (contraposición) | d) ¬(A ∧ B) |
| 5. "Puedes elegir pizza o arroz" | e) A ∨ B (solo uno) |

---

### Ejercicio 5 — Razonamiento inverso (10 puntos)

Eres desarrollador y un usuario no puede iniciar sesión en tu sistema. Aplica razonamiento inverso para identificar qué condiciones deben cumplirse para que el login sea exitoso.

**Condiciones necesarias:**
- El usuario debe estar registrado
- La contraseña debe ser correcta
- La cuenta no debe estar bloqueada

Si el login falla, ¿cuál podría ser la causa? Completa la tabla:

| Usuario registrado | Contraseña correcta | Cuenta no bloqueada | ¿Login exitoso? | Causa del fallo |
|:---:|:---:|:---:|:---:|:---|
| V | V | V | **Sí** | Ninguna |
| V | V | F | **No** | ____________ |
| V | F | V | **No** | ____________ |
| F | V | V | **No** | ____________ |

---

### Ejercicio 6 — Pensamiento crítico (10 puntos)

Identifica si cada argumento es válido o es una falacia lógica. Explica por qué:

a) "El 90% de los usuarios usan Google Chrome, entonces Chrome debe ser el mejor navegador."
   - **Respuesta:** _________________________
   - **Explicación:** _________________________

b) "Si mañana hace sol, iré al parque. Mañana hace sol. Por lo tanto, iré al parque."
   - **Respuesta:** _________________________
   - **Explicación:** _________________________

---

### Ejercicio de desafío — Crea tu propio ejemplo (10 puntos)

Diseña una situación de la vida cotidiana (puede ser sobre redes sociales, videojuegos, escuela o amigos) que involucre:

- Al menos un condicional (Si... entonces...)
- Al menos un conector lógico (Y, O, NO)
- Al menos una operación con conjuntos

**Ejemplo redactado:**
_______________________________________________

**Traducción a código:**
```javascript
// Tu código aquí
```

---

**Total: 60 puntos**

*¡Buena suerte! Remember: la lógica está en todo lo que haces.*

---

*Actividad de cierre — Módulo de Matemáticas Discretas*
