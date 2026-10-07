# Créditos

## Aplicación web activa

Cartas especiales **Fantasma / Medianoche** y **Dorada / Ónix**: ilustraciones generadas
con la herramienta de imágenes de OpenAI el 2026-10-06, a partir de la propuesta
visual elegida por el autor del proyecto. Plantillas locales en
`assets/cards/specials/`; rango, palo y nombre se dibujan por HTML/CSS.
Carmesí, Pirata, Fortuna y Forjadora reutilizan recortes de la lámina aprobada
`assets/designs/classes-concept.png`, extraídos con `scripts/extract-special-art.py`.
Las 36 parejas de clases reutilizan seis imágenes base: las distintas muestran
mitades verticales iguales (jugador a la izquierda, rival a la derecha), mediante CSS.
No hay assets nuevos para combinaciones. Los índices fijos se borraron al extraer
los cuatro nuevos diseños para dibujar el valor y palo reales por HTML/CSS.
Estos archivos son arte generado para el proyecto, no recursos Kenney ni CC0.

La distribución de Spec 002 selecciona 52 caras y un dorso de **Kenney Board Game Pack**,
la madera **Wood049**, el tejido **Fabric030**, las fuentes **Inter** y **Libre Baskerville**. Se conservan sus
licencias y procedencias detalladas debajo. No se incluyen Joker, fichas PNG ni el
catálogo Playing Cards Pack del primer MVP. Los archivos originales no se modificaron.

- Iconos: **Lucide 0.468.0**, Lucide Contributors; porciones de Feather por Cole Bemis.
	[Origen](https://github.com/lucide-icons/lucide), ISC con el aviso de Feather incluido.
- Evaluador de manos: **phe 0.6.0**, Thorsten Lorenz, MIT.
	[Origen](https://github.com/thlorenz/phe). Biblioteca sin modificar; adaptador TypeScript propio.
- [Avisos de dependencias web](assets/licenses/web-dependencies.txt), conservados desde
	las versiones fijadas en el lockfile. El build concatena estos avisos y las licencias
	de los recursos seleccionados en `THIRD-PARTY-NOTICES.txt` dentro de la distribución.
- Tejido **Fabric030**, ambientCG / Lennart Demes, CC0 1.0:
	[origen](https://ambientcg.com/a/Fabric030) y [licencia](assets/licenses/ambientCG-CC0.txt).
	Mapa de color sin modificar; tinte verde y escalado por CSS.
- Luz, papel, anillas, fichas apiladas, dorsos decorativos, lápiz y ruleta: HTML/CSS propios en
	[web/src/style.css](web/src/style.css) y [web/src/table-materials.css](web/src/table-materials.css),
	implementados con GitHub Copilot el 2026-10-06. Método: capas CSS, bordes, sombras y
	texturas Wood049 y Fabric030 locales; sin imágenes generadas ni RNG de juego para decoración.
	Las correcciones orientan composición y materiales, no se utilizan como fondos.

El [inventario](assets/manifest.json) registra la selección web, su procedencia y licencia.
Los recursos restantes permanecen disponibles para el respaldo Godot.

## Inicio, sala y personajes

COR-009: ocho hojas de caminata de Pipe, Gary, Buhler y Ulda (cardinales y diagonales), generadas con `image_gen` integrado de OpenAI el 2026-10-07, dirigidas y aportadas por el autor a partir de los personajes aprobados. Modelo no informado. Prompts, referencias y método en `assets/designs/casino/walk-v1/README.md` y `walk-diagonal-v1/README.md`; hashes en el inventario. PNG intactos, ventanas CSS con normalización y ancla de pies, sin nuevas imágenes compuestas ni licencia CC0 ajena.

Correcciones del 2026-10-07: ilustración de menú aportada por el autor en COR-006, conservada sin modificar en `assets/designs/casino/menu-principal.png`. COR-008 incorpora el arte vertical aportado, sin modificar, como `assets/designs/casino/menu-mobile.png`: ventanas CSS muestran casino/título/cartas y un sector del piso sin rótulos. Herramienta/modelo de generación no informados en los adjuntos; no se asigna licencia CC0 de terceros. Los botones son HTML/CSS interactivos; las ventanas CSS excluyen los controles dibujados. El selector reutiliza las hojas aprobadas de personajes. Las seis mesas de la sala reutilizan ventanas CSS del fondo aprobado; suelo, paredes y HUD son CSS propio. No se generaron nuevos bitmaps ni se copiaron objetos de alcohol de la referencia del selector.

Pipe, Gary, Buhler, Ulda, crupier y sala: arte generado con la herramienta integrada `image_gen` de OpenAI, dirigido y aprobado por el autor, 2026-10-06. Modelo no informado por la herramienta. Assets en `assets/designs/casino/`; prompts y referencias documentados allí y en el inventario. Las fotografías privadas no se distribuyen. Las hojas se reutilizan con recorte CSS, sin copiar arte de The Binding of Isaac.

Música **Jazz**, Julie Damsgaard / Spring Spring / Spring Enterprises, [OpenGameArt](https://opengameart.org/content/jazz-1), **CC0 1.0**. OGG local sin modificar; reproducción en bucle y volumen regulable. Evidencia: `assets/licenses/casino-audio.txt`. Efectos cortos sintetizados originales en `web/src/audio.ts`.

## Recursos y respaldo Godot

Cartas originales del primer MVP: **Kenney**, [Playing Cards Pack](https://kenney.nl/assets/playing-cards-pack), CC0 1.0.
Sin modificaciones en los archivos originales. Atribución voluntaria.

Fuente **Inter**, The Inter Project Authors, SIL Open Font License 1.1.
Fuente y avisos originales en [Google Fonts](https://github.com/google/fonts/tree/main/ofl/inter).

Licencias completas: `assets/licenses/`. Inventario y hashes: `assets/manifest.json`.
Mesa, paneles, indicadores y ruleta: controles y geometría propios del proyecto en Godot.
Documentos originales y dirección del juego: autor del proyecto.

Cartas y fichas de la reconstrucción: **Kenney**,
[Board Game Pack](https://kenney.nl/assets/boardgame-pack), **CC0 1.0**.
PNG originales, sin modificación; evidencia en assets/licenses/Kenney-Boardgame-CC0.txt.
Mesa oval, madera, paño y anillas: geometría propia en scripts/ui/table_surface.gd y
notebook_paper.gd, creada en Godot el 2026-10-06 con las correcciones como referencia
de composición. Las tres imágenes adjuntas no se incorporan como assets de producción.

Refinamiento visual del 2026-10-06:
- **Libre Baskerville**, The Libre Baskerville Project Authors, SIL OFL 1.1.
	[Origen](https://github.com/google/fonts/tree/main/ofl/librebaskerville) y
	[licencia incluida](assets/licenses/LibreBaskerville-OFL.txt). Fuente sin modificar.
- **Wood 049**, ambientCG / Lennart Demes, CC0 1.0.
	[Origen](https://ambientcg.com/a/Wood049) y
	[evidencia de licencia](assets/licenses/ambientCG-CC0.txt). Mapa de color original;
	tinte y escalado durante el renderizado.
- Fieltro, iluminación de mesa, fichas apiladas, papel y ruleta: dibujo procedural
	propio en Godot, implementado con GitHub Copilot siguiendo las tres referencias.
	El ruido visual usa una semilla local y no consume el RNG de la partida.
