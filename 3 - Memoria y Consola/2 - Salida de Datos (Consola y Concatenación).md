
---

> **CONCEPTO:** La consola es la interfaz básica. Para que la información sea útil, debemos aprender a **concatenar** (unir) variables con texto explicativo.

### 📝 EXPLICACIÓN

Soltar un número solo en la pantalla no sirve de nada. El usuario necesita contexto. Java utiliza el operador `+` no solo para sumar números, sino para **pegar** piezas de información como si fueran imanes.

Dominar la diferencia entre `print` y `println` es lo que hace que un programa parezca profesional y no un montón de números desordenados.

### ✅ EJEMPLOS Y USOS REALES:

- **`print`**: Se usa para crear barras de progreso (`[### ]`) o prompts de escritura.
    
- **`println`**: Para cada línea de un menú o mensajes de confirmación.
    

### ❌ ERRORES COMUNES:

- **La trampa de la suma:** Si haces `System.out.println("Resultado: " + 5 + 5);`, Java escribirá **"Resultado: 55"** porque al ver texto, trata todo como texto. Tienes que usar paréntesis: `("Resultado: " + (5 + 5))`.
    
- **Mayúsculas en System:** Es el error número 1 de los principiantes. La **S** siempre es mayúscula.
    
- **Espacios olvidados:** Escribir `"Nivel:"+nivel` -> Resultado: `Nivel:5`. Siempre añade un espacio dentro de las comillas para que respire: `"Nivel: "`.