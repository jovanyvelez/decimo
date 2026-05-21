# Clase de Algoritmos: Contadores, Acumuladores y Banderas

**Duración:** 3 horas · **Audiencia:** Jóvenes de 15 a 17 años  
**Lenguajes:** PSeInt + C# · **Modalidad:** Resolución colaborativa en pizarra

---

## Estructura de la clase

| Sección | Tema | Tiempo |
|---------|------|--------|
| 1 | Introducción y conceptos | 25 min |
| 2 | Contadores | 35 min |
| 3 | Acumuladores | 35 min |
| 4 | Banderas (flags) | 35 min |
| 5 | Combinación de técnicas | 30 min |
| 6 | Taller práctico integrador | 20 min |

---

## 1. Introducción y conceptos (25 min)

### 1.1. ¿Por qué necesitamos estos conceptos?

Imagina que eres el portero de un concierto. Necesitas:

- **Contar** cuántas personas entran (contador)
- **Sumar** el dinero recaudado (acumulador)
- **Saber si** ya se llenó el aforo para cerrar puertas (bandera)

Estas tres ideas son la base de muchísimos algoritmos.

### 1.2. Definiciones en pizarra

| Concepto | Definición | Analogía |
|----------|-----------|----------|
| **Contador** | Variable que se incrementa en una cantidad fija (generalmente +1) | Conteo de goles en un partido |
| **Acumulador** | Variable que suma cantidades variables | Total de una cuenta de supermercado |
| **Bandera** | Variable booleana que indica si ocurrió un evento | Semáforo: verde = sigue, rojo = para |

### 1.3. Actividad rápida (5 min)

> **Pregunta al grupo:** En un videojuego de plataformas, ¿qué serían?
> - Las vidas restantes → contador (decreciente)
> - El puntaje total → acumulador
> - Si el jugador tiene escudo activo → bandera

---

## 2. Contadores (35 min)

### 2.1. Concepto

**PSeInt:**
```
Definir contador Como Entero
contador <- 0                // Inicialización (SIEMPRE)
contador <- contador + 1     // Incremento
```

**C#:**
```csharp
int contador = 0;           // Inicialización (SIEMPRE)
contador = contador + 1;    // Incremento
contador++;                 // Incremento abreviado
contador += 1;              // Otra forma abreviada
```

### 2.2. Ejemplo 1 — Contar números pares ingresados

**Problema:** El usuario ingresa N números. Contar cuántos son pares.

**PSeInt:**
```
Algoritmo ContarPares
    Definir n, num, contadorPares Como Entero
    Definir i Como Entero

    Escribir "¿Cuántos números ingresarás? "
    Leer n

    contadorPares <- 0

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        Si num MOD 2 == 0 Entonces
            contadorPares <- contadorPares + 1
        FinSi
    FinPara

    Escribir "Cantidad de números pares: ", contadorPares
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("¿Cuántos números ingresarás? ");
int n = int.Parse(Console.ReadLine());

int contadorPares = 0;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    if (num % 2 == 0)
    {
        contadorPares++;
    }
}

Console.WriteLine($"Cantidad de números pares: {contadorPares}");
```

### 2.3. Ejemplo 2 — Contar aprobados y reprobados

**PSeInt:**
```
Algoritmo AprobadosReprobados
    Definir aprobados, reprobados Como Entero
    Definir nota Como Real
    Definir i Como Entero

    aprobados <- 0
    reprobados <- 0

    Para i <- 1 Hasta 10 Con Paso 1 Hacer
        Escribir "Nota del estudiante ", i, ": "
        Leer nota

        Si nota >= 6.0 Entonces
            aprobados <- aprobados + 1
        Sino
            reprobados <- reprobados + 1
        FinSi
    FinPara

    Escribir "Aprobados: ", aprobados, " | Reprobados: ", reprobados
FinAlgoritmo
```

**C#:**
```csharp
int aprobados = 0, reprobados = 0;

for (int i = 1; i <= 10; i++)
{
    Console.Write($"Nota del estudiante {i}: ");
    double nota = double.Parse(Console.ReadLine());

    if (nota >= 6.0)
        aprobados++;
    else
        reprobados++;
}

Console.WriteLine($"Aprobados: {aprobados} | Reprobados: {reprobados}");
```

### 2.4. Ejercicios para pizarra — Contadores

