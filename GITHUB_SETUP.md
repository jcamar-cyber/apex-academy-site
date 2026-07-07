# Guía GitHub para APEX Academy

## Recomendación de repositorios

Usar una sola cuenta de GitHub personal y crear dos repositorios separados:

1. `apex-academy-program`
   - Propósito: documentos internos del programa, charter, misiones, bitácoras, evidencias, arquitectura y roadmap.
   - Visibilidad recomendada: privado.

2. `apex-academy-site`
   - Propósito: sitio web público de APEX Academy.
   - Visibilidad recomendada: público si se usará GitHub Pages gratis y no contiene información sensible.

## Estructura recomendada del repositorio del programa

```text
apex-academy-program/
├── 00_charter/
├── 01_framework/
├── 02_misiones/
├── 03_bitacora/
├── 04_evidencias/
├── 05_templates/
├── 06_roadmap/
└── README.md
```

## Estructura recomendada del repositorio de la página

Este paquete ya está listo para el repositorio `apex-academy-site`:

```text
apex-academy-site/
├── index.html
├── 404.html
├── robots.txt
├── assets/
├── docs/
├── netlify.toml
├── vercel.json
├── README.md
├── GITHUB_SETUP.md
└── .gitignore
```

## Crear repositorio desde GitHub Web

1. Entrar a GitHub.
2. Seleccionar `+` y luego `New repository`.
3. Crear `apex-academy-site`.
4. Subir todos los archivos de esta carpeta.
5. Ir a `Settings > Pages`.
6. Source: `Deploy from a branch`.
7. Branch: `main`.
8. Folder: `/root`.
9. Guardar.

## Crear repositorio usando Git en consola

Reemplazar `TU_USUARIO` por tu usuario real de GitHub:

```bash
cd apex_academy_site
git init
git add .
git commit -m "Initial APEX Academy website"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/apex-academy-site.git
git push -u origin main
```

## Actualizar cambios futuros

```bash
git add .
git commit -m "Update APEX Academy website"
git push
```

## Nota de seguridad

No subir claves, contraseñas, tokens, archivos `.env`, datos internos de clientes ni documentación sensible al repositorio público del sitio web.
