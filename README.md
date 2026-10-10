# Algoritmos from Scratch

Notebooks de Jupyter para estudiar algoritmos desde cero: fundamentos de ciencias de la computación, análisis de complejidad, algoritmos clásicos, optimización, modelos generativos y computación cuántica.

## Enfoque

Cada notebook combina teoría (definiciones, notación matemática y análisis de complejidad), implementaciones en Python paso a paso y visualizaciones.

Las notebooks se guardan con sus resultados ejecutados, así que se pueden leer directamente en GitHub.

## Notebooks

Las carpetas y las notebooks están numeradas en el orden sugerido de estudio.

### 01 · Fundamentos

| # | Notebook | Contenido |
|---|----------|-----------|
| 01 | [Fundamentos de Ciencias de la Computación](notebooks/01-fundamentos/01-fundamentos-ciencia-computacion.ipynb) | Teoría de la computación, arquitectura de computadores, lenguajes y paradigmas de programación, estructuras de datos y compiladores |
| 02 | [Complejidad Algorítmica](notebooks/01-fundamentos/02-complejidad-algoritmica.ipynb) | Notación asintótica, reglas de cálculo, conteo de operaciones, resolución de recurrencias, análisis empírico y complejidad espacial |
| 03 | [Big O: análisis empírico](notebooks/01-fundamentos/03-big-o-analisis-empirico.ipynb) | Experimento que compara cuatro formas de sumar la diagonal de una matriz (bucles anidados, un bucle, comprensión de listas y NumPy) y ajusta curvas de complejidad a los tiempos medidos |

### 02 · Algoritmos clásicos

| # | Notebook | Contenido |
|---|----------|-----------|
| 04 | [Algoritmos de Búsqueda](notebooks/02-algoritmos-clasicos/04-algoritmos-busqueda.ipynb) | Lineal, binaria, por saltos, exponencial, por interpolación y ternaria |
| 05 | [Algoritmos de Ordenamiento](notebooks/02-algoritmos-clasicos/05-algoritmos-ordenamiento.ipynb) | Bubble, Selection, Insertion, Merge y Quick Sort |
| 06 | [Algoritmos de Grafos](notebooks/02-algoritmos-clasicos/06-algoritmos-grafos.ipynb) | Representaciones, BFS, DFS, Dijkstra, Bellman-Ford, Floyd-Warshall, Kruskal, Prim, orden topológico, ciclos, componentes conexas y grafos bipartitos |
| 07 | [Algoritmos de Compresión](notebooks/02-algoritmos-clasicos/07-algoritmos-compresion.ipynb) | RLE, Huffman, LZW, Shannon-Fano, LZ77, codificación aritmética, entropía y límites teóricos |

### 03 · Optimización y modelos generativos

| # | Notebook | Contenido |
|---|----------|-----------|
| 08 | [Algoritmos de Optimización](notebooks/03-optimizacion-y-modelos-generativos/08-algoritmos-optimizacion.ipynb) | Descenso del gradiente, método de Newton, SGD, Adam, recocido simulado, enjambre de partículas (PSO) y algoritmos genéticos |
| 09 | [Modelos Generativos y Datos Sintéticos](notebooks/03-optimizacion-y-modelos-generativos/09-modelos-generativos-datos-sinteticos.ipynb) | GAN y variantes (WGAN, cGAN), VAE, Normalizing Flows, modelos de difusión, modelos para datos tabulares y métricas de evaluación |

### 04 · Computación cuántica

| # | Notebook | Contenido |
|---|----------|-----------|
| 10 | [Computación Cuántica](notebooks/04-computacion-cuantica/10-computacion-cuantica.ipynb) | Qubits, superposición y entrelazamiento, notación de Dirac, puertas y circuitos, Deutsch-Jozsa, Grover, QFT, Shor, Quantum Machine Learning (VQC, QSVM, QAOA, QNN) y estado del arte del hardware |
| 11 | [Cómputo y Programación Cuántica](notebooks/04-computacion-cuantica/11-computo-programacion-cuantica.ipynb) | Curso práctico en 5 bloques: fundamentos, programación con Qiskit, algoritmos fundamentales (Deutsch, Bernstein-Vazirani, Simon, Grover, SWAP Test), PennyLane y algoritmos variacionales (QAOA, QFT, QPE, HHL, QML) |

## Estructura

```
.
├── notebooks/
│   ├── 01-fundamentos/
│   ├── 02-algoritmos-clasicos/
│   ├── 03-optimizacion-y-modelos-generativos/
│   └── 04-computacion-cuantica/
├── requirements.txt
└── README.md
```

## Cómo usar

Requisitos: Python 3.10 o superior.

```bash
git clone https://github.com/astorress/algoritmos-from-scratch.git
cd algoritmos-from-scratch

python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt

jupyter notebook
```

Abre cualquier notebook de la carpeta `notebooks/` y ejecuta las celdas en orden.

También puedes abrir cualquier notebook en [Google Colab](https://colab.research.google.com): *File → Open notebook → GitHub* y pega la URL del repositorio.

### Notas

- **Dependencias:** las notebooks 01 a 09 solo necesitan la sección base de `requirements.txt` (NumPy, SciPy, Matplotlib y Plotly). Qiskit, PennyLane y PyTorch son más pesadas y solo las usan las notebooks 10 y 11.
- **Hardware cuántico real (10 y 11):** las notebooks corren en simuladores locales (Qiskit Aer y PennyLane). Las celdas que envían circuitos a hardware real de IBM necesitan un token de [IBM Quantum](https://quantum.ibm.com/account): reemplaza el marcador `TU_TOKEN_AQUI` o `PEGA_TU_TOKEN_AQUI` por el tuyo y no lo subas al repositorio.

## Repositorios relacionados

- [math-for-ml](https://github.com/astorress/math-for-ml): álgebra lineal, sistemas de ecuaciones, cálculo vectorial y estadística para ML.
- [ml-from-scratch](https://github.com/astorress/ml-from-scratch): Machine Learning, Deep Learning y Reinforcement Learning implementados desde cero.
- [data-science-lab](https://github.com/astorress/data-science-lab): casos prácticos de data science aplicado con librerías.
