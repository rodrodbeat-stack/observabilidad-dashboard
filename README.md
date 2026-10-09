# Dashboard de Observabilidad

Dashboard web estático para visualizar métricas, logs y trazas distribuidas mediante datos demostrativos.

## Contenido

- `index.html`: aplicación completa del dashboard.
- `.github/workflows/deploy.yml`: despliegue automático con GitHub Pages al hacer push a `main`.
- `.nojekyll`: evita el procesamiento de Jekyll en GitHub Pages.

## Ejecutar localmente

Abre `index.html` en un navegador. Si prefieres servirlo localmente con Python:

```bash
python3 -m http.server 8000
```

Luego visita `http://localhost:8000`.

## Publicar en GitHub Pages

1. Crea un repositorio público llamado `observabilidad-dashboard`.
2. Sube el contenido de esta carpeta directamente a la raíz del repositorio (no subas el ZIP como un único archivo).
3. En GitHub, entra a **Settings → Pages** y selecciona **GitHub Actions** como fuente.
4. Haz push a la rama `main`; el workflow desplegará la web automáticamente.

> Las métricas y eventos son de demostración; esta página no se conecta por sí sola a sistemas productivos.
