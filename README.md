# Brújula Lab

Ejercicio interactivo para la clase de Monitoreo, Evaluación y Learning del programa Learning Design (UdeSA Educación Ejecutiva).

Los equipos eligen la pregunta del comité, validan una teoría de cambio, arman un tablero de métricas con 100 puntos de esfuerzo para un asistente de IA, reciben recomendaciones y guardan su reflexión. El tablero de la clase se arma en vivo con tres gráficos: lo que creen vs. lo que miden, qué capas miraron y qué tensión pesó al elegir.

## Archivos

| Archivo | Qué es |
|---|---|
| `index.html` | La app completa (HTML, CSS y JavaScript en un solo archivo). |
| `Code.gs` | El backend: un Google Apps Script que guarda los equipos en una Google Sheet. |

## Puesta en marcha

1. Crear una Google Sheet nueva en Drive.
2. En la Sheet: **Extensiones → Apps Script**. Borrar el contenido y pegar `Code.gs`. Guardar.
3. **Implementar → Nueva implementación → Aplicación web**. Ejecutar como: *yo*. Quién tiene acceso: *cualquier usuario*. Autorizar y copiar la URL (termina en `/exec`).
4. En `index.html`, pegar la URL en `const SCRIPT_URL = "";`.
5. Subir `index.html` al repositorio y activar **Settings → Pages** (rama `main`, carpeta raíz).

## Uso en clase

- Participantes: abren el link de GitHub Pages.
- Facilitador: abre el mismo link y comparte pantalla con «Tablero de la clase».
- Para vaciar el tablero entre ediciones: borrar las filas (menos la primera) en la hoja «equipos».
- Los datos quedan en la Sheet, una fila por equipo, para analizarlos después.

## Cambios en el Apps Script

Después de editar `Code.gs`: **Implementar → Administrar implementaciones → editar (lápiz) → Versión: nueva versión → Implementar**. Así la URL no cambia.
