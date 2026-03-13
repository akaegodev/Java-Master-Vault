
---

> **CONCEPTO:** Los tipos primitivos en Java se almacenan en el **Stack** (pila). Cuando asignas una variable a otra, Java duplica el valor físico, creando dos entidades totalmente desconectadas.

### 📝 EXPLICACIÓN

Imagina que cada variable es un papel donde escribes un número. Si haces `int b = a;`, estás cogiendo un papel nuevo y copiando el número que ves en el primero. Si luego borras y cambias el número del primer papel, el segundo sigue teniendo el número viejo.

En Java, esto se llama **paso por valor**. El sistema no recuerda de dónde vino el dato, solo le importa el dato en sí.

### ✅ EJEMPLOS Y USOS REALES:

- **Reset de estados:** Guardar la `posicionInicial` de un personaje para poder devolverlo ahí si muere.
    
- **Cálculos complejos:** Usar una copia del valor para probar fórmulas sin alterar el dato real que se muestra en pantalla.
    

### ❌ ERRORES COMUNES:

- **Pensar en "punteros":** Creer que `b` apunta a `a`. En Java, los primitivos **no apuntan a nada**, son el valor en sí mismos.
    
- **Actualización en cadena:** Intentar cambiar 10 variables cambiando solo la "madre". Tendrás que actualizarlas una a una.