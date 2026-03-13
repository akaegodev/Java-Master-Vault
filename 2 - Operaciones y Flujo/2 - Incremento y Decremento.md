
---

> **CONCEPTO:** Operadores unarios que sirven para sumar o restar exactamente **1** a una variable. Su posición (antes o después de la variable) determina el orden de ejecución.

### 📝 EXPLICACIÓN

Aunque parezcan simples, estos operadores son una de las mayores fuentes de errores. La clave no es la matemática, sino la **prioridad**:

1. **Pre-incremento/decremento (`++x`, `--x`):** "Cambia el valor **ya mismo** y luego úsame". Es la opción más rápida y directa.
    
2. **Post-incremento/decremento (`x++`, `x--`):** "Úsame con mi valor actual y, cuando termine la instrucción (al llegar al `;`), cámbiame".

### ✅ EJEMPLOS Y USOS REALES:

- **`puntos++;`**: Ideal para subir el marcador tras una acción.
    
- **`balas--;`**: Perfecto para descontar munición tras un disparo.
    
- **Uso en cálculos:** `int total = ++puntos * 2;` (Primero sube puntos, luego multiplica).
    

### ❌ ERRORES COMUNES (Los que te harán fallar):

1. **El "Espejismo" del Post-incremento:** Creer que `System.out.println(x++)` va a mostrar el número ya sumado. **No**, mostrará el valor viejo. El "+" está "detrás", así que la suma va "detrás".
    
2. **Operaciones combinadas:** Mezclar `x++` con otras cuentas en la misma línea. Java lee de izquierda a derecha; si el incremento es "post", usará el valor antiguo para toda la operación de esa línea.
    
3. **Confusión de dirección:** Usar `++` cuando quieres bajar el valor de una variable (decremento). Parece obvio, pero en códigos largos es un error típico de despiste.
    
4. **Olvidar el `;`**: Como estos operadores suelen ir en líneas sueltas, es muy común olvidar cerrar la instrucción.