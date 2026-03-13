
**CÓDIGO USADO**
```java
import java.util.Scanner;  
public class Main {  
    public static void main(String[] args) {  
  
        //Creamos el Scanner para leer los datos del teclado (input)  
        Scanner teclado = new Scanner(System. in);  
        System.out.println("Introduce el total de la cuenta");  
        double cuentaBase= teclado.nextDouble();  
  
        System.out.println("¿Cuántas personas sois?");  
        int personas = teclado.nextInt();  
  
        System.out.println("¿Qué % de propina queréis dejar?");  
        double porcentajePropina = teclado.nextDouble();  
  
        double iva = cuentaBase * 0.21;  
  
        double totalConIva = cuentaBase + iva;  
        double dineroPropina = totalConIva * (porcentajePropina / 100);  
        double granTotal = totalConIva + dineroPropina;  
        double pagoPorPersona = granTotal / personas;  
  
        System.out.println("--- RESULTADOS ---");  
        System.out.println("IVA: " + iva);  
        System.out.println("Total con IVA:" + totalConIva);  
        System.out.println("Propina:" + dineroPropina);  
        System.out.println("Multa aka dolorosa:" + granTotal);  
        System.out.println("Cada uno tiene que pagar:" + pagoPorPersona);

```

---

***RESULTADOS DEL CÓDIGO
![[Resultado 2.png]]


---

### 🔑 Conceptos Clave
#### 1. Tipos de Datos (Double vs Int)

- Usa `double` siempre que haya dinero o decimales.
    
- **Cuidado:** `double` no es exacto para finanzas por la forma en que el binario maneja decimales (produce "basura" al final como `12.300000004`). Para cosas reales se usa `BigDecimal`, pero para aprender, `double` cumple.
    

#### 2. Precedencia de Operadores (PEMDAS)

- Java siempre multiplica y divide antes de sumar.
    
- Usa paréntesis `()` para forzar el orden. Ejemplo: `(porcentaje / 100)` asegura que primero obtengas el decimal del porcentaje.
    

#### 3. El Flujo de Datos

1. **Entrada:** `Scanner` (siempre cerrarlo al final).
    
2. **Proceso:** - Base -> IVA -> Total con IVA.
    
    - Total con IVA -> Propina -> Total Final.
        
    - Total Final / Comensales -> Cuota individual.
        
3. **Salida:** `System.out.println`
