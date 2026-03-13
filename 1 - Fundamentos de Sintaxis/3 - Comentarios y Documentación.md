
---

> **CONCEPTO:** Anotaciones en el código que el compilador de Java ignora por completo. Su función es explicar el "porqué" de las cosas a otros humanos (o a ti mismo en el futuro).

### 📝 EXPLICACIÓN

El código dice **cómo** se hace algo, pero los comentarios dicen **por qué** se hizo así. En Java existen tres tipos de comentarios según su alcance y función:

1. **Línea única:** Para explicaciones breves.
    
2. **Bloque o Multilínea:** Para explicaciones extensas o anular trozos de código temporalmente.
    
3. **JavaDoc:** Para generar documentación técnica automática (usado en empresas).
    

### ✅ EJEMPLOS Y USOS REALES:

- **Explicar lógica compleja:** "Calculamos el IVA aquí porque la ley cambió en 2024".
    
- **Marcar tareas pendientes:** `// TODO: Revisar por qué el jugador no salta`.
    
- **Desactivar código:** Si quieres probar una función sin borrar otra, la comentas para que no se ejecute.
    

### ❌ ERRORES COMUNES:

- **Comentar lo obvio:** `int x = 5; // Declaramos x igual a 5`. Esto ensucia el código.
    
- **Comentarios desactualizados:** Cambiar el código pero olvidar cambiar el comentario. Es peor que no tener nada.
    
- **Olvidar cerrar el bloque:** Abrir un `/*` y no poner el `*/`. Java creerá que **todo** el resto de tu programa es un comentario y no ejecutará nada.