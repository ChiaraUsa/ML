
# Proyecto de Clasificación de MNIST con SVM

## Integrantes del Grupo
- Chiara Vivian Valenzuela Losada.
- Oscar Eduardo Miranda Puentes.
- Mitchell Phillip Bermin Suarez.

## Descripción del Proyecto
Este proyecto utiliza una Máquina de Vectores de Soporte (SVM) para clasificar imágenes del dataset MNIST. El modelo es entrenado con diferentes tamaños de muestras para evaluar su precisión en los conjuntos de entrenamiento y validación.

### Requisitos de Configuración

#### Requisitos de Software y Librerías:
- **Python**: Python 3.7 o superior es necesario para asegurar compatibilidad con todas las librerías y características del código.
- **Librerías de Python**:
  - `numpy`: Para manejo de arrays y operaciones matemáticas.
  - `matplotlib`: Para la generación de gráficos y visualización de datos.
  - `scikit-learn`: Proporciona herramientas esenciales para el machine learning, como los modelos SVM y las funciones de cálculo de precisión.
  - `pandas`: Utilizado para la manipulación y análisis de datos.
  - `pathlib`: Para manejo de rutas de archivos de forma orientada a objetos.
  - `urllib.request`: Necesario para la descarga de datos desde Internet.
  - `packaging`: Utilizada para comparar versiones de librerías, asegurando la compatibilidad.

#### Instalación de Librerías:
Para un entorno local, puedes instalar las librerías necesarias utilizando pip. Ejecuta el siguiente comando en tu terminal o prompt de comandos:
```bash
pip install numpy matplotlib scikit-learn pandas
```

Si estás utilizando Google Colab, la mayoría de estas librerías ya estarán preinstaladas; solo asegúrate de que las versiones sean compatibles.

#### Configuración Específica para Google Colab:
Para usuarios de Google Colab, es necesario montar Google Drive para acceder a los archivos de datos:
```python
from google.colab import drive
drive.mount('/content/drive')
```

#### Verificación de la Configuración del Entorno:
Antes de ejecutar el proyecto, verifica que la versión de Python y scikit-learn cumplan con los requisitos mínimos necesarios:
```python
import sys
assert sys.version_info >= (3, 7)

import sklearn
from packaging import version
assert version.parse(sklearn.__version__) >= version.parse("1.0.1")
```

Estas verificaciones aseguran que el entorno está correctamente configurado y es capaz de ejecutar el código sin problemas.

#### Ejecución del Código:
Una vez configurado el entorno, puedes ejecutar el código en Jupyter Notebook o Google Colab siguiendo estas instrucciones. Asegúrate de que todos los archivos de datos, como `mnist-data.npz`, estén ubicados en la ruta especificada en el script.

##Referencias
1. GfG, A. (2020, julio 1). Ways to import CSV files in Google Colab. GeeksforGeeks. https://www.geeksforgeeks.org/ways-to-import-csv-files-in-google-colab/

2. Khadija. (2021, septiembre 8). What if there is a lot of outliers in your dataset. Stack Overflow. https://stackoverflow.com/questions/69104651/what-if-there-is-a-lot-of-outliers-in-your-dataset

3. LeCun, Yann and Cortes, Corinna and Burges, CJ. (2010). MNIST handwritten digit database. TensorFlow. http://yann.lecun.com/exdb/mnist