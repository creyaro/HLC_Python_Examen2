## **Python - Examen 2 [Tipo B]**  
 
Los alumnos que realizarán este examen son Jesús, Helena, Marcos, Oliver, Carmen, Valeria, Saúl, Álvaro, Daniel JR, Marc y Santiago. 

>**Nota**: En todos los ejercicios hay que entregar la programación de los métodos y la llamada a los mismos. Esto incluye la inicialización de las clases. Para los ejercicios 1-6, se pueden realizar todas las llamadas juntas al final.

---
**Ejercicio 1 (1.5pto)**: Crea una clase llamada `Personaje` que tenga las siguientes propiedades:
- `nombre`: Almacena el nombre del personaje. Cada personaje debe tener un nombre único, por lo que no pueden existir dos personajes con el mismo nombre.
- `vida`: Representa la cantidad de vida del personaje mediante un número entero. Su valor mínimo es 0, y su valor inicial por defecto debe ser 500.

**Ejercicio 2 (1.75ptos)**: Crea una clase `Héroe` que herede de `Personaje` y agregue dos atributos: `poder` (que por defecto valga 50) y `defensa` (que por defecto valga 20). 
 
**Ejercicio 3 (1pto)**: Crea una clase `Enemigo` que herede de `Personaje` y agregue dos atributos: `peligrosidad` (que por defecto valga 3) y `tipo`, que almacene el tipo de enemigo (por ejemplo, "Orco", "Dragón", "Esqueleto").

**Ejercicio 4 (2.25ptos)**: Crea un método `atacar_enemigo` en `Héroe` que reciba un objeto de tipo `Enemigo` como parámetro y le cause daño igual al valor de `poder`. Si la vida del enemigo llega a 0, debe imprimirse un mensaje indicando que ha sido derrotado. El formato del mensaje debe ser `El enemigo [nombre] de tipo [tipo] ha sido derrotado.` Hay que tener en cuenta que si el héroe fue derrotado (es decir, su vida vale 0), no podrá atacar, en cuyo caso debe mostrarse un mensaje indicándolo. Dicho mensaje debe tener el formato `El héroe [nombre] no puede atacar porque ha sido derrotado`.

**Ejercicio 5 (1pto)**: Crea un método `atacar_heroe` en `Enemigo` que reciba un objeto de tipo `Héroe` como parámetro y le cause daño igual al valor de `peligrosidad` multiplicado por 10. La cantidad de daño que recibe el héroe debe reducirse según el valor de `defensa` antes de restarse a la vida. Es decir, si recibe 30 de ataque pero tiene 20 de defensa, entonces solo recibirá 10 de daño. Si la vida llega a 0, debe imprimirse un mensaje indicando que el personaje ha sido derrotado. El formato del mensaje debe ser `El héroe [nombre] ha sido derrotado.` Hay que tener en cuenta que si el enemigo fue derrotado (es decir, su vida vale 0), no podrá atacar, en cuyo caso debe mostrarse un mensaje indicándolo. Dicho mensaje debe tener el formato `El enemigo [nombre] de tipo [tipo] no puede atacar porque ha sido derrotado`

**Ejercicio 6 (2.5pto)**: Crea un método `luchar` en `Héroe` que reciba un objeto de tipo `Enemigo` y un parámetro `num_combates`. Este método realizará tantos combates como indique `num_combates`. En cada combate se ejecutará primero el método `atacar_enemigo` y después `atacar_heroe`. Cuando los combates acaban, el método debe imprimir un mensaje que diga `El personaje [nombre_personaje_ganador] ha derrotado a [nombre_personaje_perdedor]` si uno de los dos ha sido derrotado, o el mensaje `Los dos personajes han quedado en empate` si ninguno ha sido derrotado (en cuyo caso, se considera empate). Si un personaje es derrotado antes de que acaben los combates, la lucha se interrumpe y no se siguen ejecutando los que quedaban.

**Ejercicio Extra (1pto)**: Crea un método que ordene una lista de números de mayor a menor mediante el algoritmo BubbleSort.