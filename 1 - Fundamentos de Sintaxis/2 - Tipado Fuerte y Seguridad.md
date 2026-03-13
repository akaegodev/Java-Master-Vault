
---

> **CONCEPTO:** Java es un lenguaje de **tipado estático y fuerte**. Cada variable tiene un tipo definido que determina cuánta memoria ocupa y qué operaciones puede realizar.

### 📝 EXPLICACIÓN

No todos los datos pesan lo mismo ni sirven para lo mismo. Java separa los datos en dos grandes grupos: **Primitivos** (simples y rápidos) y **Referencia** (complejos y con métodos).

El sistema de tipado es el "muro de seguridad" de Java: evita que intentes sumar una palabra a un número o que pierdas precisión decimal sin darte cuenta.

### ✅ EJEMPLOS Y USOS REALES:

- **¿Cuándo usar `int`?** Para todo lo que se pueda contar por unidades: munición, enemigos, días del mes, edad.
    
- **¿Cuándo usar `double`?** Para medidas físicas o dinero: temperatura (24.5), estatura (1.80), precio con IVA.
    
- **¿Cuándo usar `boolean`?** Para estados del juego o la app: `isPaused`, `hasKey`, `isGameOver`.
    
- **¿Cuándo usar `String`?** Para cualquier dato que sea puramente información visual: nombres de usuario, contraseñas, direcciones.
    

### ❌ ERRORES COMUNES (Los que te harán fallar):

1. **Pérdida de Precisión:** Intentar meter un `10.9` en un `int`. Java no redondea a 11, ni a 10; simplemente **lanza un error** y no te deja compilar porque el `.9` no cabe en el cajón de los enteros.
    
2. **Confusión de Comillas:** * `char c = "A";` -> **ERROR** (Las dobles son para String).
    
    - `String s = 'Hola';` -> **ERROR** (Las simples son solo para un carácter).
        
3. **Números en Strings:** `String edad = "25";`. Aunque veas un número, Java ve un dibujo. **No puedes hacer** `edad + 1` para que de 26; el sistema daría un error o lo pegaría como texto ("251").
    
4. **El error de la coma:** `double n = 10,5;`. Java usa el estándar internacional. La coma se usa para separar variables, el punto para los decimales.