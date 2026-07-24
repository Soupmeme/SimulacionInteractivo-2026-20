# Navegar la incertidumbre

**Reto de diseño — Consorcio de Agujeros Negros** · Curso basado en *The Nature of Code*, Cap. 0

150 estrellas de masa variable se mueven alrededor de un único agujero negro. El sistema vive, en todo momento, en uno de 5 estados — nunca depende de un visitante para ser interesante; el clic solo interrumpe el ciclo y fuerza un quinto estado propio.

---

## Los 5 momentos, como estados

| Estado | Qué hace | Se ve como | Cómo se activa |
|---|---|---|---|
| **Posibilidad** | Dirección y paso libres, amplios | Dispersión enérgica, sin rumbo | Autónomo (4–7 s) |
| **Normalidad** | Paso gaussiano, calmo | Vibración contenida | Autónomo (4–7 s) |
| **Tendencia** | Rumbo hacia el centro (`atan2`) + desvío de ruido Perlin | Corriente gravitacional | Autónomo (5–8 s) |
| **Excepción** | Ráfaga breve de saltos grandes | Disrupciones de marea (TDE) | Autónomo, breve (1.5–2.5 s) |
| **Influencia** | Pull más fuerte y más directo que Tendencia | Respuesta directa al visitante | Clic sostenido |

El sistema elige el siguiente estado autónomo al azar (ponderado, Excepción es el más raro) al expirar cada temporizador. Un clic interrumpe esto en cualquier momento; al soltar, el ciclo continúa como si nada.

---

## Cómo se mantiene vivo

- **Una sola variable de estado real** (`state`), no probabilidades recalculadas cada cuadro.
- **Adopción escalonada:** cada partícula reacciona al cambio con un retraso según su distancia al centro — se ve como una onda, no un corte sincronizado.
- **Masa individual por estrella:** deriva tamaño, brillo y qué tan directo cae hacia el centro (licencia artística, no física real).
- **Horizonte de eventos:** la materia que se acerca demasiado se recicla en otro punto — el sistema nunca se vacía.

---

## Especificaciones

| | |
|---|---|
| Formato | 9:16, escritorio |
| Motor | p5.js, tiempo real (~60 fps) |
| Entrada | Mouse (clic sostenido) |
| Variación | Semilla aleatoria por corrida, misma identidad visual |

---

## Checklist

- [x] Pieza única, no 5 sketches
- [x] 4 conceptos combinados (caminata aleatoria, distribución normal, ruido Perlin, salto tipo Lévy)
- [x] Interacción cambia el estado del sistema, no una posición
- [x] Visualmente activo sin interacción
- [x] Varía por corrida sin perder identidad
- [x] Dentro de las herramientas del Capítulo 0 (salvo la máquina de estados, pedida por el profesor)

---

Decisiones, alternativas descartadas, dificultades encontradas y uso de IA generativa: ver `bitacora.md`.
