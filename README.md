# Shin Megami Tensei: Strange Journey Redux — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/nintendo-3ds/shin-megami-tensei-strange-journey-redux)**.

Traducción al **español de España** de *Shin Megami Tensei: Strange Journey Redux* (Nintendo 3DS, Atlus, 2017), que nunca salió en español. Se ha hecho sobre la **edición europea en inglés**; no es una traducción directa del japonés.

La primera opción es el parche **LayeredFS**; también hay un **XDELTA** alternativo. Necesitas tu propia copia del juego: ninguna descarga incluye una ROM.

## Estado

Versión **1.0**: guion completo, interfaz de texto, gráficos de interfaz y escenas de vídeo.

| Parte | Alcance |
|---|---|
| Guion e interfaz de texto | **21.652 mensajes** traducidos (17.590 textos únicos): historia, misiones, negociación con demonios, compendio, objetos, habilidades, menús y ayudas |
| Texto dentro de imágenes | **25 texturas** de interfaz: menú de título, barra de botones, combate, estado, menú Demonica, compendio, fusión, guardado, mapa y visor |
| Vídeos | **119 textos en 11 vídeos** (introducción, apertura animada, escenas de Alex y epílogo), sustituidos en la propia imagen |
| Caracteres españoles | **á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿ « »** en los cinco tamaños de fuente del juego |

Se conservan los nombres de demonio y de hechizo de la saga (Jack Frost, Agi, Bufu…), los logotipos y rótulos de marca, y las voces originales. La terminología sigue la de nuestra traducción de *Shin Megami Tensei IV: Apocalypse* (PS/PM, Nivel, Macca…).

### Comprobaciones y límites

- Todo el texto se ha reinsertado con validación automática de etiquetas, codificación, ancho en píxeles con la fuente real del juego y líneas por cuadro; los límites se midieron en el emulador.
- Traducción por lotes con biblia y glosario comunes, revisión independiente de cada lote y pasadas de unificación.
- **Prueba jugable en Azahar 2126.0:** tres rondas desde partida nueva (unas 4 horas en total): introducción y vídeos, escena inicial, nombre del protagonista, sala de mando, Cubierta, llegada al Schwarzwelt y primera planta del Sector Antlia, con combates, análisis, negociación y reclutamiento de demonios, huida, subida de nivel, menú Demonica, Laboratorio (desarrollar y reciclar), Opciones y **guardado y carga reales**. Sin cuelgues ni glifos vacíos.
- El LayeredFS se ha comprobado en Azahar. El XDELTA se ha reaplicado sobre la ROM original con resultado idéntico a la ROM reconstruida, y esa ROM arranca en Azahar sin mods hasta la escena inicial.
- **Pendiente:** no se han jugado la fusión de demonios, los jefes ni los sectores posteriores a Antlia; falta una partida completa hasta los finales y la prueba en consola física. No se certifican todas las ventanas, rutas ni el contenido descargable.
- Siguen en inglés algunos gráficos menores: las insignias «NEW», «1ST/2ND/RESULT» del menú de fusión, el rótulo «mission failed» del vídeo de fin de partida y los rótulos de marca y de las noticias de la escena inicial. Dos cadenas del ejecutable también siguen en inglés: «NOT FOUND» en la pantalla de resultados y el aviso del menú de contenido descargable.
- Detalles de maquetación conocidos: en la cabecera de la ficha de análisis la tilde de la «í» puede verse recortada («Espíritu»), y en la lista de datos de demonios una raza larga puede quedar pegada al nombre.
- Los vídeos traducidos guardan el audio en PCM (idéntico al original una vez descodificado); la recompresión de la imagen puede suavizarla ligeramente.

La traducción y la revisión se han hecho con asistencia de modelos de IA; no se atribuye una revisión humana independiente.

## Descarga

En **[Releases](../../releases)**:

1. **LayeredFS — primera opción:** `sjr-es-v1.0.zip`, para Luma3DS o Azahar.
2. **XDELTA — alternativa:** `sjr-rom-es-v1.0.xdelta`, para crear una ROM `.3ds` ya traducida.

Ambos contienen la misma traducción. Elige uno de los dos métodos.

