
---

> **CONCEPTO:** El Casting es el proceso de convertir una variable de un tipo de dato a otro. Es necesario porque Java, por seguridad, no permite meter "datos grandes" en "cajas pequeñas" de forma automática.

### 📝 EXPLICACIÓN

Imagina que intentas meter el contenido de una garrafa de 5 litros en una botella de 2 litros. Java te detendrá para evitar que derrames líquido (pierdas datos).

1. **Casting Implícito (Automático):** De pequeño a grande (un `int` cabe de sobra en un `double`).
    
2. **Casting Explícito (Forzado):** De grande a pequeño. Aquí tú asumes el riesgo y le dices a Java: "Sé lo que hago, corta lo que sobre".
    

### ✅ EJEMPLOS Y USOS REALES:

- **Limpiar decimales:** Cuando solo te interesa la parte entera de un cálculo (ej: cuántas monedas enteras tiene un jugador).
    
- **Compatibilidad:** Cuando una función te pide obligatoriamente un `int` pero tu dato es `double`.
    
- **Ahorro de memoria:** Convertir datos a tipos más pequeños cuando sabes que el número nunca será muy grande.
    

### ❌ ERRORES COMUNES:

- **Confundir con redondeo:** El casting `(int)` **no redondea** al número más cercano. Simplemente "trunca" (corta) los decimales. `19.99` se convierte en `19`, no en `20`.
    
- **Olvidar los paréntesis:** Escribir `int x = int precio;` dará error. El tipo de destino debe ir entre paréntesis: `(int)`.
    
- **Desbordamiento:** Si intentas forzar un número gigante en un tipo muy pequeño (ej: un `long` de millones en un `byte`), el resultado será un número sin sentido porque Java "romperá" el binario para que quepa.