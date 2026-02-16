# Estructura del Curso py131: Estructuras de Datos y Algoritmia Pythonica

## Enfoque
**100% Práctico y "Hands-on"**. Menos teoría académica, más resolución de problemas reales (Katas) aprovechando la biblioteca estándar de Python. Objetivo: Pensamiento algorítmico eficiente.

## Temario (12 Talleres)

### Módulo 1: La Realidad del Rendimiento
*Midiendo y optimizando antes de programar.*

1.  **01_taller_big_o.ipynb**
    *   *Experimento:* Medir tiempos de ejecución reales (list vs set lookup).
    *   *Reto:* Identificar cuellos de botella en funciones dadas. Gráficas de rendimiento.
2.  **02_optimizando_listas.ipynb**
    *   *Concepto:* Arrays dinámicos y búsqueda binaria.
    *   *Reto:* Sistema de "High Scores" en tiempo real usando `bisect` vs `.sort()`.

### Módulo 2: Estructuras Lineales de Batalla
*Herramientas para manipulación de datos.*

3.  **03_hackeando_diccionarios.ipynb**
    *   *Concepto:* Hash Maps y Tablas de frecuencia.
    *   *Reto:* Detección de anagramas y "Primer caracter único" en textos masivos.
4.  **04_pilas_colas_practico.ipynb**
    *   *Reto Pila:* Validador de sintaxis de código (balanceo de paréntesis).
    *   *Reto Cola:* Simulador de sistema de impresión (Round Robin) con `deque`.
5.  **05_domando_el_heap.ipynb**
    *   *Concepto:* Colas de prioridad.
    *   *Reto:* "Top K Elements" en streaming (logs de servidor) y fusión de listas ordenadas.

### Módulo 3: Grafos (El core de redes y dependencias)
*Fundamentos para entender Airflow y Orquestadores.*

6.  **06_modelando_grafos.ipynb**
    *   *Ejercicio:* Modelar una red de vuelos/rutas usando diccionarios de adyacencia.
    *   *Reto:* Consultas de conectividad ("¿Puedo llegar de A a B?").
7.  **07_bfs_dfs_rescatista.ipynb**
    *   *Proyecto:* "Laberinto Bot". Implementar BFS para ruta más corta y DFS para exploración completa.
8.  **08_orden_topologico_dependencias.ipynb** (★ Vital para CI/CD y Airflow)
    *   *Reto:* "El Build System". Resolver orden de ejecución de tareas con dependencias. Detectar ciclos circulares.

### Módulo 4: Patrones de Resolución
*Técnicas para resolver lo complejo.*

9.  **09_recursion_kata.ipynb**
    *   *Reto:* Aplanador de estructuras JSON profundamente anidadas. Explorador de carpetas recursivo.
10. **10_programacion_dinamica_memoization.ipynb**
    *   *Experimento:* Fibonacci recursivo (lento) vs `@cache` (instantáneo).
    *   *Reto:* Problema de la escalera (formas de subir) o "Coin Change" básico.
11. **11_backtracking_sudoku.ipynb**
    *   *Reto Visual:* Solver de Sudoku o N-Reinas. Visualizar cómo el algoritmo "se arrepiente" y retrocede.

### Módulo 5: Proyecto Integrador

12. **12_el_optimizador_logistico.ipynb**
    *   *Capstone:* Sistema de despacho.
    *   *Inputs:* Mapa (Grafo ponderado), Pedidos (Cola Prioridad), Flota.
    *   *Objetivo:* Asignar y rutear eficientemente usando Dijkstra + Heaps.
