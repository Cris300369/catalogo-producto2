
# Plan del Proyecto: Contador de Productos con Firebase

## Visión General

Esta aplicación es un contador de productos simple que se sincroniza con Firebase. La aplicación Flutter permite a los usuarios ver y reiniciar el contador, mientras que un dispositivo ESP32 (simulado a través de un botón en la aplicación) es responsable de incrementar el contador.

## Lógica de Control

- **ESP32 (simulado):** Incrementa un valor de contador en la base de datos de Firebase cada vez que se detecta un producto (simulado con el clic de un botón).
- **Aplicación Flutter:**
  - Lee y muestra el valor del contador en tiempo real.
  - Envía una señal de "reinicio" a Firebase para restablecer el contador a cero.
  - Muestra una alerta cuando el contador alcanza un límite predefinido (por ejemplo, 10).

## Diseño y Estilo (Implementación Actual)

- **Tema:** La aplicación utiliza Material Design 3 con un tema personalizable.
  - **Paleta de Colores:** Se genera una paleta de colores vibrante y consistente para los modos claro y oscuro utilizando `ColorScheme.fromSeed` con un color base de `Colors.deepPurple`.
  - **Tipografía:** Se usan fuentes de Google Fonts para mejorar la legibilidad y la estética. Se emplean `GoogleFonts.oswald` para los títulos y `GoogleFonts.roboto` y `GoogleFonts.openSans` para el cuerpo del texto.
- **Componentes:**
  - **Barra de Aplicación:** Muestra el título de la aplicación y un botón para cambiar entre los temas claro y oscuro.
  - **Tarjeta de Contador:** El contador se muestra dentro de un widget `Card` para darle un aspecto elevado y moderno.
  - **Botones:** Se usan `ElevatedButton.icon` para la acción principal (incrementar) y `TextButton.icon` para la acción secundaria (reiniciar).

## Plan de Implementación

1. **Configurar el proyecto de Flutter:**
   - [x] Crear un nuevo proyecto de Flutter.
   - [x] Añadir las dependencias necesarias de Firebase (`firebase_core`, `firebase_database`).
   - [x] Añadir las dependencias de diseño (`provider`, `google_fonts`).

2. **Diseñar la interfaz de usuario:**
   - [x] Crear un diseño visualmente atractivo con Material Design 3.
   - [x] Implementar un tema para los modos claro y oscuro.
   - [x] Usar fuentes personalizadas con Google Fonts.
   - [x] Mostrar el contador en una tarjeta (`Card`).
   - [x] Añadir un botón para incrementar el contador.
   - [x] Añadir un botón para reiniciar el contador.
   - [x] Añadir un interruptor de tema en la barra de la aplicación.

3. **Integrar con Firebase (Próximos Pasos):**
   - [ ] Configurar un nuevo proyecto de Firebase.
   - [ ] Conectar la aplicación Flutter al proyecto de Firebase.
   - [ ] Implementar la lógica para leer el contador de Firebase en tiempo real.
   - [ ] Implementar la lógica para escribir el "reinicio" en Firebase.
   - [ ] Implementar la lógica para incrementar el contador desde la acción del "ESP32" (botón).
