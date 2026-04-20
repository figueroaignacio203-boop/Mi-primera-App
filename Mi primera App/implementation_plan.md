# Aplicación de Trivia Estilo "Preguntados" (Películas de Acción)

El objetivo es crear una aplicación web dinámica, colorida y atractiva al estilo del popular juego "Preguntados" (Trivia Crack). El juego constará de 10 preguntas centradas en el género de películas de acción, con una sola respuesta correcta por pregunta.

## User Review Required

> [!WARNING]
> Dado que el directorio de trabajo actual (`Myprimerproyecto`) contiene los archivos de un proyecto anterior (Landing Page de WhatsApp), **sobreescribiré los archivos `index.html`, `style.css` y `main.js`** con el código del nuevo juego. Si prefieres conservar el proyecto anterior, avísame para crear la aplicación de trivia en una subcarpeta distinta.

## Open Questions

1. **Estética:** He planificado una paleta de colores vibrante (naranja, azul, verde, amarillo) con bordes redondeados y animaciones suaves, típica de juegos móviles. ¿Hay algún color principal que te gustaría destacar o prefieres un modo oscuro?
2. **Dificultad:** Las preguntas están diseñadas para ser de dificultad media/conocimiento general sobre películas clásicas y modernas de acción. ¿Te parecen bien?

## Proposed Changes

### Archivos Principales del Proyecto

Se actualizarán completamente los siguientes archivos en la raíz del proyecto para construir la nueva aplicación:

#### [MODIFY] index.html
Estructura de la aplicación. Contendrá tres secciones principales (pantallas) manejadas vía JavaScript:
- **Pantalla de Inicio:** Título animado del juego y botón de "Comenzar Juego".
- **Pantalla de Juego:** Contenedor de la pregunta actual, indicador de progreso (ej. Pregunta 1 de 10), puntaje actual y cuadrícula con 4 opciones de respuesta.
- **Pantalla de Resultados:** Puntaje final, mensaje de felicitación/ánimo según el puntaje, y botón para "Volver a Jugar".

#### [MODIFY] style.css
Sistema de diseño (Design System).
- **Colores:** Paleta lúdica y contrastante (botones interactivos con efectos hover y active).
- **Tipografía:** Uso de fuentes modernas (Google Fonts: 'Nunito' o 'Poppins' para darle un toque amigable).
- **Animaciones:** Transiciones suaves al cambiar de pregunta, efectos de rebote (bounce) al seleccionar respuestas correctas, y vibración (shake) al seleccionar incorrectas.
- **Responsividad:** Diseño pensado primero para móviles (Mobile First) pero que se verá excelente en escritorio, con un contenedor central tipo "tarjeta" o "smartphone".

#### [MODIFY] main.js
Lógica del juego.
- Array de objetos con las 10 preguntas, opciones y la respuesta correcta.
- Funciones de estado (estado actual de la pregunta, puntaje).
- Manejo de eventos del DOM para validar la respuesta del usuario.
- Funciones para transicionar entre las pantallas de Inicio, Juego y Resultados.

### Lista de Preguntas (Temática: Películas de Acción)
1. ¿Quién interpretó a John McClane en la saga "Duro de Matar" (Die Hard)? (R: Bruce Willis)
2. En la película "Matrix", ¿qué pastilla elige Neo para descubrir la verdad? (R: La roja)
3. ¿Cuál de estas películas protagoniza Keanu Reeves como un asesino a sueldo buscando venganza por su perro? (R: John Wick)
4. ¿Cómo se llama el personaje de Arnold Schwarzenegger en la película "Terminator"? (R: T-800)
5. En "Gladiador", ¿cuál es el nombre del general romano que se convierte en esclavo y luego en gladiador? (R: Máximo Décimo Meridio)
6. ¿Qué actor interpreta a Ethan Hunt en la saga de "Misión Imposible"? (R: Tom Cruise)
7. En "Mad Max: Furia en la carretera", ¿quién es el dictador del Páramo que persigue a Max y Furiosa? (R: Immortan Joe)
8. ¿Cómo se llama el maestro de artes marciales que entrena a La Novia en "Kill Bill"? (R: Pai Mei)
9. En la película "Depredador" (1987), ¿en qué entorno se desarrolla la acción principal? (R: La selva centroamericana)
10. ¿Cuál de estos actores NO forma parte del equipo principal original en "Los Indestructibles" (The Expendables)? (R: Dwayne "The Rock" Johnson)

## Verification Plan

### Manual Verification
- Iniciar el servidor local (usando Live Server o abriendo el HTML).
- Probar el flujo de inicio de juego.
- Responder preguntas seleccionando opciones correctas e incorrectas para verificar las animaciones, la lógica de validación y la suma de puntos.
- Comprobar que la pantalla final muestre el puntaje correcto y permita reiniciar el juego.
- Verificar la correcta visualización (diseño "premium", responsivo) tanto en vistas de escritorio como de móvil en el navegador.
