# Admin-Proy1 
La cadena Automercados Plaza ha decidido abrir dos nuevas sucursales en Caracas con un concepto
revolucionario. La tienda estará dotada con tecnología de IoT para que los clientes puedan hacer sus
compras sin la necesidad de la interacción humana. La logística de la tienda funciona de la siguiente
manera:
 Los productos de las tiendas cuentan con una categoría (Enlatados, No Perecederos, Frescos,
etc) y con un costo que puede ser variable en el tiempo. Las dos tiendan pueden no tener los
mismos productos.
 Cuando una persona entra a una de las tiendas una cámara toma una imagen de su rostro. Si la
persona pertenece al programa de fidelidad, se le reconocerá el rostro y se contará su visita. De
no pertenecer al programa solo se contará la visita de una persona desconocida.
 La persona comienza a realizar su compra en la tienda, escogiendo los productos que desea
comprar de los estantes inteligentes. Estos estantes tienen la capacidad de medir cuanto
producto hay disponible y enviar una alerta cuando queda menos del 20% de lo que está
capacitado para tener. Al enviar la alerta unos empleados llenan el estante con producto del
almacén.
 Al terminar la compra, el cliente va a las máquinas de venta, donde el mismo escanea todos los
productos y paga. De ser un cliente que pertenece al programa de fidelidad se le asigna a su
cuenta una cantidad de puntos equivalente al 10% del monto de su compra en Bs.
 El cliente puede pagar por transferencia a cualquiera de estos 3 bancos: Mercantil, Banesco,
Provincial
 Cada tienda tiene por diseño un número máximo de personas que pueden comprar al mismo
tiempo.
 Cada equipo debe agregarle otra funcionalidad al sistema avanzado de la tienda, que tenga su
basamento en la teoría del IoT.
Usted debe presentar el modelo lógico ER y el modelo físico para ser evaluado. Además, debe
implementar este sistema en el manejador de Bases de datos PostgreSQL llenando las relaciones con
información de prueba para poder hacer las consultas.
Consultas que debe tener:
 Cuales son los clientes conocidos y desconocidos que mas han comprado en cada una de las
tiendas.
 Diga cual es la categoría de producto que menos se ha vendido en cada una de las tiendas.
 Cuales es el top 5 de productos que mas se han vendido en cada una de las tiendas.
 Diga todos los clientes que en los últimos 7 días a partir de la ejecución del query han comprado
solo en una tienda y los que han comprado en las dos tiendas (realice queries distintos).
 Haga un análisis por estante de cuales categorías de producto tienen mayor rotación de
inventario y haga una propuesta de modificación
 Encuentre a todos los clientes que han pagado con 2 bancos distintos en la ultima semana.
Enumérelos y diga si son parte del programa de afiliados.

Funciones que debe tener:
 Realizar compra: Esta función debe tener como parámetro una lista de productos con su
cantidad, el banco por donde se va a cancelar y un cliente. Debe tener toda la lógica para
ingresar en las distintas tablas la compra realizada.
 Haga una función que al final del día saque un estado de cuenta de cuanto dinero se tiene en
cada banco
 Haga una función que al final del mes saque un estado de cuenta de los puntos de todos los
afiliados al programa de fidelidad que compraron ese mes.
Triggers que debe tener:
 Cada vez que entre un cliente conocido, se debe agregar 1 punto a su estado de cuenta del
programa de fidelidad.
 Cada vez que un cliente conocido realice una compra, se le agregaran los puntos en su programa
de fidelidad
 Si un cliente desconocido con la misma cedula compra mas de 4 veces, automáticamente se
agregará al programa de fidelidad.
 Todos los demás Triggers necesarios para realizar la solución. (Debe enumerarlos y explicarlos)
Análisis que debe tener:
 ¿Cuáles son las categorías de producto que se venden mejor en cada una de las tiendas? Use un
pivot table para razonar su respuesta.
 ¿Qué banco, categoría de producto y tienda prefieren los clientes de nuestro programa de
afiliados? Razone su respuesta.
 ¿Qué horas del día son más rentable para cada una de las tiendas? Razone su respuesta.
 ¿Es posible ver la cantidad de mercancía que había por hora en uno de los estantes de una de
las tiendas en el día anterior?
