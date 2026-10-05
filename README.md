# GUÍA DE PRÁCTICAS #04

## Implementación y representación de árboles y grafos

### 📚 Asignatura

**Estructura de Datos**

### 🎓 Carrera

**Tecnologías de la Información**

### 🏫 Universidad

**Universidad Estatal Amazónica (UEA)**

---

## 👨‍💻 Descripción del proyecto

El presente proyecto corresponde a la Guía de Prácticas #04 de la asignatura Estructura de Datos y tiene como finalidad aplicar los conocimientos adquiridos sobre árboles y grafos mediante la implementación de un problema práctico utilizando un lenguaje de programación.

Para el desarrollo de la práctica se seleccionó el problema de **encuentro de vuelos baratos a partir de una base de datos ficticia**.

El sistema utiliza un **grafo ponderado**, donde las ciudades representan los vértices y los vuelos representan las aristas. El precio de cada vuelo se utiliza como peso de la arista.

El programa permite consultar las ciudades disponibles, visualizar los vuelos registrados y encontrar una ruta de menor costo entre una ciudad de origen y una ciudad de destino.

---

## 🎯 Objetivo general

Implementar un grafo ponderado mediante un lenguaje de programación para encontrar rutas de vuelos de menor costo entre diferentes ciudades, aplicando estructuras de datos y algoritmos de búsqueda eficientes.

---

## 🎯 Objetivos específicos

* Representar las ciudades mediante vértices de un grafo.
* Representar los vuelos mediante aristas ponderadas.
* Crear una base de datos ficticia de vuelos.
* Implementar un algoritmo para encontrar rutas de menor costo.
* Permitir al usuario consultar los elementos del grafo.
* Generar reportes con los resultados obtenidos.
* Medir el tiempo de ejecución del algoritmo.
* Analizar las ventajas y desventajas de la estructura utilizada.

---

## 🧩 Estructura de datos utilizada

La estructura de datos principal utilizada en este proyecto es un **grafo ponderado** implementado mediante una **lista de adyacencia**.

### Representación

* **Vértices:** ciudades.
* **Aristas:** vuelos.
* **Peso:** precio del vuelo.
* **Origen:** ciudad inicial.
* **Destino:** ciudad final.

Ejemplo:

```text
Quito ---- $40 ---- Cuenca
  |                   |
 $35                 $45
  |                   |
 Loja              Manta
  |
 $50
  |
Guayaquil
```

---

## 🧮 Algoritmo utilizado

Para determinar la ruta de menor costo se utiliza el **algoritmo de Dijkstra**, debido a que permite encontrar caminos de costo mínimo en grafos cuyos pesos son no negativos.

El algoritmo analiza las diferentes conexiones disponibles y determina la ruta cuyo costo total sea menor entre el origen y el destino seleccionado.

---

## 🗂️ Base de datos

La información utilizada corresponde a una base de datos ficticia de vuelos.

Ejemplo:

| Origen    | Destino   | Precio |
| --------- | --------- | -----: |
| Quito     | Guayaquil |    $45 |
| Quito     | Loja      |    $35 |
| Quito     | Cuenca    |    $40 |
| Loja      | Cuenca    |    $25 |
| Loja      | Guayaquil |    $50 |
| Cuenca    | Guayaquil |    $30 |
| Guayaquil | Manta     |    $35 |
| Cuenca    | Manta     |    $45 |

---

## 📊 Reportería

El programa permite:

1. Visualizar las ciudades disponibles.
2. Visualizar los vuelos registrados.
3. Consultar las conexiones entre ciudades.
4. Seleccionar una ciudad de origen.
5. Seleccionar una ciudad de destino.
6. Obtener la ruta de menor costo.
7. Mostrar el costo total de la ruta.
8. Mostrar el tiempo de ejecución del algoritmo.

Ejemplo de resultado:

```text
========== RESULTADO ==========

Origen: Quito
Destino: Manta

Ruta encontrada:
Quito -> Cuenca -> Manta

Costo total: $85

Tiempo de ejecución:
0.000012 segundos
```

---

## ⏱️ Análisis del tiempo de ejecución

Para medir el tiempo de ejecución del algoritmo se utiliza la función `perf_counter()` de Python.

El tiempo de ejecución permite analizar el rendimiento del programa durante la búsqueda de la ruta de menor costo.

Los resultados pueden variar dependiendo de:

* Cantidad de ciudades.
* Cantidad de vuelos.
* Número de conexiones.
* Capacidad del computador.
* Tamaño de la información procesada.

---

## 🤖 Agente de inteligencia artificial utilizado

Durante el desarrollo del proyecto se utilizó **ChatGPT** como herramienta de apoyo para:

* Comprender el funcionamiento de los grafos.
* Analizar el algoritmo de Dijkstra.
* Orientar la estructura del código.
* Detectar y corregir errores.
* Mejorar la documentación del proyecto.

**Porcentaje estimado de código desarrollado con apoyo de IA: 60 %.**

El código fue revisado, adaptado y probado por el estudiante con el propósito de comprender su funcionamiento.

> El porcentaje debe ser modificado de acuerdo con el porcentaje real de código desarrollado con ayuda de inteligencia artificial.

---

## ✅ Ventajas de la estructura utilizada

* Permite representar fácilmente las conexiones entre ciudades.
* Permite asociar un costo a cada vuelo.
* Es adecuada para representar redes y rutas.
* Permite aplicar algoritmos de búsqueda de caminos.
* La lista de adyacencia permite almacenar eficientemente grafos con pocas conexiones.
* Facilita la incorporación de nuevas ciudades y vuelos.

---

## ❌ Desventajas de la estructura utilizada

* Su implementación es más compleja que una estructura lineal.
* Los algoritmos de búsqueda requieren mayor conocimiento.
* Los grafos grandes pueden requerir mayor cantidad de recursos.
* Una mala organización de los datos puede producir resultados incorrectos.
* Dijkstra no está diseñado para trabajar con pesos negativos.

---

## 📁 Organización del proyecto

```text
guia-practica-04-arboles-grafos/
│
├── README.md
├── src/
│   └── vuelos.py
├── datos/
│   └── vuelos.txt
├── evidencias/
│   ├── captura_01_repositorio.png
│   ├── captura_02_codigo.png
│   ├── captura_03_ejecucion.png
│   └── captura_04_resultados.png
├── documentos/
│   └── informe-guia-practica-04.pdf
└── resultados/
    └── reporte.txt
```

---

## ▶️ Ejecución del proyecto

Para ejecutar el programa es necesario tener instalado **Python 3**.

Desde la terminal se debe ingresar a la carpeta del proyecto y ejecutar:

```bash
python src/vuelos.py
```

---

## 📌 Conclusión

La implementación del sistema de búsqueda de vuelos baratos permitió aplicar los conocimientos relacionados con grafos, listas de adyacencia y algoritmos de búsqueda. La utilización de un grafo ponderado permitió representar las ciudades y sus conexiones, mientras que el algoritmo de Dijkstra permitió determinar rutas de menor costo.

El proyecto permitió relacionar los conocimientos teóricos de la asignatura Estructura de Datos con una aplicación práctica orientada a la resolución de problemas de rutas y optimización.

---

## 👨‍🎓 Autor

**Estudiante:** Maria Jose Torres JUngal

**Carrera:** Tecnologías de la Información

**Asignatura:** Estructura de Datos

**Docente:** Delfín Bernabé Ortega Tenezaca

**Guía:** Práctica #04

**Año:** 2026
