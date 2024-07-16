# Challenge MeLi
#### Autor: Juan Ovalle


## Overview
Este repositorio contiene el codigo utilizado para resolver el Challenge MeLi de Data Scientist.

## Estructura del repositorio
| Folder/File | Description |
| ----------- | ------------|
| `data/` | Debe ser populado con los datos originales (`MLA_100k_checked_v3.jsonlines`). Despues de la ejecucion del notebook `00_prepare_data.ipynb` deben aparecer los datos en formato ``.parquet`` (`data.parquet.gzip`) |
| `notebooks/` | Contiene todos los notebooks utilizados para resolver el challenge.  |

- ``00_prepare_data.ipynb``: Contiene un breve analisis inicial (valores faltantes, tipos de datos y duplicados) la extraccion de algunas variables, y la transformacion a formato `.parquet`.
- `01_eda.ipynb`: Contiene el analisis exploratorio de los datos. Este esta compuesto por analisis univariados y multivariados.
- `02_modelado.ipynb`: Contiene todos los pasos utilizados para entrenar y seleccionar el modelo de clasificacion.
- `03_explicabilidad.ipynb`: Contiene el analisis de los valores SHAP del modelo de clasificacion.

## Setup e Instalacion

### Prerequisitos
- Python 3.11
- Poetry

### Pasos
1. Instalar Python 3.11 (se recomienda pyenv):
   ```
   pyenv install 3.11
   ```

2. Instalar Poetry:
   ```
   pip install poetry
   ```

3. Instalar dependencias:
   ```
   poetry install
   ```