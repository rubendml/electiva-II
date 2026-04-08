# Prueba Lectiva

Base SvelteKit con arquitectura `feature-first/domain-first` para integrar la API de Rick and Morty.

## Run

```bash
npm install
npm run dev
```

## Check

```bash
npm run check
npm run build
```

## Deploy en GitHub Pages

El proyecto queda preparado para publicarse con GitHub Actions en GitHub Pages.

1. En GitHub ve a `Settings > Pages`.
2. En `Source` selecciona `GitHub Actions`.
3. Cada push a `main` ejecuta el workflow de build y despliegue.

Para probar localmente un build equivalente al de Pages:

```bash
$env:BASE_PATH="/electiva-II"
npm run build
```

## Estructura

- `src/lib/core`: cliente HTTP, configuracion y adaptadores.
- `src/lib/entities`: tipos y mapeos de dominio.
- `src/lib/features`: features por caso de uso.
- `src/routes`: composicion de rutas y carga de datos.
