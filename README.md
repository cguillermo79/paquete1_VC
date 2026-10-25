# Mi Paquete de Estadística (mi_paquete1)

Paquete de Python diseñado para calcular estadísticas descriptivas y generar visualizaciones gráficas a partir de vectores numéricos.

## Características

- Cálculo de media, mediana, desviación estándar, varianza, mínimo, máximo, cuartiles y rango intercuartílico (IQR).
- Generación de histogramas con curva KDE y diagramas de caja.
- Estructura de empaquetado mediante `pyproject.toml`.

## Requisitos

- Python 3.8 o superior.
- Git instalado para realizar la instalación directamente desde GitHub.

Las dependencias del paquete son `numpy`, `pandas`, `matplotlib` y `seaborn`.

## Instalación

Ejecute en la terminal:

```bash
python -m pip install "git+https://github.com/msmejia/mi_paquete1.git"
```

## Ejemplo de uso

```python
import numpy as np
from mi_paquete import visualizar_estadisticas_vector

# Generar datos de prueba
np.random.seed(42)
datos = np.random.normal(loc=65, scale=12, size=1000)

# Calcular estadísticas y visualizar resultados
resultados = visualizar_estadisticas_vector(datos)

# Mostrar resultados
print("\nResultados obtenidos:")
print(f"Media: {resultados['Media']:.2f}")
print(f"Desviación estándar: {resultados['Desviación Estándar']:.2f}")
```

## Resultados

La función muestra en consola las estadísticas descriptivas y genera dos gráficos: un histograma con curva de densidad KDE y un diagrama de caja.

También devuelve un diccionario de Python con las estadísticas calculadas.

## Autor

Ing. Edwin Mejía — Trabajo inicial, ESPOCH.
