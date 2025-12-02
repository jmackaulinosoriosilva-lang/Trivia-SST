Cómo ejecutar los tests

Este proyecto incluye un runner de pruebas simple basado en navegador.

1) Levanta el servidor estático desde la raíz del proyecto:

```bash
python3 -m http.server 8000
```

2) Abre en tu navegador:

http://localhost:8000/tests/test-runner.html

El runner cargará `index.html` en un iframe y ejecutará varias comprobaciones automáticas de UI.
