# 10-Proyects-Python

Este repositorio contiene 10 proyectos en Python que utilizan diversas técnicas y bibliotecas para realizar análisis de datos y procesamiento de archivos. A continuación se presentan detalles sobre los proyectos y el contenido del archivo `Practice.ipynb`.

## Proyectos

1. **Supermercados**
   - Lectura de archivos en diferentes formatos (CSV, JSON, Excel, TXT con diferentes delimitadores)
   - Visualización y manipulación de datos utilizando pandas
   - Ejemplos de cómo cargar datos y mostrar tablas

## Contenido del archivo `Practice.ipynb`

El archivo `Practice.ipynb` contiene los siguientes ejemplos de código:

1. **Listado de archivos en el directorio `supermarkets/`**
   ```python
   import os
   os.listdir('supermarkets/')
   ```

2. **Lectura de un archivo CSV y visualización de datos**
   ```python
   import pandas as pd
   df1 = pd.read_csv('supermarkets/supermarkets.csv')
   df1
   ```

3. **Lectura de un archivo JSON y visualización de datos**
   ```python
   df2 = pd.read_json('supermarkets/supermarkets.json')
   df2.set_index('ID')
   ```

4. **Lectura de un archivo Excel y visualización de datos**
   ```python
   df3 = pd.read_excel('supermarkets/supermarkets.xlsx', sheet_name=0)
   df3
   ```

5. **Lectura de un archivo TXT con comas como delimitador y visualización de datos**
   ```python
   df4 = pd.read_csv('supermarkets/supermarkets-commas.txt')
   df4
   ```

6. **Lectura de un archivo TXT con punto y coma como delimitador y visualización de datos**
   ```python
   df5 = pd.read_csv('supermarkets/supermarkets-semi-colons.txt', sep=";")
   df5.set_index('ID')
   ```

7. **Lectura de un archivo JSON desde una URL y visualización de datos**
   ```python
   df6 = pd.read_json('http://pythonhow.com/supermarkets.json')
   df6.set_index('Address', inplace=True)
   df6
   ```

## Cómo ejecutar los notebooks

1. Clona el repositorio:
   ```bash
   git clone https://github.com/MarioS4t/10-Proyects-Python.git
   ```
2. Navega al directorio del proyecto:
   ```bash
   cd 10-Proyects-Python
   ```
3. Abre el archivo `Practice.ipynb` con Jupyter Notebook:
   ```bash
   jupyter notebook Practice.ipynb
   ```

## Requisitos

- Python 3.x
- pandas
- Jupyter Notebook

Instala los requisitos con el siguiente comando:
```bash
pip install pandas jupyter
```

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request para cualquier mejora o corrección.

## Licencia

Este proyecto está bajo la Licencia MIT.