Resuelvan juntos en la pizarra, escribiendo código paso a paso (primero PSeInt, luego lo pasan a C#):

**Ejercicio 2A.** Leer 15 números e indicar cuántos son negativos.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo ContarNegativos
    Definir num, contNegativos Como Entero
    Definir i Como Entero

    contNegativos <- 0

    Para i <- 1 Hasta 15 Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        Si num < 0 Entonces
            contNegativos <- contNegativos + 1
        FinSi
    FinPara

    Escribir "Cantidad de números negativos: ", contNegativos
FinAlgoritmo
```

**C#:**
```csharp
int contNegativos = 0;

for (int i = 1; i <= 15; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    if (num < 0)
        contNegativos++;
}

Console.WriteLine($"Cantidad de números negativos: {contNegativos}");
```
</details>

**Ejercicio 2B.** Leer N números y contar cuántos están entre 10 y 50 (inclusive).

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo ContarEnRango
    Definir n, num, contRango Como Entero
    Definir i Como Entero

    Escribir "¿Cuántos números? "
    Leer n

    contRango <- 0

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        Si num >= 10 Y num <= 50 Entonces
            contRango <- contRango + 1
        FinSi
    FinPara

    Escribir "Cantidad en rango [10, 50]: ", contRango
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("¿Cuántos números? ");
int n = int.Parse(Console.ReadLine());

int contRango = 0;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    if (num >= 10 && num <= 50)
        contRango++;
}

Console.WriteLine($"Cantidad en rango [10, 50]: {contRango}");
```
</details>

**Ejercicio 2C.** Leer 20 edades. Contar cuántos son menores de edad (<18), cuántos son adultos jóvenes (18-35) y cuántos son mayores de 35.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo CategoriasEdad
    Definir edad, menores, jovenes, mayores Como Entero
    Definir i Como Entero

    menores <- 0
    jovenes <- 0
    mayores <- 0

    Para i <- 1 Hasta 20 Con Paso 1 Hacer
        Escribir "Edad persona ", i, ": "
        Leer edad

        Si edad < 18 Entonces
            menores <- menores + 1
        Sino
            Si edad <= 35 Entonces
                jovenes <- jovenes + 1
            Sino
                mayores <- mayores + 1
            FinSi
        FinSi
    FinPara

    Escribir "Menores de edad: ", menores
    Escribir "Adultos jóvenes (18-35): ", jovenes
    Escribir "Mayores de 35: ", mayores
FinAlgoritmo
```

**C#:**
```csharp
int menores = 0, jovenes = 0, mayores = 0;

for (int i = 1; i <= 20; i++)
{
    Console.Write($"Edad persona {i}: ");
    int edad = int.Parse(Console.ReadLine());

    if (edad < 18)
        menores++;
    else if (edad <= 35)
        jovenes++;
    else
        mayores++;
}

Console.WriteLine($"Menores de edad: {menores}");
Console.WriteLine($"Adultos jóvenes (18-35): {jovenes}");
Console.WriteLine($"Mayores de 35: {mayores}");
```
</details>

**Ejercicio 2D.** Leer N caracteres (letras). Contar cuántas vocales hay.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo ContarVocales
    Definir n, contVocales Como Entero
    Definir letra Como Caracter
    Definir i Como Entero

    Escribir "¿Cuántas letras ingresarás? "
    Leer n

    contVocales <- 0

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Letra ", i, ": "
        Leer letra

        letra <- Mayusculas(letra)

        Si letra == "A" O letra == "E" O letra == "I" O letra == "O" O letra == "U" Entonces
            contVocales <- contVocales + 1
        FinSi
    FinPara

    Escribir "Cantidad de vocales: ", contVocales
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("¿Cuántas letras ingresarás? ");
int n = int.Parse(Console.ReadLine());
int contVocales = 0;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Letra {i}: ");
    char letra = char.ToUpper(Console.ReadKey().KeyChar);
    Console.WriteLine();

    if (letra == 'A' || letra == 'E' || letra == 'I' || letra == 'O' || letra == 'U')
        contVocales++;
}

Console.WriteLine($"Cantidad de vocales: {contVocales}");
```
</details>

---

## 3. Acumuladores (35 min)

### 3.1. Concepto

**PSeInt:**
```
Definir acumulador Como Real
acumulador <- 0              // Inicialización (SIEMPRE)
acumulador <- acumulador + valor   // Acumulación
```

**C#:**
```csharp
double acumulador = 0;              // Inicialización
acumulador = acumulador + valor;    // Acumulación
acumulador += valor;                // Forma abreviada
```

### 3.2. Ejemplo 3 — Promedio de notas

**PSeInt:**
```
Algoritmo PromedioNotas
    Definir n Como Entero
    Definir nota, suma, promedio Como Real
    Definir i Como Entero

    Escribir "Cantidad de notas: "
    Leer n

    suma <- 0

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Nota ", i, ": "
        Leer nota
        suma <- suma + nota
    FinPara

    promedio <- suma / n
    Escribir "Promedio: ", promedio
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("Cantidad de notas: ");
int n = int.Parse(Console.ReadLine());

double suma = 0;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Nota {i}: ");
    double nota = double.Parse(Console.ReadLine());
    suma += nota;
}

double promedio = suma / n;
Console.WriteLine($"Promedio: {promedio:F2}");
```

### 3.3. Ejemplo 4 — Total de una compra con IVA

**PSeInt:**
```
Algoritmo CompraConIVA
    Definir precio, total, iva, totalFinal Como Real
    Definir cantidad Como Entero
    Definir respuesta Como Caracter

    total <- 0

    Repetir
        Escribir "Precio del producto: "
        Leer precio
        Escribir "Cantidad: "
        Leer cantidad

        total <- total + (precio * cantidad)

        Escribir "¿Agregar otro producto? (s/n): "
        Leer respuesta
    Hasta Que Minusculas(respuesta) <> "s"

    iva <- total * 0.21
    totalFinal <- total + iva

    Escribir "Subtotal: $", total
    Escribir "IVA (21%): $", iva
    Escribir "Total: $", totalFinal
FinAlgoritmo
```

**C#:**
```csharp
double total = 0;
string respuesta;

do
{
    Console.Write("Precio del producto: ");
    double precio = double.Parse(Console.ReadLine());
    Console.Write("Cantidad: ");
    int cantidad = int.Parse(Console.ReadLine());

    total += precio * cantidad;

    Console.Write("¿Agregar otro producto? (s/n): ");
    respuesta = Console.ReadLine();

} while (respuesta.ToLower() == "s");

double iva = total * 0.21;
double totalFinal = total + iva;

Console.WriteLine($"Subtotal: {total:C}");
Console.WriteLine($"IVA (21%): {iva:C}");
Console.WriteLine($"Total: {totalFinal:C}");
```

### 3.4. Diferencia clave: Contador vs Acumulador

> **Actividad en pizarra:** Dibujar dos columnas y que los estudiantes digan diferencias.

| Contador | Acumulador |
|----------|------------|
| Incremento fijo (+1, +2) | Incremento variable |
| Cuenta elementos | Suma valores |
| Suele ser Entero | Puede ser Entero, Real |
| Ej PSeInt: `cont <- cont + 1` | Ej PSeInt: `suma <- suma + nota` |
| Ej C#: `contador++` | Ej C#: `suma += nota` |

### 3.5. Ejercicios para pizarra — Acumuladores

**Ejercicio 3A.** Leer N precios de productos y mostrar el total a pagar.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo TotalPrecios
    Definir n Como Entero
    Definir precio, total Como Real
    Definir i Como Entero

    Escribir "Cantidad de productos: "
    Leer n

    total <- 0

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Precio producto ", i, ": "
        Leer precio
        total <- total + precio
    FinPara

    Escribir "Total a pagar: $", total
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("Cantidad de productos: ");
int n = int.Parse(Console.ReadLine());

double total = 0;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Precio producto {i}: ");
    double precio = double.Parse(Console.ReadLine());
    total += precio;
}

