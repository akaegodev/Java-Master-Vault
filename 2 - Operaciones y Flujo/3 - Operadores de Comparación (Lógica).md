
---

> **CONCEPTO:** Operadores que enfrentan dos valores para determinar su relación. El resultado de estas operaciones **SIEMPRE** es un tipo de dato `boolean` (`true` o `false`).

### 📝 EXPLICACIÓN

En programación, las decisiones no son grises, son blancas o negras. Estos operadores permiten que el programa "pregunte" sobre el estado de las variables. Sin ellos, el código sería una lista de instrucciones fija sin capacidad de reacción.

Cuando escribes `a > b`, Java no solo mira los números; realiza una operación lógica interna que arroja un resultado booleano que puedes guardar en una variable o usar directamente.

### ✅ EJEMPLOS Y USOS REALES:

- **Control de acceso:** `if (edad >= 18)` -> Permite decidir si el usuario entra o no.
    
- **Mecánicas de juego:** `if (vida <= 0)` -> Determina el estado de "Game Over".
    
- **Validación de datos:** `if (inputUsuario != null)` -> Evita que el programa se rompa por falta de información.
    
- **Sistemas de puntos:** `if (puntuacionActual > recordHistorico)` -> Para actualizar récords.
### ❌ ERRORES COMUNES (Los que te harán fallar):

- **El "Falso Positivo" (`=` vs `==`):**
    
    - El error más famoso de la historia: usar `=` (asignación) dentro de una comparación.
        
    - _Ejemplo:_ `if (vidas = 0)` no pregunta si tienes 0 vidas, ¡te las pone a 0! Para preguntar usa siempre **`==`**.
        
- **Orden de los símbolos combinados:**
    
    - Java solo entiende `>=` y `<=`. Si escribes `=>` o `=<`, el compilador se volverá loco. Piensa que la flecha siempre apunta hacia el valor y el igual es el cierre.
        
- **Comparar Peras con Manzanas:**
    
    - Intentar comparar un `String` con un `int`. `if ("10" == 10)` dará error. Java no convierte el texto en número automáticamente para comparar.
        
- **La trampa del `double`:**
    
    - Comparar decimales con `==` puede ser peligroso por la precisión (`0.1 + 0.2` no siempre es exactamente `0.3` en memoria). Para lógica crítica de dinero o medidas, hay que tener cuidado con las comparaciones de igualdad pura.