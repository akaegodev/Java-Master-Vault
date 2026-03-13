### 📝 Resumen

Programa inicial para practicar la entrada de datos con `Scanner` y operaciones aritméticas simples. Calcula sueldo bruto, impuestos fijos (15%) y sueldo neto.

---

**CÓDIGO USADO**
```java
import java.util.Scanner;  
public class Main {  
    public static void main(String[] args) {  
  
        //Creamos el Scanner para leer los datos del teclado (input)  
        Scanner teclado = new Scanner(System. in);  
  
        //Pedimos los datos al usuario  
        System.out.println("--- Calculadora de Sueldo ---");  
        System.out.print("Introduce las horas trabajadas:");  
        double horas = teclado.nextDouble();  
  
        System.out.print("Introduce el pago por hora:");  
        double pagoPorHora = teclado.nextDouble();  
  
        //Realizamos los cálculos  
        double sueldoBruto = horas * pagoPorHora;  
        double impuestos = sueldoBruto * 0.15; //Suponemos que de impuestos tenemos 15%  
        double sueldoNeto = sueldoBruto - impuestos;  
  
        //Mostramos los resultados en pantalla  
        System.out.println("\n--- RESULTADOS ---");  
        System.out.println("Sueldo Bruto: €" + sueldoBruto);  
        System.out.println("Retención de impuestos (15%): €" + impuestos);  
        System.out.println("Sueldo Neto: €" + sueldoNeto);  
  
        //Cerramos el Scanner  
        teclado.close();

```

---

**RESULTADOS DEL CODIGO**

![[Resultado.png]]

---
### 🧠 Conceptos Clave

- **`Scanner`**: Obligatorio importar `java.util.Scanner`.
    
- **`System.in`**: Es la entrada del teclado.
    
- **Concatenación**: Usar `+` para mezclar texto y variables. 

---
### ❌ Errores Solucionados

- Intenté usar `System.some` por error. Recordar que es `System.in`