Console.WriteLine($"Total a pagar: {total:C}");
```
</details>

**Ejercicio 3B.** Leer 10 temperaturas en °C y mostrar el promedio. Además, mostrar cuántas temperaturas superaron el promedio.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo Temperaturas
    Definir temp, suma, promedio Como Real
    Definir contSuperan Como Entero
    Definir i Como Entero
    Dimension temperaturas[10]

    suma <- 0

    Para i <- 1 Hasta 10 Con Paso 1 Hacer
        Escribir "Temperatura ", i, " (°C): "
        Leer temp
        temperaturas[i] <- temp
        suma <- suma + temp
    FinPara

    promedio <- suma / 10

    contSuperan <- 0
    Para i <- 1 Hasta 10 Con Paso 1 Hacer
        Si temperaturas[i] > promedio Entonces
            contSuperan <- contSuperan + 1
        FinSi
    FinPara

    Escribir "Promedio: ", promedio, " °C"
    Escribir "Superan el promedio: ", contSuperan
FinAlgoritmo
```

**C#:**
```csharp
double[] temperaturas = new double[10];
double suma = 0;

for (int i = 0; i < 10; i++)
{
    Console.Write($"Temperatura {i + 1} (°C): ");
    temperaturas[i] = double.Parse(Console.ReadLine());
    suma += temperaturas[i];
}

double promedio = suma / 10;
int contSuperan = 0;

for (int i = 0; i < 10; i++)
{
    if (temperaturas[i] > promedio)
        contSuperan++;
}

Console.WriteLine($"Promedio: {promedio:F1} °C");
Console.WriteLine($"Superan el promedio: {contSuperan}");
```
</details>

**Ejercicio 3C.** Un alumno rinde 5 exámenes con distintos pesos (porcentajes). Leer cada nota y su peso, y calcular la nota final ponderada.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo NotaPonderada
    Definir nota, peso, notaFinal Como Real
    Definir i Como Entero

    notaFinal <- 0

    Para i <- 1 Hasta 5 Con Paso 1 Hacer
        Escribir "Nota examen ", i, ": "
        Leer nota
        Escribir "Peso (%) del examen ", i, ": "
        Leer peso

        notaFinal <- notaFinal + (nota * peso / 100)
    FinPara

    Escribir "Nota final ponderada: ", notaFinal
FinAlgoritmo
```

**C#:**
```csharp
double notaFinal = 0;

for (int i = 1; i <= 5; i++)
{
    Console.Write($"Nota examen {i}: ");
    double nota = double.Parse(Console.ReadLine());
    Console.Write($"Peso (%) del examen {i}: ");
    double peso = double.Parse(Console.ReadLine());

    notaFinal += nota * peso / 100;
}

Console.WriteLine($"Nota final ponderada: {notaFinal:F2}");
```
</details>

**Ejercicio 3D.** Leer números positivos hasta que el usuario ingrese 0. Mostrar la suma total y el promedio de los números ingresados.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo SumaHastaCero
    Definir num, suma, promedio Como Real
    Definir cont Como Entero

    suma <- 0
    cont <- 0

    Repetir
        Escribir "Ingrese un número positivo (0 para terminar): "
        Leer num

        Si num > 0 Entonces
            suma <- suma + num
            cont <- cont + 1
        FinSi
    Hasta Que num == 0

    Si cont > 0 Entonces
        promedio <- suma / cont
        Escribir "Suma total: ", suma
        Escribir "Promedio: ", promedio
    Sino
        Escribir "No se ingresaron números positivos."
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
double suma = 0;
int cont = 0;
double num;

do
{
    Console.Write("Ingrese un número positivo (0 para terminar): ");
    num = double.Parse(Console.ReadLine());

    if (num > 0)
    {
        suma += num;
        cont++;
    }
} while (num != 0);

if (cont > 0)
{
    double promedio = suma / cont;
    Console.WriteLine($"Suma total: {suma}");
    Console.WriteLine($"Promedio: {promedio:F2}");
}
else
{
    Console.WriteLine("No se ingresaron números positivos.");
}
```
</details>

---

## 4. Banderas (Flags) (35 min)

### 4.1. Concepto

Una bandera es una variable lógica (booleana) que recuerda si algo ocurrió o si se cumple una condición.

**PSeInt:**
```
Definir encontrado Como Logico
encontrado <- Falso          // Bandera abajo: aún no encontramos

// Durante el recorrido...
Si condicionDeHallazgo Entonces
    encontrado <- Verdadero   // ¡Izamos la bandera!
FinSi
```

**C#:**
```csharp
bool encontrado = false;        // Bandera: aún no encontramos

// Durante el recorrido...
if (condicionDeHallazgo)
{
    encontrado = true;          // ¡Izamos la bandera!
}
```

### 4.2. Ejemplo 5 — Buscar si existe un número negativo

**PSeInt:**
```
Algoritmo BuscarNegativo
    Definir num Como Entero
    Definir hayNegativo Como Logico
    Definir i Como Entero

    hayNegativo <- Falso

    Para i <- 1 Hasta 10 Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        Si num < 0 Entonces
            hayNegativo <- Verdadero
        FinSi
    FinPara

    Si hayNegativo Entonces
        Escribir "Sí se ingresó al menos un número negativo."
    Sino
        Escribir "Todos los números fueron positivos o cero."
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
bool hayNegativo = false;

for (int i = 1; i <= 10; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    if (num < 0)
    {
        hayNegativo = true;
    }
}

if (hayNegativo)
    Console.WriteLine("Sí se ingresó al menos un número negativo.");
else
    Console.WriteLine("Todos los números fueron positivos o cero.");
```

### 4.3. Ejemplo 6 — Validar si todos aprobaron

**PSeInt:**
```
Algoritmo TodosAprobaron
    Definir nota Como Real
    Definir todosAprobaron Como Logico
    Definir i Como Entero

    todosAprobaron <- Verdadero    // Bandera optimista: suponemos que sí

    Para i <- 1 Hasta 5 Con Paso 1 Hacer
        Escribir "Nota del alumno ", i, ": "
        Leer nota

        Si nota < 6.0 Entonces
            todosAprobaron <- Falso    // Banderazo: alguien reprobó
        FinSi
    FinPara

    Si todosAprobaron Entonces
        Escribir "¡Todos aprobaron!"
    Sino
        Escribir "Al menos uno reprobó."
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
bool todosAprobaron = true;     // Suponemos que sí (bandera optimista)

for (int i = 1; i <= 5; i++)
{
    Console.Write($"Nota del alumno {i}: ");
    double nota = double.Parse(Console.ReadLine());

    if (nota < 6.0)
    {
        todosAprobaron = false; // Banderazo: alguien reprobó
    }
}

Console.WriteLine(todosAprobaron
    ? "¡Todos aprobaron!"
    : "Al menos uno reprobó.");
```

