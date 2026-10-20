# Pruebas unitarias de Bubble Sort

## Descripción

Este proyecto implementa y verifica el algoritmo de ordenamiento **Bubble Sort** mediante pruebas unitarias en Python 3. Se utiliza el framework `unittest` para las pruebas y `pytest-cov` para medir la cobertura del código.

## Estructura del proyecto

```text
Pruebas-bubble-sort/
├── main/
│   ├── __init__.py
│   └── bubble_sort.py
├── test/
│   ├── __init__.py
│   └── test_bubble_sort.py
├── requirements.txt
├── README.md
└── .gitignore
```

## Requisitos

- Python 3
- pip
- Entorno virtual de Python (`venv`)

Las dependencias del proyecto están definidas en `requirements.txt`:

- `pytest`
- `pytest-cov`

## Instalación

Clona el repositorio y entra en la carpeta del proyecto:

```bash
git clone https://github.com/MoisesCcaso/Pruebas-bubble-sort
cd Pruebas-bubble-sort
```

Crea y activa el entorno virtual en Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Instala las dependencias:

```bash
python3 -m pip install -r requirements.txt
```

## Ejecución de las pruebas unitarias

Para ejecutar las pruebas con `unittest`:

```bash
python3 -m unittest discover -s test
```

## Cobertura de código

Para ejecutar las pruebas y mostrar la cobertura en la terminal:

```bash
python3 -m pytest --cov=main.bubble_sort --cov-report=term-missing test
```

Para generar un informe HTML de cobertura:

```bash
python3 -m pytest --cov=main.bubble_sort --cov-report=term-missing --cov-report=html test
```

El informe se genera en `htmlcov/index.html`. Para abrirlo en Linux:

```bash
xdg-open htmlcov/index.html
```

## Casos de prueba

Las pruebas se basan en los cuatro casos definidos para evaluar el comportamiento del algoritmo:

| Caso | Entrada | Resultado esperado | Descripción |
|---|---|---|---|
| CP1 | `[7]` | `[7]` | Lista con un elemento |
| CP2 | `[1, 2]` | `[1, 2]` | Lista ordenada sin intercambios |
| CP3 | `[2, 1]` | `[1, 2]` | Lista que requiere un intercambio |
| CP4 | `[3, 1, 2]` | `[1, 2, 3]` | Lista que requiere varias comparaciones e intercambios |

## Autor

**Moises Robert Ccaso Idme**
