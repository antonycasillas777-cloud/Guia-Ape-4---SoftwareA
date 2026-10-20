# 💻 Guía APE · Programación Orientada a Objetos

Cinco ejercicios de **Programación Orientada a Objetos (POO)** desarrollados en **Java y C++**, para practicar clases, objetos, atributos, constructores y referencias.

Cada documento incluye:

- 📌 Enunciado del ejercicio.
- 💡 Explicación de la solución.
- ☕ Código completo en Java.
- ⚙️ Código completo en C++.
- 🖥️ Salidas de ejecución.

## 📚 Documentación

📘 **[PDF general con todos los ejercicios](Guia_APE_Java_y_CPP_Explicada.pdf)**

| N.º | Ejercicio | Clases | Documento |
|:---:|---|---|:---:|
| 01 | Notas del curso | `Estudiante` | [📄 PDF](01_Notas_del_curso.pdf) |
| 02 | Inventario de una tienda | `Producto` | [📄 PDF](02_Inventario_de_una_tienda.pdf) |
| 03 | Veterinaria | `Mascota` | [📄 PDF](03_Veterinaria.pdf) |
| 04 | Cuenta de ahorro | `Cuenta` | [📄 PDF](04_Cuenta_de_ahorro.pdf) |
| 05 | Biblioteca | `Libro` y `Socio` | [📄 PDF](05_Biblioteca.pdf) |

## 🧩 Ejercicios

### 🎓 01. Notas del curso

Crea cinco estudiantes, calcula el promedio de sus tres notas y muestra su estado académico:

- **Aprobado:** promedio mayor o igual que 7.
- **Supletorio:** promedio mayor o igual que 5 y menor que 7.
- **Reprobado:** promedio menor que 5.

Al finalizar, muestra la cantidad de estudiantes aprobados.

### 🛒 02. Inventario de una tienda

Crea cuatro productos con nombre, precio y stock.

Simula la venta de tres unidades de dos productos, muestra **“Reponer”** cuando quedan menos de cinco unidades y calcula el valor total del inventario restante.

### 🐾 03. Veterinaria

Crea tres mascotas con nombre, especie, edad y peso. Muestra **“Revisar peso”** cuando una mascota supera los 20 kg.

También demuestra cómo dos variables pueden acceder al mismo objeto.

**En Java:**

```java
Mascota m4 = m1;
```

**En C++:**

```cpp
Mascota& m4 = m1;
```

Al modificar la edad mediante `m4`, el cambio también se observa en `m1`. En C++, escribir esa declaración sin `&` crearía una copia.

### 💰 04. Cuenta de ahorro

Crea dos cuentas con saldos iniciales de **$200** y **$350**.

Mediante un ciclo `while`, deposita **$50 por mes** en cada cuenta hasta alcanzar **$500**. Muestra los saldos después de cada depósito y los meses necesarios para llegar a la meta.

### 📖 05. Biblioteca

Crea cuatro libros y dos socios.

Registra dos préstamos para el primer socio y uno para el segundo. Actualiza la disponibilidad de los libros, muestra los préstamos de cada socio y cuenta cuántos libros siguen disponibles.

## 🛠️ Conceptos practicados

- Clases, atributos y objetos.
- Constructores e inicialización de datos.
- Arreglos de objetos.
- Condicionales `if` y `else`.
- Ciclos `for` y `while`.
- Contadores y acumuladores.
- Referencias compartidas en Java.
- Referencias en C++.
- Métodos para mostrar información.

## ▶️ Cómo ejecutar los programas

Los códigos completos están dentro de los PDFs. Cada ejercicio se ejecuta por separado y utiliza datos definidos en el código.

### ☕ Java

Necesitas tener instalado un **JDK**.

Guarda el código del primer ejercicio como `Ejercicio1.java` y ejecuta desde esa carpeta:

```bash
javac Ejercicio1.java
java Ejercicio1
```

### ⚙️ C++

Necesitas un compilador compatible con **C++11 o posterior**.

Guarda el código del primer ejercicio como `Ejercicio1.cpp` y compílalo:

```bash
g++ -std=c++11 Ejercicio1.cpp -o Ejercicio1
```

**En Windows con PowerShell:**

```powershell
.\Ejercicio1.exe
```

**En Linux o macOS:**

```bash
./Ejercicio1
```

Para ejecutar los demás, cambia el número del archivo y del programa: `Ejercicio2`, `Ejercicio3`, `Ejercicio4` o `Ejercicio5`.

## ✅ Resultados obtenidos

Los cinco ejercicios se compilaron y ejecutaron en ambos lenguajes.

| Ejercicio | Resultado con los datos del ejemplo |
|---|---|
| 🎓 Notas del curso | 3 estudiantes aprobados. |
| 🛒 Inventario | Valor restante de $104; Lapiz y Mochila requieren reposición. |
| 🐾 Veterinaria | La edad de `m1` cambia de 4 a 5 al modificarla mediante `m4`. |
| 💰 Cuenta de ahorro | La primera cuenta necesita 6 meses y la segunda, 3. |
| 📖 Biblioteca | Los socios tienen 2 y 1 préstamos; queda 1 libro disponible. |

> Java puede mostrar `9.0` donde C++ muestra `9`. Esa diferencia de presentación no cambia el resultado.
