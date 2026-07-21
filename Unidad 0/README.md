# Unidad 0

Introducir la simulación computacional a partir de la aleatoriedad como principio generativo. En esta unidad se explorarán caminatas aleatorias, distribuciones de probabilidad, ruido y variación como recursos para producir sistemas visuales e interactivos.

## Reto de diseño
### Reto de diseño: Navegar la incertidumbre

Un festival de ciencia y creatividad necesita una experiencia interactiva. Antes de ingresar al evento, los visitantes encontrarán una pantalla interactiva que debe introducir una idea central:

*La incertidumbre no es ausencia de reglas. Diferentes formas de aleatoriedad producen diferentes comportamientos y posibilidades.*

La pregunta orientadora de diseño es:

¿Cómo convertir diferentes formas de aleatoriedad en diferentes significados?

¿Qué tienes qué hacer? Diseña en p5.js una experiencia generativa en tiempo real en la que el visitante pueda influir sobre un sistema sin controlarlo completamente.

El sistema deberá interpretar los siguientes momentos:

**Posibilidad:** todas las direcciones parecen posibles.

**Tendencia:** una pequeña preferencia repetida termina construyendo una dirección.

**Normalidad:** la mayoría de los recorridos permanece cerca de lo habitual.

**Excepción:** un evento improbable permite descubrir un territorio nuevo.

**Influencia:** la presencia del visitante transforma lo que puede ocurrir.

No debes ilustrar literalmente las frases. Debes traducirlas en comportamientos, trayectorias, ritmos, concentraciones o transformaciones.

Condiciones de diseño
La experiencia debe ser una sola pieza coherente, no cinco sketches separados.
Debe combinar significativamente al menos tres conceptos de la unidad: caminata aleatoria, distribuciones de probabilidad, distribución normal, Lévy flight o ruido Perlin.
La interacción debe modificar las probabilidades o reglas del sistema. No basta con cambiar colores, avanzar escenas o dibujar directamente.
El sistema debe continuar funcionando cuando nadie interactúa.
Cada ejecución debe producir variaciones sin perder su identidad visual.
Formato 9:16, full screen y ejecución interactiva en tiempo real.
Bitácora de la unidad
El proceso deberá documentarse en la bitácora permanente del curso en GitHub. Para este reto debe incluir, como mínimo:

La intención conceptual de cada momento.
Experimentos y versiones intermedias.
Decisiones tomadas y alternativas descartadas.
Dificultades y soluciones.
Evidencias visuales y enlace al prototipo.
Uso dado a la IA generativa y cambios realizados sobre sus propuestas.
La bitácora debe mostrar evolución mediante control de versión. No se considera suficiente subir únicamente el resultado final.

### Conceptualización

El reto de diseño utiliza como ancla para el desarrollo el hecho de que esto es una pieza visual para un festival de ciencia y creatividad. Me gustaria implementar este concepto ancla en algo que utilice sistemas o recursos similares a los que se pueden observar en materia de ejemplos de la unidad 0 del libro. No solo porque ya me encuentro familiarizado con su comportamiento, si no que tambien me permite ejemplificar el concepto que quiero tratar: Una convencion de astronomia, cuyo tema central son los agujeros negros. La manera en como funcionaria la experiencia visual seria similar a lo que se espera cuando se observan cuerpos celestiales; tienen un comportamiento "predecible" pero que ciertas anomalias indetectables, modifican su comportamiento temporalmente.

No hay metafora que funcione mejor que los cuerpos celestiales para ejemplificar la incertidumbre. Ellos mismos estan ligados a leyes fisicas precisas, pero ciertas influencias externas alteran la manera en como se perciben.

El concepto de walker, explorado en la unidad, me permite trabajar esta idea de manera eficiente. Los comportamientos simples de los walker responden al comportamiento esperable de objetos celestiales, y permite mediente otras reglas escondidas, cambiar su comportamiento si estos son influenciados de cierta manera. (La gravedad, el redshift, entre otros conceptos referentes a cuerpos celestiales.)

