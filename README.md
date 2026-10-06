# Hoja de trabajo 2: Transformers y mecanismos de atención

Este proyecto contiene un notebook reproducible para cargar `bert-base-uncased` y `gpt2`, extraer sus matrices de atención y analizar visualizaciones, resolución de pronombres, máscaras causales, attention sinks y entropía por capa.

## Instalación y ejecución

Se recomienda Python 3.10 o superior:

```bash
python -m venv .venv
pip install -r requirements.txt
jupyter notebook transformers_atencion.ipynb
```

La primera ejecución descarga los modelos de Hugging Face. El notebook selecciona CUDA automáticamente cuando está disponible, pero también funciona en CPU. Las figuras se guardan en `outputs/bert`, `outputs/gpt2` y `outputs/metrics`.

## Contenido

- Configuración reproducible y carga de ambos modelos.
- Funciones reutilizables para extraer y visualizar atención.
- Cuatro visualizaciones de cabezas distintas.
- Comparación automática de `it` con `animal` y `street`.
- Verificación numérica de la máscara causal de GPT-2.
- Medición de attention sinks y entropía por capa.
- Celdas de discusión que deben completarse a partir de las salidas reales.
