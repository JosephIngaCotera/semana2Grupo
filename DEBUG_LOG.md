# DEBUG_LOG

## Registro de depuración y validación

Este archivo documenta incidencias detectadas durante la validación del proyecto web `Semana02Grupo`, junto con las correcciones manuales aplicadas y el resultado obtenido.

## Errores encontrados durante la validación

### 1. Falta de soporte claro para navegación por teclado

- **Error detectado:** No todos los elementos relevantes del flujo de navegación ofrecían una referencia clara para usuarios que usan teclado.
- **Evidencia en el proyecto:** Fue necesario asegurar un enlace de salto al contenido principal y un destino enfocable.
- **Corrección aplicada:** Se incorporó el enlace `skip-link` en [index.html](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/index.html:13) y se agregó `tabindex="-1"` al elemento [main](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/index.html:41).
- **Resultado:** La navegación por teclado permite saltar directamente al contenido principal y posicionar correctamente el foco.

### 2. Deficiencias de accesibilidad semántica y descriptiva

- **Error detectado:** Algunos elementos interactivos y secciones requerían nombres accesibles y relaciones semánticas explícitas para mejorar la interpretación por lectores de pantalla.
- **Evidencia en el proyecto:** Durante la validación se verificó la necesidad de usar `aria-label`, `aria-labelledby` y `aria-hidden` en elementos clave.
- **Corrección aplicada:** Se mantuvieron y ajustaron atributos ARIA en navegación, encabezado, contenido principal, artículos y panel lateral, por ejemplo en [index.html](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/index.html:16), [index.html](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/index.html:31), [index.html](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/index.html:42) y [index.html](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/index.html:150).
- **Resultado:** La estructura es más comprensible para tecnologías asistivas y mejora la accesibilidad general del sitio.

### 3. Señal visual insuficiente del foco en componentes interactivos

- **Error detectado:** Los enlaces y controles interactivos necesitaban una indicación visual más evidente al recibir foco.
- **Evidencia en el proyecto:** La validación de accesibilidad exigía una retroalimentación visual clara para navegación no táctil.
- **Corrección aplicada:** Se definieron estilos con `:focus-visible` en [styles.css](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/styles.css:61), [styles.css](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/styles.css:182) y [styles.css](c:/Users/Joseph/Desktop/Desarrollo%20de%20aplicaciones%20web/Semana02Grupo/styles.css:404).
- **Resultado:** El foco ahora es visible en enlaces, control de tema y contenido principal, facilitando la interacción con teclado.

## Correcciones manuales realizadas

1. Se revisó la estructura semántica del HTML.
2. Se verificó el uso de atributos ARIA en zonas clave de navegación y contenido.
3. Se aseguraron estilos de foco visibles en elementos interactivos.
4. Se confirmó la navegación por teclado hacia el contenido principal.

## Conclusión

La validación permitió identificar y corregir tres incidencias importantes relacionadas con accesibilidad y navegación. Como resultado, el proyecto presenta una estructura más robusta, mejor soporte para teclado y una experiencia más clara para usuarios y herramientas de asistencia.