### 4.4. Ejemplo 7 — Primer número divisible por 7

**PSeInt:**
```
Algoritmo PrimerDivisible7
    Definir i Como Entero
    Definir encontrado Como Logico

    encontrado <- Falso
    i <- 1

    Mientras NO encontrado Y i <= 100 Hacer
        Si i MOD 7 == 0 Entonces
            Escribir "El primer divisible por 7 es: ", i
            encontrado <- Verdadero
        FinSi
        i <- i + 1
    FinMientras
FinAlgoritmo
```

**C#:**
```csharp
// Con bandera (mismo enfoque que PSeInt)
bool encontrado = false;
int i = 1;

while (!encontrado && i <= 100)
{
    if (i % 7 == 0)
    {
        Console.WriteLine($"El primer divisible por 7 es: {i}");
        encontrado = true;
    }
    i++;
}

// Alternativa con break (no disponible en PSeInt básico)
for (int j = 1; j <= 100; j++)
{
    if (j % 7 == 0)
    {
        Console.WriteLine($"El primer divisible por 7 es: {j}");
        break;
    }
}
```

### 4.5. Patrones de bandera

| Patrón | Inicialización PSeInt | Inicialización C# | Significado |
|--------|----------------------|-------------------|-------------|
| "¿Existe algo?" | `bandera <- Falso` | `bool bandera = false;` | Se vuelve `Verdadero`/`true` si aparece |
| "¿Todos cumplen?" | `bandera <- Verdadero` | `bool bandera = true;` | Se vuelve `Falso`/`false` si alguno falla |
| "¿Ya terminamos?" | `continuar <- Verdadero` | `bool continuar = true;` | Controla la salida del bucle |

### 4.6. Ejercicios para pizarra — Banderas

**Ejercicio 4A.** Leer 10 números. Determinar si al menos uno es múltiplo de 5. Usar bandera.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo MultiploDe5
    Definir num Como Entero
    Definir hayMultiplo5 Como Logico
    Definir i Como Entero

    hayMultiplo5 <- Falso

    Para i <- 1 Hasta 10 Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        Si num MOD 5 == 0 Entonces
            hayMultiplo5 <- Verdadero
        FinSi
    FinPara

    Si hayMultiplo5 Entonces
        Escribir "Sí hay al menos un múltiplo de 5."
    Sino
        Escribir "No hay ningún múltiplo de 5."
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
bool hayMultiplo5 = false;

for (int i = 1; i <= 10; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    if (num % 5 == 0)
        hayMultiplo5 = true;
}

Console.WriteLine(hayMultiplo5
    ? "Sí hay al menos un múltiplo de 5."
    : "No hay ningún múltiplo de 5.");
```
</details>

**Ejercicio 4B.** Leer N números. Determinar si todos son positivos. Usar bandera.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo TodosPositivos
    Definir n, num Como Entero
    Definir todosPositivos Como Logico
    Definir i Como Entero

    Escribir "¿Cuántos números? "
    Leer n

    todosPositivos <- Verdadero    // Optimista

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        Si num <= 0 Entonces
            todosPositivos <- Falso
        FinSi
    FinPara

    Si todosPositivos Entonces
        Escribir "Todos los números son positivos."
    Sino
        Escribir "Al menos un número NO es positivo."
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("¿Cuántos números? ");
int n = int.Parse(Console.ReadLine());

bool todosPositivos = true;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    if (num <= 0)
        todosPositivos = false;
}

Console.WriteLine(todosPositivos
    ? "Todos los números son positivos."
    : "Al menos un número NO es positivo.");
```
</details>

**Ejercicio 4C.** Buscar la primera vocal en una palabra ingresada por el usuario. Mostrar cuál es y en qué posición aparece.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo PrimeraVocal
    Definir palabra Como Caracter
    Definir letra Como Caracter
    Definir encontrado Como Logico
    Definir pos, long Como Entero

    Escribir "Ingrese una palabra: "
    Leer palabra

    long <- Longitud(palabra)
    encontrado <- Falso
    pos <- 1

    Mientras NO encontrado Y pos <= long Hacer
        letra <- Mayusculas(Subcadena(palabra, pos, pos))

        Si letra == "A" O letra == "E" O letra == "I" O letra == "O" O letra == "U" Entonces
            Escribir "Primera vocal: ", letra, " en posición ", pos
            encontrado <- Verdadero
        FinSi

        pos <- pos + 1
    FinMientras

    Si NO encontrado Entonces
        Escribir "La palabra no contiene vocales."
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("Ingrese una palabra: ");
string palabra = Console.ReadLine();

bool encontrado = false;

for (int pos = 0; pos < palabra.Length; pos++)
{
    char letra = char.ToUpper(palabra[pos]);

    if (letra == 'A' || letra == 'E' || letra == 'I' || letra == 'O' || letra == 'U')
    {
        Console.WriteLine($"Primera vocal: {letra} en posición {pos + 1}");
        encontrado = true;
        break;
    }
}

if (!encontrado)
    Console.WriteLine("La palabra no contiene vocales.");
```
</details>

**Ejercicio 4D.** Leer números hasta que el usuario ingrese uno mayor a 100 o haya ingresado 10 números. Usar bandera para controlar la salida.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo HastaMayor100
    Definir num, cont Como Entero
    Definir salir Como Logico

    salir <- Falso
    cont <- 0

    Mientras NO salir Y cont < 10 Hacer
        Escribir "Ingrese un número: "
        Leer num

        cont <- cont + 1

        Si num > 100 Entonces
            Escribir "¡Se ingresó un número mayor a 100!"
            salir <- Verdadero
        FinSi
    FinMientras

    Escribir "Total de números ingresados: ", cont
FinAlgoritmo
```

**C#:**
```csharp
bool salir = false;
int cont = 0;

while (!salir && cont < 10)
{
    Console.Write("Ingrese un número: ");
    int num = int.Parse(Console.ReadLine());
    cont++;

    if (num > 100)
    {
        Console.WriteLine("¡Se ingresó un número mayor a 100!");
        salir = true;
    }
}

Console.WriteLine($"Total de números ingresados: {cont}");
```
</details>

