# Oído Musical · Pack de audio premium v0.8.0

Sube TODO el contenido de esta carpeta a la raíz del repositorio
`oido-musical-audio-pack` (rama main). La app lo detecta vía CDN.

## Novedades v0.8.0
- Frases reales de VIOLÍN (3) y PÁJARO (3): completados los dos últimos huecos.
- NUEVO juego "Épocas de la música" (solo 3.º ciclo): el alumnado escucha una pieza
  histórica ÍNTEGRA y decide a qué época pertenece entre 3 opciones. Al responder, el
  audio se detiene. Carpeta audio/eras/<época>/.
  · 8 épocas: Antigua Grecia, Antigua Roma, Edad Media, Renacimiento, Barroco,
    Clasicismo, Romanticismo, Siglo XX (19 piezas en total).
- La app ya NO usa sintetizador: todo el sonido proviene de samples reales.
- La app solo se abre si la descarga ha sido correcta; si falla, ofrece reintentar.

## Estructura
- audio/phrases/<id>/fraseN.mp3   — frases reales de instrumentos, animales y naturaleza
- audio/instruments/<id>/<Nota>.mp3 — notas reales (respaldo del motor de frases y modo Color)
- audio/eras/<época>/<épocaN>.mp3  — piezas históricas íntegras (sin recortar)

Audio de instrumentos/efectos: mono, 44,1 kHz, MP3 160 kbps, −16 LUFS.
Piezas de época: estéreo, conservan su duración original; solo normalizadas en volumen.

## Etiquetas corregidas musicológicamente
- Susato (Danserye) → Renacimiento (no Barroco)
- Vivaldi (La primavera) → Barroco (no Clasicismo)
- Cantigas de Santa María → Edad Media (no Renacimiento)

## Notas
- Antigua Roma y Renacimiento tienen 1 pieza cada una; para reforzarlas, añade más
  piezas a su carpeta y al manifest (campo eras.pieces).
- Licencias: VCSL (CC0) e instrumentos/efectos propios; piezas históricas con fin educativo.
