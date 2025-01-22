# AI-DataAssistant
Este proyecto es una aplicación web desarrollada con Flask que combina un modelo predictivo basado en TensorFlow con herramientas de análisis de datos como Pandas. Además, incluye un asistente de IA interactivo capaz de responder preguntas relacionadas con los datos y generar reportes visuales mediante gráficos. La aplicación también consume datos de APIs externas para enriquecer los análisis y reportes.
Estructura de archivos del proyecto

AI-DataAssistant/
│
├── app.py                 # Archivo principal de la aplicación Flask.
├── config.py              # Configuración de la aplicación (e.g., claves API, rutas).
├── requirements.txt       # Lista de dependencias necesarias para el proyecto.
├── README.md              # Descripción del proyecto y guía de instalación.
│
├── models/                # Modelos de aprendizaje automático.
│   ├── model.h5           # Modelo TensorFlow entrenado.
│   └── preprocess.py      # Script para preprocesamiento de datos.
│
├── static/                # Archivos estáticos (CSS, JS, imágenes).
│   ├── css/
│   │   └── styles.css     # Estilos personalizados.
│   ├── js/
│   │   └── scripts.js     # Scripts de frontend, si es necesario.
│   └── images/            # Imágenes estáticas.
│
├── templates/             # Plantillas HTML para renderizar páginas.
│   ├── base.html          # Plantilla base.
│   ├── home.html          # Página principal.
│   ├── analysis.html      # Página de reportes y visualización de datos.
│   └── assistant.html     # Página del asistente de IA.
│
├── utils/                 # Utilidades y funciones auxiliares.
│   ├── api_handler.py     # Funciones para consumir APIs externas.
│   ├── data_analysis.py   # Funciones de análisis y manipulación de datos.
│   └── visualizations.py  # Generación de gráficos con Matplotlib/Seaborn.
│
├── datasets/              # Archivos de datos utilizados en el análisis.
│   └── sample_data.csv    # Archivo CSV de ejemplo.
│
├── logs/                  # Archivos de registro para depuración y monitoreo.
│   └── app.log            # Log de ejecución de la aplicación.
│
└── tests/                 # Pruebas automatizadas.
    ├── test_app.py        # Pruebas para rutas de Flask.
    ├── test_model.py      # Pruebas para el modelo predictivo.
    └── test_utils.py      # Pruebas para utilidades.

Dependencias principales (requirements.txt)

Flask==2.2.2
Flask-Cors==3.0.10
pandas==2.0.3
numpy==1.24.2
tensorflow==2.13.0
matplotlib==3.7.1
seaborn==0.12.2
requests==2.31.0
openai==0.27.6  # Si usas la API de OpenAI para el asistente IA.
scikit-learn==1.3.0
gunicorn==20.1.0  # Para despliegue en producción.

Pasos iniciales

    Clona el repositorio

git clone https://github.com/tu_usuario/AI-DataAssistant.git
cd AI-DataAssistant

Crea un entorno virtual e instala dependencias

python3 -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt

Ejecuta la aplicación

flask run

Abre en el navegador
Ve a http://127.0.0.1:5000 para ver la aplicación en acción.