---

## 5. Combinación de técnicas (30 min)

Los problemas reales suelen mezclar contadores, acumuladores y banderas.

### 5.1. Ejemplo 8 — Análisis completo de un conjunto de números

**Problema:** Leer N números y mostrar:
- Cuántos son pares (contador)
- Suma de los impares (acumulador)
- Si hay algún múltiplo de 10 (bandera)

**PSeInt:**
```
Algoritmo AnalisisNumeros
    Definir n, num, contPares, sumaImpares Como Entero
    Definir hayMultiplo10 Como Logico
    Definir i Como Entero

    Escribir "Cantidad de números: "
    Leer n

    contPares <- 0
    sumaImpares <- 0
    hayMultiplo10 <- Falso

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        // Contador
        Si num MOD 2 == 0 Entonces
            contPares <- contPares + 1
        FinSi

        // Acumulador
        Si num MOD 2 <> 0 Entonces
            sumaImpares <- sumaImpares + num
        FinSi

        // Bandera
        Si num MOD 10 == 0 Entonces
            hayMultiplo10 <- Verdadero
        FinSi
    FinPara

    Escribir ""
    Escribir "--- RESULTADOS ---"
    Escribir "Pares: ", contPares
    Escribir "Suma de impares: ", sumaImpares

    Si hayMultiplo10 Entonces
        Escribir "¿Hay múltiplo de 10?: Sí"
    Sino
        Escribir "¿Hay múltiplo de 10?: No"
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("Cantidad de números: ");
int n = int.Parse(Console.ReadLine());

int contPares = 0;
int sumaImpares = 0;
bool hayMultiplo10 = false;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    // Contador
    if (num % 2 == 0)
        contPares++;

    // Acumulador
    if (num % 2 != 0)
        sumaImpares += num;

    // Bandera
    if (num % 10 == 0)
        hayMultiplo10 = true;
}

Console.WriteLine($"\n--- RESULTADOS ---");
Console.WriteLine($"Pares: {contPares}");
Console.WriteLine($"Suma de impares: {sumaImpares}");
Console.WriteLine($"¿Hay múltiplo de 10?: {(hayMultiplo10 ? "Sí" : "No")}");
```

### 5.2. Ejemplo 9 — Control de stock con mientras + bandera

**PSeInt:**
```
Algoritmo ControlStock
    Definir stock, cantidad, ventas Como Entero
    Definir recaudacion Como Real
    Definir agotado Como Logico

    stock <- 50
    agotado <- Falso
    ventas <- 0
    recaudacion <- 0

    Mientras NO agotado Hacer
        Escribir "Cantidad a comprar (0 para salir): "
        Leer cantidad

        Si cantidad == 0 Entonces
            agotado <- Verdadero      // Salida voluntaria
        Sino
            Si cantidad > stock Entonces
                Escribir "No hay suficiente stock. Quedan ", stock, " unidades."
            Sino
                stock <- stock - cantidad
                ventas <- ventas + 1
                recaudacion <- recaudacion + (cantidad * 25.50)
                Escribir "Venta realizada. Stock restante: ", stock

                Si stock == 0 Entonces
                    Escribir "¡Stock agotado!"
                    agotado <- Verdadero
                FinSi
            FinSi
        FinSi
    FinMientras

    Escribir ""
    Escribir "Resumen: ", ventas, " ventas | Recaudado: $", recaudacion
FinAlgoritmo
```

**C#:**
```csharp
int stock = 50;
bool agotado = false;
int ventas = 0;
double recaudacion = 0;

while (!agotado)
{
    Console.Write("Cantidad a comprar (0 para salir): ");
    int cantidad = int.Parse(Console.ReadLine());

    if (cantidad == 0)
    {
        agotado = true;         // Salida voluntaria
    }
    else if (cantidad > stock)
    {
        Console.WriteLine($"No hay suficiente stock. Quedan {stock} unidades.");
    }
    else
    {
        stock -= cantidad;
        ventas++;
        recaudacion += cantidad * 25.50;
        Console.WriteLine($"Venta realizada. Stock restante: {stock}");

        if (stock == 0)
        {
            Console.WriteLine("¡Stock agotado!");
            agotado = true;
        }
    }
}

Console.WriteLine($"\nResumen: {ventas} ventas | Recaudado: {recaudacion:C}");
```

### 5.3. Ejemplo 10 — Encuesta con centinela

**PSeInt:**
```
Algoritmo Encuesta
    Definir respuesta Como Caracter
    Definir contSi, contNo, total Como Entero
    Definir pctSi, pctNo Como Real
    Definir continuar Como Logico

    contSi <- 0
    contNo <- 0
    total <- 0
    continuar <- Verdadero

    Mientras continuar Hacer
        Escribir "¿Te gusta la programación? (s/n/x para salir): "
        Leer respuesta
        respuesta <- Mayusculas(respuesta)

        Segun respuesta Hacer
            "S":
                contSi <- contSi + 1
                total <- total + 1
            "N":
                contNo <- contNo + 1
                total <- total + 1
            "X":
                continuar <- Falso
            De Otro Modo:
                Escribir "Opción no válida."
        FinSegun
    FinMientras

    Si total > 0 Entonces
        pctSi <- (contSi / total) * 100
        pctNo <- (contNo / total) * 100
        Escribir "Sí: ", pctSi, "% | No: ", pctNo, "%"
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
int contSi = 0, contNo = 0;
int total = 0;
bool continuar = true;

while (continuar)
{
    Console.Write("¿Te gusta la programación? (s/n/x para salir): ");
    char respuesta = char.ToUpper(Console.ReadKey().KeyChar);
    Console.WriteLine();

    switch (respuesta)
    {
        case 'S':
            contSi++;
            total++;
            break;
        case 'N':
            contNo++;
            total++;
            break;
        case 'X':
            continuar = false;
            break;
        default:
            Console.WriteLine("Opción no válida.");
            break;
    }
}

if (total > 0)
{
    double pctSi = (double)contSi / total * 100;
    double pctNo = (double)contNo / total * 100;
    Console.WriteLine($"\nSí: {pctSi:F1}% | No: {pctNo:F1}%");
}
```

### 5.4. Ejercicios combinados para pizarra

