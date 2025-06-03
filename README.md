# 🌋 Visualización de Volcanes y población en un Mapa Interactivo

Bienvenido a **Mapa Interactivo**, un proyecto de visualización interactiva de volcanes y datos demográficos mundiales usando Python y tecnologías web modernas.

---

## 🚀 Descripción

Este proyecto genera un mapa interactivo que muestra la ubicación y altitud de volcanes en Estados Unidos y otros países, junto con información demográfica mundial. El objetivo es combinar datos geográficos y científicos para crear una herramienta visual educativa y atractiva.

---

## 🛠️ Herramientas y Tecnologías Utilizadas

- **Python 3**  
  Lenguaje principal para el procesamiento de datos y generación del mapa.

- **Pandas**  
  Para la manipulación y análisis de datos tabulares (`Volcanoes.txt`).

- **Folium**  
  Librería Python para crear mapas interactivos basados en Leaflet.js.

- **Leaflet.js**  
  Framework JavaScript para mapas interactivos (integrado a través de Folium).

- **Bootstrap**  
  Framework CSS para mejorar la visualización y responsividad del mapa.

---

## 📂 Estructura del Proyecto

```
App1_Mapa/
│
├── mapping.py         # Script principal de generación del mapa
├── Volcanoes.txt      # Base de datos de volcanes (CSV)
├── world.json         # Datos GeoJSON de países y población
├── map.html           # Mapa interactivo generado
└── README.md          # Este archivo
```

---

## 🗺️ ¿Cómo funciona?

1. **Lectura de datos**  
   Se cargan los volcanes desde `Volcanoes.txt` y los países desde `world.json`.

2. **Procesamiento**  
   Se asigna un color a cada volcán según su altitud:
   - 🟢 Verde: < 1000 m
   - 🟠 Naranja: 1000–2999 m
   - 🔴 Rojo: ≥ 3000 m

   Los países se colorean según su población.

3. **Visualización**  
   Se genera un mapa interactivo (`map.html`) con capas seleccionables:
   - Volcanes (con popups de altitud)
   - Población mundial


## ▶️ Uso rápido

1. Instala las dependencias:
   ```bash
   pip install pandas folium
   ```
2. Ejecuta el script:
   ```bash
   python mapping.py
   ```
3. Abre `map.html` en tu navegador favorito.


¡Explora, aprende y comparte! 🌍🌋
