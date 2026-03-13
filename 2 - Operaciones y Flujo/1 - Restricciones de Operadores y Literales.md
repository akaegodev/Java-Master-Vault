
---

> **CONCEPTO:** Los operadores de incremento (`++`) y decremento (`--`) solo pueden actuar sobre **variables** (contenedores de memoria), nunca sobre **literales** (valores fijos).

### 📝 EXPLICACIÓN

En Java, un número fijo como `5` es un valor inmutable; no puedes "hacer que el 5 valga 6". Lo que sí puedes hacer es cambiar lo que hay dentro de una variable.

Si intentas aplicar un incremento a un número directamente, el compilador se detiene porque no tiene un espacio de memoria donde guardar ese nuevo resultado. Para que el `++` funcione, necesita una "caja" donde sobrescribir el valor.

### ✅ EJEMPLOS Y SOLUCIONES:

- **Si quieres sumar a un número fijo:** Debes usar una variable intermedia.
    
- **En bucles:** Nunca hagas `for(int i=0; i<10; 5++)`. El incremento siempre debe ser sobre la variable de control (`i++`).
    

### ❌ ERRORES COMUNES (Fallos de escritura):

1. **Mezclar asignación y literal:** Escribir `count = 5++;`. Como Java intenta evaluar `5++` primero, el programa falla antes de poder asignar nada a `count`.
    
2. **Espacios engañosos:** Escribir `count = 5 ++;`. Aunque pongas un espacio, el problema es el mismo: el `++` está intentando "atacar" al número 5.
    
3. **Confusión con suma normal:** Creer que `5++` es lo mismo que `5 + 1`.
    
    - `5 + 1` es una operación matemática que da `6`.
        
    - `5++` es una instrucción de **modificación de memoria**, y el número 5 no tiene memoria propia que puedas modificar.