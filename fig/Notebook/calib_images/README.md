# Imágenes de calibración

Coloca aquí las fotos del tablero de ajedrez usadas para calibrar la cámara.

- Patrón: tablero de ajedrez de **8×8 casillas** → **7×7 esquinas internas**.
- Tamaño real de cada cuadrado: **17 mm** (`square_size = 17.0` en el notebook).
- Formatos aceptados: `.jpg`, `.jpeg`, `.png`.
- Recomendado: entre 10 y 20 fotos del tablero en distintas orientaciones.
  (El notebook calibra con un mínimo de 3 detecciones válidas.)

El notebook `IAyMR_20261119_Calibracion_Pose.ipynb` lee todas las imágenes
de esta carpeta con:

    glob.glob("fig/Notebook/calib_images/*.jpg")  # y .jpeg / .png

## Consejos para que la detección funcione (tablero azul/brillante)
- Evita reflejos fuertes del vidrio y zonas sobreexpuestas.
- Mantén el tablero lo más **plano** posible (sin curvar la funda).
- Enfoca bien y procura que las 7×7 esquinas internas queden completas en la foto.
