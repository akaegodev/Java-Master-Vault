
---


> **CONCEPTO:** Reservar un espacio en la memoria (caja) y darle un valor.

### 📝 EXPLICACIÓN

En Java, no puedes usar una variable si no la has presentado primero. Es un proceso de tres pasos:

1. **Declaración:** Eliges el tipo y el nombre (creas la caja).
    
2. **Inicialización:** Le das el primer valor (metes algo en la caja).
    
3. **Reasignación:** Cambias el valor por uno nuevo (tiras lo viejo, metes lo nuevo).
    
### ✅ EJEMPLOS:

- **Enteros (`int`):** `int edad = 25;` o `int balas = 30;`
    
- **Decimales (`double`):** `double altura = 1.75;`
    
- **Texto (`String`):** `String mensaje = "Nivel Completado";`
    
- **Lógicos (`boolean`):** `boolean partidaGuardada = false;`

### ❌ ERRORES COMUNES:

- **Olvidar los Enteros:** Intentar guardar un número entero en un String o viceversa.
    
- **Caja vacía:** Intentar hacer `System.out.print(puntos);` justo después de la declaración sin haberle dado un valor (inicialización).
    
- **Duplicidad:** Poner `int puntos = 10;` y luego `int puntos = 20;`. Java dirá que la variable ya está definida. Lo correcto es `puntos = 20;` sin el `int`.