**Ejercicio 5A.** Leer N números. Mostrar:
- Cuántos son positivos y cuántos negativos (contadores)
- Suma de positivos y suma de negativos por separado (acumuladores)
- Si todos los positivos son mayores a 10 (bandera)

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo AnalisisCompleto
    Definir n, num Como Entero
    Definir contPos, contNeg Como Entero
    Definir sumaPos, sumaNeg Como Real
    Definir todosPosMayor10 Como Logico
    Definir i Como Entero

    Escribir "Cantidad de números: "
    Leer n

    contPos <- 0
    contNeg <- 0
    sumaPos <- 0
    sumaNeg <- 0
    todosPosMayor10 <- Verdadero    // Optimista

    Para i <- 1 Hasta n Con Paso 1 Hacer
        Escribir "Número ", i, ": "
        Leer num

        Si num > 0 Entonces
            contPos <- contPos + 1
            sumaPos <- sumaPos + num

            Si num <= 10 Entonces
                todosPosMayor10 <- Falso
            FinSi
        Sino
            Si num < 0 Entonces
                contNeg <- contNeg + 1
                sumaNeg <- sumaNeg + num
            FinSi
        FinSi
    FinPara

    Escribir ""
    Escribir "--- RESULTADOS ---"
    Escribir "Positivos: ", contPos, " (suma: ", sumaPos, ")"
    Escribir "Negativos: ", contNeg, " (suma: ", sumaNeg, ")"

    Si todosPosMayor10 Y contPos > 0 Entonces
        Escribir "Todos los positivos son mayores a 10."
    Sino
        Escribir "No todos los positivos son mayores a 10 (o no hay positivos)."
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
Console.Write("Cantidad de números: ");
int n = int.Parse(Console.ReadLine());

int contPos = 0, contNeg = 0;
double sumaPos = 0, sumaNeg = 0;
bool todosPosMayor10 = true;

for (int i = 1; i <= n; i++)
{
    Console.Write($"Número {i}: ");
    int num = int.Parse(Console.ReadLine());

    if (num > 0)
    {
        contPos++;
        sumaPos += num;

        if (num <= 10)
            todosPosMayor10 = false;
    }
    else if (num < 0)
    {
        contNeg++;
        sumaNeg += num;
    }
}

Console.WriteLine($"\n--- RESULTADOS ---");
Console.WriteLine($"Positivos: {contPos} (suma: {sumaPos})");
Console.WriteLine($"Negativos: {contNeg} (suma: {sumaNeg})");
Console.WriteLine(todosPosMayor10 && contPos > 0
    ? "Todos los positivos son mayores a 10."
    : "No todos los positivos son mayores a 10 (o no hay positivos).");
```
</details>

**Ejercicio 5B.** Simular un cajero automático con saldo inicial de $1000. Permitir retiros mientras haya saldo y el usuario no decida salir. Mostrar: cantidad de retiros, total retirado, saldo final. Usar bandera para control de salida.

<details>
<summary>Ver solución (PSeInt + C#)</summary>

**PSeInt:**
```
Algoritmo CajeroAutomatico
    Definir saldo, monto, totalRetirado Como Real
    Definir contRetiros Como Entero
    Definir salir Como Logico

    saldo <- 1000
    totalRetirado <- 0
    contRetiros <- 0
    salir <- Falso

    Mientras NO salir Hacer
        Escribir "Saldo actual: $", saldo
        Escribir "Monto a retirar (0 para salir): "
        Leer monto

        Si monto == 0 Entonces
            salir <- Verdadero
        Sino
            Si monto > saldo Entonces
                Escribir "Fondos insuficientes."
            Sino
                saldo <- saldo - monto
                totalRetirado <- totalRetirado + monto
                contRetiros <- contRetiros + 1
                Escribir "Retiro exitoso."

                Si saldo == 0 Entonces
                    Escribir "Saldo agotado."
                    salir <- Verdadero
                FinSi
            FinSi
        FinSi
    FinMientras

    Escribir ""
    Escribir "--- RESUMEN ---"
    Escribir "Cantidad de retiros: ", contRetiros
    Escribir "Total retirado: $", totalRetirado
    Escribir "Saldo final: $", saldo
FinAlgoritmo
```

**C#:**
```csharp
double saldo = 1000;
double totalRetirado = 0;
int contRetiros = 0;
bool salir = false;

while (!salir)
{
    Console.WriteLine($"Saldo actual: {saldo:C}");
    Console.Write("Monto a retirar (0 para salir): ");
    double monto = double.Parse(Console.ReadLine());

    if (monto == 0)
    {
        salir = true;
    }
    else if (monto > saldo)
    {
        Console.WriteLine("Fondos insuficientes.");
    }
    else
    {
        saldo -= monto;
        totalRetirado += monto;
        contRetiros++;
        Console.WriteLine("Retiro exitoso.");

        if (saldo == 0)
        {
            Console.WriteLine("Saldo agotado.");
            salir = true;
        }
    }
}

