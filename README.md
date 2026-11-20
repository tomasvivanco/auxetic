# AuxiBend Studio — v1

**AI-Driven Form-Finding and Fabrication of Bending-Active Auxetic Structures**

AuxiBend Studio is an interactive web tool for designing bending-active auxetic lattices that are printed flat and bent into shape. It simulates deformation with a particle-spring solver, generates a training dataset, trains a regression surrogate model, and lets that model drive the geometry in real time. It then grades strut thickness for fabrication and exports the result as STL.

*AuxiBend Studio es una herramienta web interactiva para diseñar enrejados auxéticos activos en flexión, que se imprimen planos y luego se curvan. Simula la deformación con un solver de partículas y resortes, genera un dataset, entrena un modelo surrogate de regresión y deja que ese modelo controle la geometría en tiempo real. Luego gradúa el espesor de las barras para la fabricación y exporta el resultado en STL.*

## Features / Funciones

- Analytic reconstruction with a particle-spring solver and live telemetry: displacement, engineering and transverse strain, and strut section radius
- Generates a 2,000-sample dataset and trains a regression model, reporting held-out accuracy
- **AI Prediction** mode: the trained surrogate drives the geometry instead of the solver
- **Smart Fabrication**: graded layers per cell, estimated printed mass and material savings
- **Export STL** for 3D printing

## Download & run / Descargar y usar

1. Click **Code → Download ZIP** (or download only `index.html`). / *Haz clic en **Code → Download ZIP**, o descarga solo `index.html`.*
2. Open `index.html` in a modern browser (Chrome, Firefox, Safari, Edge). / *Abre `index.html` en un navegador moderno.*

You don't need to install anything or use a server or internet connection: the app is a single self-contained file. / *No hay que instalar nada ni usar un servidor o conexión a internet: la app es un solo archivo autocontenido.*

To serve it locally instead / *Para servirla localmente:*

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Research / Investigación

Developed by **Tomas Vivanco** as part of the AuxiBend research line on AI-assisted design and digital fabrication of bending-active auxetic structures (SIGraDi 2026).

## License / Licencia

[MIT](LICENSE) © 2026 Tomas Vivanco
