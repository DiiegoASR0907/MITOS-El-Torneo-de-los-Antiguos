# Dirección de arte — MITOS

## Identidad visual

**Estilo objetivo:** anime de fantasía oscura con siluetas muy legibles, contornos firmes, acentos luminosos y efectos de impacto exagerados. Cada personaje debe reconocerse por su postura y forma general incluso antes de ver sus colores.

La ilustración conceptual inicial de Bigfoot y Chupacabras sirve como referencia de tono y personalidad, no como sprite final ni como material integrado automáticamente en el juego.

## Bigfoot — El Guardián del Bosque

- **Silueta:** cuerpo enorme, torso ancho, brazos largos y piernas pesadas.
- **Materiales:** pelaje castaño en capas; sombras profundas y reflejos cálidos.
- **Rasgos distintivos:** melena y hombros de pelo, rostro robusto, faja roja y vendas rústicas.
- **Personalidad de combate:** resistente, directo y poderoso; sus movimientos deben sentirse pesados.
- **Afinidad visual:** ámbar y cobre.
- **Idea para su especial:** *Golpe Sísmico*, una onda de choque que recorre el suelo.

## Chupacabras — El Depredador Nocturno

- **Silueta:** cuerpo delgado y encorvado, extremidades largas, postura de acecho y garras prominentes.
- **Materiales:** placas azul grisáceo, espinas magenta y sombras azul noche.
- **Rasgos distintivos:** hocico anguloso, ojos rojos brillantes, espinas dorsales y cola afilada.
- **Personalidad de combate:** rápido, impredecible y agresivo; prioriza ataques cortos y desplazamientos veloces.
- **Afinidad visual:** rojo carmesí y violeta.
- **Idea para su especial:** *Lanza de Espinas*, una descarga rápida de energía y púas.

## Estado de implementación

- [x] Paletas cromáticas individuales para el plantel.
- [x] Primera pasada de rasgos de silueta para Bigfoot y Chupacabras en el renderizado Canvas.
- [x] Perfiles y nombres visibles en la selección de personajes.
- [ ] Sustituir los cuerpos geométricos por sprites originales dibujados por poses.
- [ ] Crear animaciones de reposo, caminar, salto, golpe, especial, daño, bloqueo y victoria.
- [ ] Probar legibilidad y escala en escritorio y móvil.
- [ ] Extender la misma guía de silueta, materiales y efectos al resto del plantel.

## Nota de producción

La versión actual sigue siendo un prototipo. Los detalles añadidos son formas vectoriales dibujadas en tiempo real, no ilustraciones rasterizadas ni hojas de sprites. No presentar el arte provisional como arte final.


## Iteración de combate — animación y efectos

La primera implementación mantiene los luchadores dibujados en Canvas 2D mediante formas vectoriales procedurales. Esto permite animar reposo, desplazamiento, salto, ataque y especial sin cargar imágenes externas ni alterar el sistema de colisiones.

- **Impacto normal:** destello corto, partículas claras, texto de golpe y retroceso.
- **Especial:** anillo de energía del color propio del luchador, ráfaga de partículas ampliada y mayor sacudida de cámara.
- **Defensa:** chispa cian y retroceso reducido; el daño sigue mitigado.
- **Bigfoot:** los tonos ámbar/tierra representan la fuerza física y el impacto sísmico.
- **Chupacabras:** los tonos magenta/carmesí representan espinas y energía depredadora.

**Alcance honesto:** esta etapa mejora los efectos de combate y la animación procedural, pero no equivale aún a sprites rasterizados dibujados cuadro a cuadro. El siguiente salto artístico será sustituir progresivamente las formas procedurales por hojas de sprites originales con transparencia y cuadros consistentes.


## Pareja de referencia — primera pasada de animación

La primera pasada de poses de combate en Canvas refuerza cinco estados legibles: reposo con respiración sutil, locomoción con balanceo de piernas, salto con extremidades recogidas, ataque con extensión del brazo delantero y especial con una carga de energía más amplia.

- **Bigfoot:** barrido ámbar, núcleo de energía cálida y trazos de impacto de fuerza.
- **Chupacabras:** estelas magenta, núcleo luminoso y líneas de energía que enfatizan su velocidad.
- Las colisiones, la energía, el daño, la defensa y el retroceso siguen gestionados por el sistema de combate existente.

Esta es una animación procedural de referencia, no una hoja de sprites cuadro a cuadro. Se usará para evaluar siluetas, tiempos y legibilidad antes de reemplazarla por sprites originales definitivos.
