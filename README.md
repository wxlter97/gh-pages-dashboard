# Mis Proyectos

Panel estático que lista, en vivo, todos los repositorios públicos de
[@wxlter97](https://github.com/wxlter97) que tienen **GitHub Pages activado**
y el topic `showcase`.

Publicado en: https://wxlter97.github.io/gh-pages-dashboard/

## Cómo funciona

- Es una única página HTML sin build ni dependencias.
- En el navegador consulta `https://api.github.com/users/wxlter97/repos` y
  filtra los repos donde `has_pages === true` y `topics` incluye `showcase`.
- El resultado se cachea 5 minutos en `localStorage` para no gastar el límite
  de la API sin autenticar (60 solicitudes/hora).

## Publicar u ocultar un proyecto

No hay que tocar este repo. Para que un proyecto aparezca en el panel:

1. Asegúrate de que tenga GitHub Pages activado.
2. Agrégale el topic **`showcase`** (Settings → General → Topics en la web,
   o desde la sección "About" del repo en la app móvil de GitHub).

Para ocultarlo, quita ese topic.
