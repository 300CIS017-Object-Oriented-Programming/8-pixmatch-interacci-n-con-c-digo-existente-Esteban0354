## Requisitos Funcionales y Criterios de Aceptación
### 1. Configuración de Nivel de Dificultad
**Requisito:** El sistema debe permitir a los jugadores seleccionar el nivel de dificultad antes de comenzar el juego.

**Criterios de Aceptación:**
- Opciones de dificultad fácil, medio y difícil disponibles para selección.
- La configuración de dificultad debe influir en la mecánica del juego, como la frecuencia de regeneración de imágenes y la puntuación.
- Tiempos de regeneración específicos:
  - Fácil: cada 8 segundos.
  - Medio: cada 6 segundos.
  - Difícil: cada 5 segundos.

**Requisito** El sistema debe identificar si el icono seleccionado es igual al icono buscado.

**Criterios de Aceptación:**
- Si el icono seleccionado es igual al icono buscado, este se debe reemplazar por el icono ✅️.
- Si el icono seleccionado es igual al icono buscado, este se debe reemplazar por el icono ❌.

**Requisito** Cada que un icono sea seleccionado, se debe generar un nuevo tablero.

**Criterios de Aceptación**
- Sin importar si el icono seleccionado es igual al icono buscado se debe generar un nuevo tablero.
- Se deben mantener la posicion en el tablero de los simbolos ❌ y ✅.

**Requisito** El sistema debe actualizar el puntaje cada que un icono sea seleccionado.

**Criterios de aceptacion**
- Cada que un icono sea seleccionado, sin importar si es igual al buscado, o no seleccione ningun icono despues
del tiempo estipulado segun la dificultad, el puntaje se debe actualizar.
- La cantidad de puntos que gana el usuario depende de la dificultad y de la cantidad de errores que haya cometido, cada
que se cometa un error se le otorgara un punto menos por cada respuesta correcta al usuario.
- Puntos segun dificultad:
  - Facil:
    - Respuesta Correcta: +10
    - Respuesta Incorrecta: -1
    - Cambio de puntos por no responder: 0
  - Medio:
    - Respuesta Correcta: +8
    - Respuesta Incorrecta: -1
    - Cambio de puntos por no responder: -1
  - Dificil:
    - Respuesta Correcta: +6
    - Respuesta Incorrecta: -1
    - Cambio de puntos por no responder: -1


**Requisito** El sistema debe reconocer cuando ha terminado el juego y debe mostrar el puntaje final obtenido por el usuario.

**Cristerios de aceptación**
- El juego se va a dar por terminado cuando el número de iconos restantes para seleccionar sea igual a cero.

**Requisito** El sistema debe llevar un registro de cuantos iconos pendientes por seleccionar se encuentran en el tablero.

**Criterios de aceptación**
- Se le debe restar 1 al total de iconos disponibles para seleccionar sin importar si el icono seleccionado es igual al
icono buscado.
- En caso de que haya un cambio de icono buscado por tiempo, el número se debe mantener igual.