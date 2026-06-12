# Mesociclo 3 — App de entrenamiento

App web para seguir el plan **Fuerza en Balance · Integrated-1** de Fernando Fuentes (3 fases, sesiones A/B/C, 4 semanas cada una). Pensada para usar en el celular durante el entrenamiento.

## Qué hace

- Navegás por **Fase → Sesión (A/B/C) → Semana (1-4)**.
- Cada día muestra sus **bloques** (Fuerza, Hipertrofia, Acondicionamiento) con cada ejercicio en una tarjeta.
- Registrás **peso y reps por serie** y marcás cada ejercicio como hecho.
- Barra de **progreso del día** y botón "Marcar día completo".
- **Notas por ejercicio** para tips de ejecución (se guardan por ejercicio, valen para todas las semanas).
- **Tabla de RM** editable con cálculo automático del 1RM estimado.
- **Preparación al movimiento** (movilidad + entrada en calor) plegable en cada sesión.
- Todo se guarda **en el dispositivo** (localStorage). Funciona **sin conexión**.

## Probar localmente

Abrí `index.html` en el navegador. En el celular: pasá la carpeta y abrila, o usá GitHub Pages (abajo).

> Nota: el `manifest.json` y los íconos solo cargan del todo cuando la app se sirve por HTTP (GitHub Pages), no abriendo el archivo con `file://`. La app igual funciona abierta como archivo.

## Subir a GitHub Pages (ícono + favicon)

1. Creá un repo nuevo en GitHub (ej. `mesociclo`).
2. Subí **todo el contenido de esta carpeta** a la raíz del repo (`index.html`, `manifest.json`, los `icon-*.png`, este README).
3. En el repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, elegí `main` y carpeta `/ (root)`. Guardá.
4. En 1-2 min queda en `https://TU-USUARIO.github.io/mesociclo/`.
5. En el celular, abrí esa URL en el navegador y elegí **"Agregar a pantalla de inicio"**. Queda con ícono propio, a pantalla completa, como una app.

## Cambiar el ícono

Reemplazá los archivos `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` (y `icon-180.png` para iOS) por los tuyos, manteniendo los nombres. El `favicon` está embebido como SVG dentro de `index.html` (buscá `rel="icon"`).

## Archivos

| Archivo | Para qué |
|---|---|
| `index.html` | La app completa (datos + lógica + estilos) |
| `manifest.json` | Config PWA (nombre, colores, íconos) |
| `icon-*.png` | Íconos de la app |
| `README.md` | Esto |
