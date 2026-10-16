# nephei-songs

[songs.nephei.org](https://songs.nephei.org): canciones para aprender chino. Unas hechas con IA para repasar vocabulario del HSK y otras de artistas reales, con la letra línea a línea en caracteres, pinyin e inglés.

## Estructura

- `public/index.html`: la página. Pinta las canciones a partir de `songs.js`.
- `public/songs.js`: los datos. **Para añadir una canción, basta con añadir una entrada aquí.** El formato está explicado al principio del fichero.
- `wrangler.jsonc`: configuración del Worker `nephei-songs` (solo assets estáticos, sin código de servidor).

## Despliegue

El repositorio está conectado al Worker `nephei-songs` con Workers Builds: cada push a `main` lo despliega en `songs.nephei.org`.
