# Trivia de SST

Este es un pequeño juego de trivia sobre Seguridad y Salud en el Trabajo (SST) preparado para demostraciones.

Características añadidas en la iteración más reciente:
- Interfaz profesional y responsive (degradado rojo-negro)
- Subida de avatar con validación (1 sola casilla)
- Preview y persistencia en localStorage
- Más preguntas y mejor experiencia de juego (barra de progreso, temporizador, animaciones)
- Tests de integración simples en browser (tests/test-runner.html)

Cómo ejecutar localmente:

```bash
# desde la raíz del proyecto
python3 -m http.server 8000
# abrir en tu navegador
http://localhost:8000
# tests
http://localhost:8000/tests/test-runner.html
```

Si quieres, puedo añadir compresión de imágenes, validaciones adicionales o pruebas end-to-end automáticas (Playwright).

Despliegue (GitHub Pages)
--------------------------

Se ha añadido un workflow de GitHub Actions para desplegar el sitio en GitHub Pages automáticamente a la rama `gh-pages` cuando se hace push a `main`.

Pasos para activar el despliegue:

- Asegúrate de que el repositorio está en GitHub y que tienes permisos para escribir.
- El workflow añadido es `.github/workflows/deploy-gh-pages.yml` y se despliega desde la raíz del repositorio.
- La acción utiliza el token `GITHUB_TOKEN` incorporado, por lo que no necesitas configurar secretos adicionales.
- Después de hacer push a `main`, en la pestaña "Actions" verás el workflow en ejecución; cuando termine, GitHub Pages servirá el contenido publicado en la rama `gh-pages`.

Notas y recomendaciones:

- Optimiza `assets/img/sd_logo.png` antes de desplegar en producción (archivo actual ~5MB). Recomiendo reducirlo a <300KB.
- Si prefieres que despliegue desde otra rama o usar Netlify/Vercel, puedo añadir configuraciones para esos servicios.

Si quieres que intente hacer el commit y push desde este entorno, dime y lo intento (nota: puede requerir credenciales si no están configuradas). 
