# uke.live

Tres instrumentos que se tocan con las manos delante de la webcam: **ukelele** (cuerda), **synth** (síntesis, en la línea de gesture.live) y **txalaparta** (percusión). Todo corre en el navegador — MediaPipe Hand Landmarker para las manos, Web Audio para el sonido — y nada sale del dispositivo.

https://joxemari.github.io/uke-live/

## Cómo se toca

**Ukelele** · mano izquierda cuenta el acorde (1–4 dedos = I–IV, abierta con pulgar = V, cuernos = vi, cuernos y pulgar = vii); la altura elige el voicing; el giro de muñeca el ritmo (recta = patrón, derecha = corcheas, izquierda = negras); el puño apaga. Mano derecha: pasada arriba y abajo rasguea; el patrón te cede dos segundos. Canciones guiadas con hoja de acordes, número de pose, letra, cuenta atrás y voz guía; *Escuchar* hace que la app rasguee por ti.

**Synth** · mano izquierda = pad (pose = grado, altura = spice: triada → 7ª → 9ª → 13ª, giro = filtro, puño = silencio). Mano derecha: dorso a la cámara con la mano cerrada abre el arco de modos; abrir la mano elige. Batería y bajo: pinza un dedo y gira para subir o bajar su peldaño, suelta y se queda. Melodía: la altura elige la nota, la pinza la hace sonar (cuatro voces, una por dedo), el temblor pone vibrato. FX / DJ: filtro, wash, stutter y crush mientras dure la pinza. Sculpt: arp, forma, trémolo, grit, color y spread del pad. Dorso abierto congela; dos puños, silencio total. Con micro: *harmonizer* (tu voz desplazada a las notas del acorde) y *sampler* (graba 8 s o carga un archivo y tócalo con la pinza, por trozos o afinado).

**Txalaparta** · dos manos, dos makilak: golpe seco hacia abajo, la zona horizontal elige la tabla (3, 5 o 7); más rápido, más fuerte.

## Dentro

- `index.html` — toda la aplicación en un archivo: teoría (12 tonos, 8 escalas, acordes diatónicos, matriz editable), detección (pinza, puño, dorso, giro con signo, escaleras con histéresis, rebobinado al soltar), motor de audio (canales por capa, reverb, delay, sidechain del bombo, saturación, compresor, limitador), worklets propios (pitch-shift granular para el harmonizer, detector de tono YIN, grabador del sampler), transporte (corcheas con swing, semicorcheas para batería, bajo, arpegio, trémolo y stutter), toma en horizontal, vertical o ambas, modo ligero automático para máquinas lentas, HUD y lecciones.
- `samples/` — muestras FluidR3_GM (CC BY 3.0): nailon, marimba y woodblock.
- `.github/workflows/pages.yml` — despliegue a GitHub Pages.

Built by [hoks](https://joxemari.github.io/hoks).