Console.WriteLine($"\n--- RESUMEN ---");
Console.WriteLine($"Cantidad de retiros: {contRetiros}");
Console.WriteLine($"Total retirado: {totalRetirado:C}");
Console.WriteLine($"Saldo final: {saldo:C}");
```
</details>

---

## 6. Taller práctico integrador (20 min + tarea)

### Ejercicio Final en el Aula

Resolver en grupos de 2-3 y luego un grupo pasa a la pizarra.

**Sistema de votación escolar:**

Se realiza una votación para elegir al personero estudiantil. Hay 3 candidatos (A, B, C). El programa debe:

1. Leer votos hasta que se ingrese "FIN".
2. Validar que el voto sea A, B o C.
3. Contar los votos de cada candidato (contadores).
4. Calcular el porcentaje de cada uno (acumulador de total + cálculo).
5. Determinar si hay un ganador con mayoría absoluta (>50%) (bandera).
6. Si nadie tiene mayoría, indicar que hay segunda vuelta entre los dos más votados.
7. Mostrar un resumen completo al final.

**PSeInt:**
```
Algoritmo VotacionEscolar
    Definir voto Como Caracter
    Definir votosA, votosB, votosC, votosNulos, total Como Entero
    Definir pctA, pctB, pctC Como Real
    Definir hayGanador Como Logico
    Definir ganador Como Caracter

    votosA <- 0
    votosB <- 0
    votosC <- 0
    votosNulos <- 0
    total <- 0
    hayGanador <- Falso
    ganador <- ""

    Escribir "=== VOTACIÓN PERSONERO ==="
    Escribir "Candidatos: A - B - C"
    Escribir "Ingrese FIN para terminar."
    Escribir ""

    Repetir
        Escribir "Su voto: "
        Leer voto
        voto <- Mayusculas(voto)

        Si voto <> "FIN" Entonces
            Segun voto Hacer
                "A":
                    votosA <- votosA + 1
                    total <- total + 1
                "B":
                    votosB <- votosB + 1
                    total <- total + 1
                "C":
                    votosC <- votosC + 1
                    total <- total + 1
                De Otro Modo:
                    Escribir "Voto inválido. Use A, B o C."
                    votosNulos <- votosNulos + 1
                    total <- total + 1
            FinSegun
        FinSi
    Hasta Que voto == "FIN"

    Si total == 0 Entonces
        Escribir "No se registraron votos."
    Sino
        pctA <- (votosA / total) * 100
        pctB <- (votosB / total) * 100
        pctC <- (votosC / total) * 100

        Escribir ""
        Escribir "========== RESULTADOS =========="
        Escribir "Total de votos: ", total
        Escribir "Votos nulos: ", votosNulos
        Escribir "Candidato A: ", votosA, " votos (", pctA, "%)"
        Escribir "Candidato B: ", votosB, " votos (", pctB, "%)"
        Escribir "Candidato C: ", votosC, " votos (", pctC, "%)"

        // Mayoría absoluta (>50%)
        Si pctA > 50 Entonces
            hayGanador <- Verdadero
            ganador <- "A"
        Sino
            Si pctB > 50 Entonces
                hayGanador <- Verdadero
                ganador <- "B"
            Sino
                Si pctC > 50 Entonces
                    hayGanador <- Verdadero
                    ganador <- "C"
                FinSi
            FinSi
        FinSi

        Si hayGanador Entonces
            Escribir ""
            Escribir "¡GANADOR CON MAYORÍA ABSOLUTA: Candidato ", ganador, "!"
        Sino
            Escribir ""
            Escribir "Nadie obtuvo mayoría absoluta. Se va a segunda vuelta."

            // Determinar los dos más votados (simplificado)
            Si votosA >= votosB Y votosA >= votosC Entonces
                Escribir "Pasan: Candidato A"
                Si votosB >= votosC Entonces
                    Escribir " y Candidato B"
                Sino
                    Escribir " y Candidato C"
                FinSi
            Sino
                Si votosB >= votosA Y votosB >= votosC Entonces
                    Escribir "Pasan: Candidato B"
                    Si votosA >= votosC Entonces
                        Escribir " y Candidato A"
                    Sino
                        Escribir " y Candidato C"
                    FinSi
                Sino
                    Escribir "Pasan: Candidato C"
                    Si votosA >= votosB Entonces
                        Escribir " y Candidato A"
                    Sino
                        Escribir " y Candidato B"
                    FinSi
                FinSi
            FinSi
        FinSi
    FinSi
FinAlgoritmo
```

**C#:**
```csharp
int votosA = 0, votosB = 0, votosC = 0, votosNulos = 0;
int totalVotos = 0;
bool hayGanador = false;
string ganador = "";

Console.WriteLine("=== VOTACIÓN PERSONERO ===");
Console.WriteLine("Candidatos: A - B - C");
Console.WriteLine("Ingrese FIN para terminar.\n");

while (true)
{
    Console.Write("Su voto: ");
    string voto = Console.ReadLine().Trim().ToUpper();

    if (voto == "FIN")
        break;

    switch (voto)
    {
        case "A": votosA++; totalVotos++; break;
        case "B": votosB++; totalVotos++; break;
        case "C": votosC++; totalVotos++; break;
        default:
            Console.WriteLine("Voto inválido. Use A, B o C.");
            votosNulos++;
            totalVotos++;
            break;
    }
}

if (totalVotos == 0)
{
    Console.WriteLine("No se registraron votos.");
    return;
}

Console.WriteLine($"\n========== RESULTADOS ==========");
Console.WriteLine($"Total de votos: {totalVotos}");
Console.WriteLine($"Votos nulos: {votosNulos}");
Console.WriteLine($"Candidato A: {votosA} votos ({(double)votosA / totalVotos * 100:F1}%)");
Console.WriteLine($"Candidato B: {votosB} votos ({(double)votosB / totalVotos * 100:F1}%)");
Console.WriteLine($"Candidato C: {votosC} votos ({(double)votosC / totalVotos * 100:F1}%)");

// Determinar ganador con mayoría absoluta
if ((double)votosA / totalVotos > 0.5)
{
    hayGanador = true;
    ganador = "A";
}
else if ((double)votosB / totalVotos > 0.5)
{
    hayGanador = true;
    ganador = "B";
}
else if ((double)votosC / totalVotos > 0.5)
{
    hayGanador = true;
    ganador = "C";
}

