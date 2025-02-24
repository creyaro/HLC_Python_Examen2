## **Python - Examen 2 [Tipo A]**  
 
Los alumnos que realizarán este examen son Laura, Alejandro E., Cristóbal, María José, Triana, David Mart., David Mor., Alejandro Paz, Andrés, Adrián, Daniel JdlC, Ayman, José Antonio, Manuel, Eduardo e Ismael.

>**Nota**: En todos los ejercicios hay que entregar la programación de los métodos y la llamada a los mismos. Esto incluye la instanciación de las clases. Para los ejercicios 1-10, se pueden realizar todas las llamadas juntas al final.

---
**Ejercicio 1 (1.25pto)**: Crea una clase llamada `Tienda` que tenga una propiedad ``catálogo`` donde almacene los productos a la venta y sus precios. Los productos se identifican de manera única por su nombre. Es decir, no puede haber dos productos con el mismo nombre.

**Ejercicio 2 (1pto)**: Agrega a la clase `Tienda` un método llamado `agregar_producto` que reciba el nombre de un producto y su precio y lo añada al catálogo. Si el producto ya existe, entonces únicamente actualizará su precio, en cuyo caso debe mostrarse un mensaje indicándolo. El formato de dicho mensaje debe ser `El precio del producto [nombre] ha sido actualizado de [precio_antiguo] a [precio_nuevo]`.
 
**Ejercicio 3 (0.5pto)**: Agrega un método `eliminar_producto` que reciba el nombre de un producto y lo elimine si existe. Si no existe, debe mostrar un mensaje indicándolo. El formato de dicho mensaje debe ser `El producto [nombre] no existe.`

**Ejercicio 4 (0.5pto)**: Agrega un método `consultar_precio` que reciba el nombre de un producto y devuelva su precio si existe. Si no existe, debe mostrar un mensaje indicándolo. El formato de dicho mensaje debe ser `El producto [nombre] no existe.`

**Ejercicio 5 (1.75ptos)**: Crea una clase `TiendaOnline` que herede de `Tienda` y agregue dos atributos: `precio_envio` (que por defecto valga 3) y `carrito`, donde se almacenen los productos que ha seleccionado el usuario. Además, debe modificar el método `agregar_producto`, de forma que cuando se almacena un nuevo producto a través de la tienda online, al precio base del mismo (en el catálogo, no en el carrito) se sume un 5% extra por gastos de logística.

**Ejercicio 6 (0.5pto)**: Agrega un método `modificar_precio_envio` en `TiendaOnline` que reciba un nuevo precio del envío y lo actualice.

**Ejercicio 7 (1.5pto)**: Crea un método `agregar_al_carrito` en `TiendaOnline` que reciba una lista de productos y los añada al carrito del usuario. Ya que el usuario puede seleccionar más de una unidad, también debe almacenarse la cantidad de cada producto. Para que un producto exista en el carrito debe tener una cantidad mínima de 1.

**Ejercicio 8 (1.5pto)**: Crea un método `eliminar_del_carrito` en `TiendaOnline` que reciba una lista de productos y los elimine del carrito del usuario. Al igual que en el método `agregar_al_carrito`, también debería indicarse la cantidad. Si la cantidad llega a 0, el producto se elimina del carrito.

**Ejercicio 9 (1.5pto)**: Crea un método `calcular_total` en `TiendaOnline` que calcule el precio total de los productos que el usuario tiene en el carrito, además del `precio_envio`.

**Ejercicio Extra (1pto)**: Crea un método que ordene una lista de palabras de menor a mayor longitud mediante el algoritmo BubbleSort.