- SHA-256 del ZIP: `5f8fdd7d56535b42c3e8f8a2a047e5522ef93ed9751eb1400613bbf0035092a7`
- SHA-256 del XDELTA: `15f1106ada0189b27e5df09baad0eb68e1f9f4e52487d4c6348a4a8de7967e05`

## Versión necesaria

| Dato | Valor |
|---|---|
| Edición | Europa, juego base sin otros parches |
| Código de producto | `CTR-P-AJ9P` |
| Title ID | `00040000001CE100` |
| ROM usada en las pruebas | `Shin Megami Tensei - Strange Journey Redux (Europe).3ds` |
| Tamaño | 2.147.483.648 bytes |
| MD5 | `31a9ebbcfec0b4c6e8843649f49883f1` |
| SHA-256 (ROM descifrada) | `de0e88270729cdc0272509cdbf03e808cbe62fa10c6c719a08070ec3f6ada4b3` |

El **XDELTA exige esta ROM exacta**. Para LayeredFS basta con la edición europea del juego base; la huella identifica el volcado de prueba. No es compatible con las ediciones americana ni japonesa y no se ha verificado con actualizaciones u otros mods.

## Cómo instalar

### Opción 1: LayeredFS en Nintendo 3DS con Luma3DS

1. Extrae el ZIP y copia la carpeta `luma` a la raíz de la tarjeta SD.
2. Comprueba que quede `luma/titles/00040000001CE100/romfs/`.
3. En la configuración de Luma3DS (mantén SELECT al encender), activa **Enable game patching** y guarda.
4. Inicia tu copia europea del juego.

### Opción 1: LayeredFS en Azahar

1. Haz clic derecho sobre el juego y abre su **carpeta de modificaciones** (*Open Mods Location*).
2. Copia allí la carpeta `romfs` que hay dentro de `luma/titles/00040000001CE100/` en el ZIP.
3. Cierra y vuelve a iniciar el juego. No cargues estados rápidos creados con otra versión del parche (las partidas guardadas del juego sí sirven).

Para desinstalarla, borra esa carpeta `romfs` de la carpeta de mods (o de `luma/titles/00040000001CE100/`).

### Opción 2: XDELTA para una ROM traducida

1. Comprueba que tu ROM europea tiene el tamaño y las huellas de arriba:

   ```bash
   md5sum "Shin Megami Tensei - Strange Journey Redux (Europe).3ds"      # Linux
   md5 "Shin Megami Tensei - Strange Journey Redux (Europe).3ds"         # macOS
   CertUtil -hashfile "Shin Megami Tensei - Strange Journey Redux (Europe).3ds" MD5   # Windows
   ```

2. Aplica el parche con [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o con:

   ```bash
   xdelta3 -d -s "Shin Megami Tensei - Strange Journey Redux (Europe).3ds" sjr-rom-es-v1.0.xdelta "Shin Megami Tensei - Strange Journey Redux (ES).3ds"
   ```

3. La ROM resultante ocupa **2.147.483.648 bytes**, MD5 `786f589bf2aa7e61f074ccadd7b05820` y SHA-256 `7fa6062db7fab1d1f7851812c4fdae83d48f864c0456a182452c8a82671c99e1`.
4. Ábrela sin LayeredFS: la traducción ya está integrada.

## Cambios

### v1.0 — 2026-10-07

- Primera versión pública: guion, interfaz, gráficos de interfaz y vídeos en castellano.

## Créditos y aviso

Proyecto de **johanderohan / Parches en Castellano**. Juego y materiales originales de **ATLUS** y **SEGA**. Traducción de aficionados sin relación oficial con ellos.

Herramientas: utilidades propias de extracción y reinserción, [Azahar](https://github.com/azahar-emu/azahar), [3dstool](https://github.com/dnasdw/3dstool), xdelta3, [FFmpeg](https://ffmpeg.org/) y [mobipeg](https://github.com/quatric/mobipeg) para los vídeos. Las letras castellanas reutilizan la fuente del juego; algunos rótulos gráficos usan además letras de fuentes libres con licencia SIL OFL (Liberation, Noto y Fira).

El repositorio contiene solo este README; el parche está en Releases. No se publican ROMs, partidas ni el guion extraído. Si encuentras un problema, abre una incidencia indicando versión del parche, emulador o consola y una captura.
