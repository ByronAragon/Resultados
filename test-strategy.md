# Plan de Ataque - Juego de Adivina tu número

El objetivo de este plan de ataque es verificar el correcto funcionamiento del juego "Adivina tu número". El juego consiste en adivinar un número aleatorio entre 1 y 100 en un total de 10 turnos o menos.

## Objetivo de pruebas

El objetivo principal de las pruebas es garantizar que el juego funcione correctamente y proporcione una experiencia adecuada al usuario. Para ello, se verificarán los siguientes aspectos:

1. El juego genera correctamente un número aleatorio entre 1 y 100.
2. El juego limita el número de intentos a 10.
3. El juego muestra los mensajes adecuados en función de los intentos del usuario y la relación con el número aleatorio.
4. El juego deshabilita los campos de entrada y el botón de envío cuando se ha alcanzado el límite de intentos.
5. El juego permite reiniciar una nueva partida después de que se haya alcanzado el límite de intentos.

## Estrategia de pruebas

1. **Prueba de generación de número aleatorio:**
   - Verificar que el número generado esté dentro del rango esperado (entre 1 y 100).

2. **Prueba de límite de intentos:**
   - Realizar 10 intentos válidos y verificar que el juego finalice correctamente al alcanzar el límite de intentos.
   - Realizar un intento adicional y verificar que el juego no permita ingresar un nuevo número y muestre un mensaje adecuado.

3. **Prueba de mensajes y relación con el número aleatorio:**
   - Realizar intentos con diferentes valores y verificar que los mensajes se muestren correctamente:
     - Si el número es mayor que el número aleatorio, el mensaje debe indicar que el número es mayor.
     - Si el número es menor que el número aleatorio, el mensaje debe indicar que el número es menor.
     - Si el número es igual al número aleatorio, el juego debe finalizar y mostrar un mensaje de felicitaciones.

4. **Prueba de reinicio del juego:**
   - Al alcanzar el límite de intentos, reiniciar el juego y verificar que todos los valores se restablezcan correctamente, incluyendo el contador de intentos, los mensajes y la habilitación de los campos de entrada y el botón de envío.

## Entorno de pruebas

Se realizarán pruebas en un entorno de ejecución web que admita HTML, CSS y JavaScript. Se utilizarán herramientas de desarrollo web para inspeccionar y depurar el código, así como para simular interacciones con el usuario.

## Plan de Ejecución

1. Ejecutar la prueba de generación de número aleatorio.
2. Ejecutar la prueba de límite de intentos.
3. Ejecutar la prueba de mensajes y relación con el número aleatorio.
4. Ejecutar la prueba de reinicio del juego.

## Responsabilidades

- **Desarrollador:** Proporcionar el código del juego y asegurarse de que esté listo para ser probado.
- **Probador:** Diseñar el plan de ataque, ejecutar las pruebas y documentar los resultados.
- **Equipo de desarrollo:** Revisar los resultados de las pruebas, solucionar los errores identificados y proporcionar una versión corregida del

 juego.

## Criterios de aceptación

- Todas las pruebas mencionadas en el plan de ataque se han ejecutado y han producido los resultados esperados.
- Los errores identificados durante las pruebas se han corregido y se ha verificado su solución.
- El juego se comporta de manera adecuada y proporciona una experiencia satisfactoria al usuario.