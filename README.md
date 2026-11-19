# Ordenacion-Listas
# UD01 – Implementación de algoritmos de ordenación en Kotlin

Actividad de la unidad UD01 del módulo **PMDM 2026/27** (iLERNA).

**Autor/a:** NOMBRE APELLIDO
**Curso:** PMDM 2026/27

## Descripción del proyecto

El objetivo es investigar, implementar y comparar **cinco algoritmos de ordenación** en Kotlin, sin utilizar `sort()`, `sorted()`, `sortBy()` ni funciones equivalentes de la librería estándar.

Todos los algoritmos trabajan con **los mismos datos**, generados en `GenerarDatos.kt`:

| Lista | Tipo | Contenido |
|-------|------|-----------|
| Vehículos | `MutableList<String>` | Al menos 40 nombres de vehículos distintos, desordenados. Se ordenan alfabéticamente (A-Z). |
| Números | `MutableList<Int>` | 100 enteros aleatorios entre 1 y 10000, sin repetir. Se ordenan de menor a mayor. |

Cada programa:

1. Obtiene las listas generadas en `GenerarDatos.kt`.
2. Trabaja sobre una **copia** de cada lista, para no alterar los datos originales.
3. Muestra la lista original.
4. La ordena con su algoritmo.
5. Muestra la lista ordenada.
6. Mide el tiempo de ejecución con `System.nanoTime()`.

## Algoritmos implementados

| Fichero | Algoritmo | Complejidad media | Complejidad en el peor caso |
|---------|-----------|-------------------|-----------------------------|
| `01_QuickSort.kt` | QuickSort | O(n log n) | O(n²) |
| `02_PancakeSort.kt` | Pancake Sort | O(n²) | O(n²) |
| `03_MergeSort.kt` | MergeSort | O(n log n) | O(n log n) |
| `04_HeapSort.kt` | Heap Sort | O(n log n) | O(n log n) |
| `05_InsertionSort.kt` | Insertion Sort | O(n²) | O(n²) |

## Estructura del repositorio

```
.
├── GenerarDatos.kt
├── 01_QuickSort.kt
├── 02_PancakeSort.kt
├── 03_MergeSort.kt
├── 04_HeapSort.kt
├── 05_InsertionSort.kt
├── UD01_OrdenacionListas_NombreApellido.pdf
└── README.md
```

## Requisitos

- JDK 17 o superior.
- Kotlin 1.9 o superior.
- IntelliJ IDEA (recomendado) o el compilador `kotlinc` desde terminal.

## Instrucciones de ejecución

### Opción 1: IntelliJ IDEA (recomendada)

1. Clona el repositorio:
   ```bash
   git clone https://github.com/USUARIO/NOMBRE-REPOSITORIO.git
   ```
2. Abre la carpeta como proyecto en IntelliJ IDEA.
3. Abre el fichero del algoritmo que quieras probar (por ejemplo, `01_QuickSort.kt`).
4. Pulsa el icono verde ▶ junto a la función `main` y elige **Run**.

### Opción 2: Línea de comandos

Compila el fichero del algoritmo junto con `GenerarDatos.kt` y ejecútalo. Ejemplo con QuickSort:

```bash
kotlinc GenerarDatos.kt 01_QuickSort.kt -include-runtime -d quicksort.jar
java -cp quicksort.jar _01_QuickSortKt
```

> El nombre de la clase generada depende del nombre del fichero (los que empiezan por un número llevan un `_` delante). Si hay dudas, se puede consultar con `unzip -l quicksort.jar`.

Repite el proceso cambiando el fichero para el resto de algoritmos.

## Resultados

Los tiempos medidos, las capturas de ejecución y el análisis comparativo se encuentran en el informe PDF incluido en este repositorio:
`UD01_OrdenacionListas_NombreApellido.pdf`.

| Algoritmo | Tiempo lista de números (ns) | Tiempo lista de vehículos (ns) |
|-----------|------------------------------|--------------------------------|
| QuickSort | *(completar)* | *(completar)* |
| Pancake Sort | *(completar)* | *(completar)* |
| MergeSort | *(completar)* | *(completar)* |
| Heap Sort | *(completar)* | *(completar)* |
| Insertion Sort | *(completar)* | *(completar)* |

## Bibliografía

- *(añadir las fuentes consultadas, las mismas que aparecen en el informe)*

---

Actividad realizada con fines educativos para el módulo PMDM, curso 2026/27.