if (hayGanador)
{
    Console.WriteLine($"\n¡GANADOR CON MAYORÍA ABSOLUTA: Candidato {ganador}!");
}
else
{
    Console.WriteLine("\nNadie obtuvo mayoría absoluta. Se va a segunda vuelta.");

    if (votosA >= votosB && votosA >= votosC)
    {
        Console.Write("Pasan: Candidato A");
        if (votosB >= votosC)
            Console.WriteLine(" y Candidato B");
        else
            Console.WriteLine(" y Candidato C");
    }
    else if (votosB >= votosA && votosB >= votosC)
    {
        Console.Write("Pasan: Candidato B");
        if (votosA >= votosC)
            Console.WriteLine(" y Candidato A");
        else
            Console.WriteLine(" y Candidato C");
    }
    else
    {
        Console.Write("Pasan: Candidato C");
        if (votosA >= votosB)
            Console.WriteLine(" y Candidato A");
        else
            Console.WriteLine(" y Candidato B");
    }
}
```

---

## Banco de ejercicios adicionales (para práctica en casa)

Cada ejercicio debe resolverse **primero en PSeInt y luego en C#**.

### Nivel 1 — Básico (solo un concepto)

**E1.** Leer 10 números y contar cuántos son mayores a 100.

**E2.** Leer N números y mostrar la suma de los que son múltiplos de 3.

**E3.** Leer una frase carácter por carácter e indicar si contiene la letra 'z'. Usar `Para` con `Longitud` en PSeInt y `foreach` en C#.

**E4.** Leer 5 números y mostrar el mayor de todos (usar acumulador lógico: variable `mayor` que se actualiza).

**E5.** Leer N palabras ingresadas por el usuario y contar cuántas tienen más de 5 letras.

### Nivel 2 — Intermedio (dos conceptos)

**E6.** Leer números hasta que se ingrese -1. Contar cuántos son primos y mostrar la suma de los no primos.

**E7.** Leer 15 temperaturas. Calcular el promedio y contar cuántas temperaturas están por encima del promedio. (Requiere arreglo o dos recorridos.)

**E8.** Leer N nombres. Indicar si hay algún nombre que empiece con vocal. Contar cuántos empiezan con consonante.

**E9.** Leer montos de ventas de 10 vendedores. Si algún vendedor supera $5000, izar bandera y mostrar "Hay vendedor estrella". Calcular el total vendido.

**E10.** Leer números hasta que se ingresen 3 números pares consecutivos. Mostrar cuántos números se ingresaron en total.

### Nivel 3 — Avanzado (tres conceptos combinados)

**E11.** Juego: adivinar un número secreto (entre 1 y 100). El usuario ingresa intentos. El programa dice "mayor" o "menor". Contar intentos, acumular la diferencia entre el intento y el número real, y usar bandera cuando acierte. Al final mostrar intentos y promedio de cercanía.

**E12.** Cajero automático completo:
- Saldo inicial $5000
- Opciones: 1=Depositar, 2=Retirar, 3=Ver saldo, 4=Salir
- No permitir retiros mayores al saldo (bandera de saldo insuficiente)
- Contar cantidad de depósitos y retiros
- Acumular total depositado y total retirado
- Al salir, mostrar resumen completo

**E13.** Torneo de 3 equipos (todos contra todos, 3 partidos). Por cada partido ingresar goles del equipo local y visitante. Determinar:
- Puntos de cada equipo (3 por ganar, 1 empate, 0 perder)
- Diferencia de gol de cada equipo (goles a favor - goles en contra)
- Si hay un campeón invicto (bandera)
- El equipo con más goles a favor

**E14.** Validación de contraseña con 3 intentos:
- La contraseña correcta es "Csharp2024"
- Usar bandera `accesoConcedido` (en PSeInt: `acceso <- Falso`)
- Contar intentos fallidos
- Si en 3 intentos no acierta, bloquear (bandera `bloqueado`)
- Mostrar mensaje adecuado al final

**E15.** Calculadora de notas de un curso:
- Se ingresan 4 notas por estudiante (cada una de 1.0 a 7.0)
- El curso tiene N estudiantes
- Calcular nota final de cada uno (promedio simple)
- Contar aprobados y reprobados
- Promedio general del curso (acumulador)
- Bandera si todos los estudiantes aprobaron
- Bandera si algún estudiante tuvo nota perfecta (7.0 en todas las notas)
- Mostrar nota más alta y más baja del curso

---

## Resumen visual para la pizarra (cierre de clase)

```
┌────────────────────────────────────────────────────────────────────┐
│  CONTADOR             ACUMULADOR              BANDERA              │
│                                                                    │
│  PSeInt:              PSeInt:                PSeInt:              │
│  Definir c Entero     Definir s Real         Definir b Logico     │
│  c <- 0               s <- 0                 b <- Falso           │
│  c <- c + 1           s <- s + valor         Si cond Entonces     │
│                                                  b <- Verdadero   │
│  C#:                  C#:                    C#:                  │
│  int c = 0;           double s = 0;          bool b = false;      │
│  c++;                 s += valor;            if(cond)             │
│                                                b = true;          │
│                                                                    │
│  ¿Cuántos?            ¿Cuánto?               ¿Ocurrió?            │
│  Cantidad             Total                  Estado               │
├────────────────────────────────────────────────────────────────────┤
│  Las tres trabajan DENTRO de estructuras repetitivas               │
│  (Para/Mientras/Repetir en PSeInt, for/while/do-while en C#).     │
│                                                                    │
│  Regla de oro: Siempre inicializar antes del bucle.               │
└────────────────────────────────────────────────────────────────────┘
```

### Preguntas de cierre (5 min)

1. ¿Qué tipo de variable usarías para saber cuántos estudiantes miden más de 1.70 m?
2. ¿Qué tipo de variable usarías para saber el peso total de un grupo?
3. ¿Qué tipo de variable usarías para saber si alguien sacó nota máxima?
4. ¿Puede un mismo problema usar los tres conceptos? Da un ejemplo.

---

## Notas para el docente

- **Sección 1:** Usar la pizarra para las definiciones. Hacer que los estudiantes den ejemplos cotidianos.
- **Sección 2-4:** Escribir primero el algoritmo en PSeInt en la pizarra (es más cercano al español). Luego traducirlo a C#. Los estudiantes deben ver la correspondencia entre ambos lenguajes.
- **Flujo recomendado por cada ejemplo:**
  1. Plantear el problema en voz alta.
  2. Escribir el PSeInt completo en la pizarra.
  3. Preguntar: "¿Cómo se traduce esta línea a C#?"
  4. Escribir el C# al lado, línea por línea.
  5. Ejecutar mentalmente con datos de prueba.
- **Ejercicios de pizarra:** Las soluciones están en `<details>` para referencia del docente. Llamar a distintos estudiantes a resolver cada ejercicio. Que primero escriban en PSeInt y luego lo pasen a C#.
- **Sección 5:** El ejemplo del cajero y la votación suelen ser los que más enganchan. Dedicarles tiempo suficiente.
- **Taller final:** Formar grupos de 2-3. El primer grupo que termine (y funcione) pasa a explicar en pizarra ambas versiones.
- **Tarea:** Asignar 3 ejercicios del banco (uno de cada nivel) según el desempeño observado. Deben entregar ambos: PSeInt y C#.
- **Para los ejercicios del banco sin solución en este documento:** Se sugiere resolver al menos E1, E6 y E12 en clase si hay tiempo extra, o usarlos como ejemplos adicionales. Los estudiantes deben practicar la traducción PSeInt → C# de forma autónoma.
