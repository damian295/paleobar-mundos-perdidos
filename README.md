# Mundos Perdidos 2026 · Río Paraná

Sitio web estático para las Jornadas Mundos Perdidos 2026 del Museo de Ciencias Naturales A. Scasso.

URL prevista:

https://mundos-perdidos.museoscasso.com.ar/

## Archivos principales

- `index.html`: estructura y contenido del sitio.
- `style.css`: diseño visual responsive.
- `app.js`: menú móvil y animaciones suaves.
- `CNAME`: dominio personalizado para GitHub Pages.
- `.cpanel.yml`: despliegue automático a `$HOME/public_html/mundos-perdidos/` desde cPanel Git Version Control.

## Cómo publicarlo

### Opción A: GitHub Pages + DNS en cPanel

1. En GitHub, abrir este repositorio.
2. Ir a **Settings > Pages**.
3. En **Build and deployment**, elegir **Deploy from a branch**.
4. Seleccionar rama `main` y carpeta `/root`.
5. Guardar.
6. En cPanel, crear el subdominio `mundos-perdidos.museoscasso.com.ar` o, si el dominio ya existe, editar su zona DNS.
7. Crear un registro `CNAME` para `mundos-perdidos` apuntando a `damian295.github.io`.
8. Esperar propagación y activar HTTPS en GitHub Pages cuando aparezca disponible.

### Opción B: cPanel Git Version Control

1. En cPanel, crear el subdominio `mundos-perdidos.museoscasso.com.ar` con carpeta `public_html/mundos-perdidos`.
2. En **Git Version Control**, clonar este repositorio:
   `https://github.com/damian295/paleobar-mundos-perdidos.git`
3. En el repositorio dentro de cPanel, usar **Pull or Deploy**.
4. El archivo `.cpanel.yml` copia automáticamente `index.html`, `style.css`, `app.js` y `CNAME` a `public_html/mundos-perdidos`.

## Nota editorial

El programa está cargado como preliminar para permitir ajustes de horarios, nombres de actividades, invitados y enlaces de inscripción sin modificar el diseño general.
