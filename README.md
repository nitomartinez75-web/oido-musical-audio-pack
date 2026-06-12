# Oído Musical · Pack de audio premium v0.6.0

Muestras reales para la app Oído Musical. Sube TODO el contenido de esta carpeta
a la raíz del repositorio GitHub `oido-musical-audio-pack` (rama main).
La app lo detecta automáticamente vía jsDelivr (manifest.json, versión 0.6.0).

## Contenido
- audio/instruments/<id>/<Nota>.mp3 — notas reales por instrumento (mono, 44,1 kHz, 160 kbps, sonoridad −16 LUFS)
  piano (18, vertical Yamaha · VCSL), violin (8), violonchelo (5), bajo (7, contrabajo pizzicato),
  saxo (5), clarinete (3, clarinete bajo), flauta (25, grabación propia),
  marimba (5), xilofono (4), glockenspiel (4)
- audio/phrases/<id>/ — patrones rítmicos reales compuestos a partir de golpes VCSL:
  claves, caja_china, maracas (shaker), bombo y pandero (cajón), crotalos (campanas de mano)
- audio/phrases/{perro,oveja,caballo,gallina,gato}/ — grabaciones propias (mejor segmento, 3 s)
  · caballo, gallina y gato ya están integrados en la app (v3 con manifest 0.6.0).

## Licencias
- VCSL (Versilian Community Sample Library): CC0 — sin restricciones.
- Flauta y animales: material propio del autor.

## Notas técnicas
- Las notas ausentes en el material original se generaron desde la muestra real más
  cercana (desplazamiento ≤5 semitonos) con compensación de afinación medida (±35 cents).
- El clarinete usa clarinete bajo (misma familia tímbrica); incluye D4, F4 y A#4.
  El motor de frases de la app se adapta a las notas disponibles.
