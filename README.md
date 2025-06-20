# 🎨 ColorFinder

**ColorFinder** es un proyecto de automatización en Python diseñado para extraer paletas de colores dominantes desde imágenes en sitios web de diseño de interiores y muebles. El objetivo es facilitar la creación de herramientas para diseñadores, decoradores y desarrolladores de apps que trabajan con color y estética visual.

---

## 🧠 Objetivo

El proyecto automatiza el proceso de navegación y recolección de imágenes desde sitios web populares del rubro, y extrae los colores más representativos de cada imagen. La información puede ser utilizada para:

- Inspirar paletas de diseño para ambientes.
- Clasificar espacios por gama de colores.
- Sugerir combinaciones cromáticas en aplicaciones.

---

## ⚙️ Tecnologías utilizadas

- **Python 3.10+**
- **Scrapy**: crawling estructurado de sitios web.
- **Playwright**: interacción con páginas dinámicas (scroll, carga JS).
- **Colorthief / Pillow / OpenCV**: procesamiento de imagen para extraer colores.
- **Pandas**: manipulación de datos tabulares.
- **JSON / CSV / SQLite**: almacenamiento de resultados.
- **(Opcional) Streamlit**: visualización interactiva de paletas.

---

## 🔁 Flujo del proyecto

1. Scraping de sitios web de diseño o decoración para obtener URLs de imágenes y metadatos.
2. Descarga temporal de imágenes.
3. Análisis automático para extraer colores dominantes.
4. Clasificación por tipo de ambiente, estilo o categoría.
5. Exportación del resultado a CSV / JSON / visualización.

---

## 📂 Estructura del proyecto (sugerida)
ColorFinder/
├── scraper/
│ ├── spiders/
│ │ └── example_spider.py
│ ├── middlewares.py
│ ├── pipelines.py
│ └── settings.py
├── image_processing/
│ └── color_extractor.py
├── data/
│ ├── raw/
│ ├── processed/
│ └── outputs/
├── visualizer/
│ └── app.py (opcional con Streamlit)
├── requirements.txt
└── README.md


---

## 🚀 Cómo correr el proyecto

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/tuusuario/ColorFinder.git
   cd ColorFinder

2. Instalar dependencias:
bash
pip install -r requirements.txt

3. Ejecutar el spider (ejemplo):
bash
scrapy crawl example_spider

4. Procesar imaganes y extraer colores:
bash
python image_processing/color_extractor.py

5. Ejecutar el visualizador:
streamlit run visualizer/app.py

🧪 Estado del proyecto
🚧 En desarrollo — ¡se aceptan sugerencias y mejoras!