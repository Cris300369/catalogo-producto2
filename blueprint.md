# Blueprint

## Visión General

Una aplicación de contador en Flutter con un diseño sofisticado y cohesivo de "glassmorphism", una paleta de colores elegante en tonos de azul y morado, una interfaz de usuario intuitiva y alertas interactivas completamente estilizadas en español.

## Características

*   **Diseño de Vanguardia (Glassmorphism):**
    *   La tarjeta del contador y el **diálogo de confirmación** utilizan un efecto de cristal esmerilado (`BackdropFilter`) para una apariencia unificada, elegante y moderna.
    *   Un fondo degradado que transiciona de un azul claro a un morado oscuro, creando una atmósfera serena y atractiva.

*   **Paleta de Colores y Tipografía:**
    *   **Texto Blanco Uniforme:** Todo el texto de la aplicación, incluidos los diálogos y botones, es de color blanco para lograr un contraste nítido y una estética limpia.
    *   El tema principal de la aplicación (`primarySwatch`) está configurado en `Colors.blue`.
    *   El botón de acción principal y otros elementos de acento utilizan tonos de azul para una apariencia profesional.
    *   Utiliza Google Fonts para una tipografía moderna.

*   **Interfaz de Usuario Optimizada:**
    *   **Acción Principal Clara:** El botón "Añadir" es un `FloatingActionButton` extendido y centrado, destacándose como la acción principal.
    *   **Acción Secundaria Accesible:** El botón "Reiniciar" está ubicado como un ícono en la `AppBar`, un lugar convencional para acciones secundarias.

*   **Contador Interactivo:**
    *   Un botón principal para incrementar el contador.
    *   Cuando el contador alcanza 20 (y para cada incremento posterior), un diálogo de confirmación estilizado solicita al usuario permiso para continuar.

*   **Localización:**
    *   Toda la interfaz de usuario está en español.
