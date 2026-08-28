# Regalos de Mistria

Buscador de regalos de **Fields of Mistria** (versión 1.0) en español. Escribes el
nombre de un vecino y ves al instante lo que le encanta, lo que le gusta, lo que
no le gusta y lo que odia. También funciona al revés: buscas un objeto y te dice
a quién dárselo.

- 34 personajes, 474 objetos
- Todo en español, con el nombre original en inglés debajo (las traducciones de
  la comunidad no coinciden entre sí, así que el inglés te saca de dudas)
- Modo claro y oscuro
- Una sola página, sin dependencias ni compilación

## Ponerlo en marcha

```bash
git clone https://github.com/TU-USUARIO/regalos-mistria.git
cd regalos-mistria
python3 descargar-sprites.py     # baja los sprites a assets/ (una sola vez)
```

Luego abre `index.html` en el navegador. Ya está.

Si te saltas el script, la web funciona igual: carga los sprites desde la wiki
(necesita internet) y, si tampoco puede, usa iconos dibujados a mano.

## Publicarlo en GitHub Pages

1. Sube el repo a GitHub.
2. Settings → Pages → Source: `Deploy from a branch`, rama `main`, carpeta `/ (root)`.
3. En un par de minutos estará en `https://TU-USUARIO.github.io/regalos-mistria/`.

Ejecuta `descargar-sprites.py` **antes** de subir el repo si quieres que los
sprites viajen con la web.

## Qué hay en cada archivo

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | La aplicación entera: datos, estilos y lógica |
| `descargar-sprites.py` | Baja los PNG del juego a `assets/` |
| `assets/` | Los sprites, una vez descargados |

## De dónde salen los datos

Las listas de regalos vienen de las guías de la versión 1.0 de GameSpot y
TechRaptor, contrastadas con la [Fields of Mistria Wiki](https://fieldsofmistria.wiki.gg).
Las traducciones al español son propias.

## Sobre los sprites

Los PNG son arte de **NPC Studio** y siguen siendo suyos. `descargar-sprites.py`
los copia desde la wiki para uso personal. Si vas a publicar esto en abierto,
pide permiso antes o quédate con los iconos dibujados, que son originales.
