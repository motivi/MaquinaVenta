
Miembros:

		Cheng Deng				G36302433
		Jesús María Gómez Moreno		75917069A
		Zhang Xiao				E02018202

Descripcion inicial de proyecto - Maquina de Venta:
===================================================

####Estructura externa(Componentes visibles):
		* Brazo movil
		* Pantalla de led informativa
		* Ranura de salida de cambio
		* Ranura de entrada de monedas
		* Ranura para la entrada de billetes
		* Escaparate de tamaño [10 filas * 5 columnas]
		* Soportes de producto 50 unidades
		* Sensores infrarrojos
		* Ranura grande de salida de producto (con puerta y tirador)

####Estructura interna:
		* Alimentador
		* Placa de control
		* Refrigerador
		* Soporte para hardware
		* Lector de tarjeta(SIM)  -- para enviar mensajes en caso de errores

####Descripción
######	Nuestro objetivo es el diseño de una máquina dispensadora de comestibles ("snacks") y bebidas de uso público. La interfaz consistirá en ranuras para la introducción del pago y una botonera para la interacción, así como una pantalla que mostrará información del producto, el estado de la operación actual (o un mensaje en caso de estar inactiva) e información adicional (fecha y hora, empresa proveedora y otros datos similares). Deberá mostrar también los productos a través de un vidrio protector (los productos estarán ordenados por filas y columnas con letreros informativos). La interfaz también incluirá una cavidad para recoger el producto a través de una pequeña puerta situada en la parte inferior, bajo el vidrio protector así como un pequeño hueco para recoger el cambio.

######	También se deberán incluir ranuras para la introducción de billetes pequeños (de 5 y 10 euros). Los billetes más grandes no deberán ser aceptados. Por otro lado, se incluye una ranura para introducir tarjetas de descuentos.

######	Los productos se encuentran en el interior sujetos por espirales metálicas y con paneles que soporten el peso. Para extraer un producto, la espiral gira, arrastrando el objeto hasta la zona en la que no hay panel. Para evitar que los productos caigan desde demasiada altura se incluirá un brazo mecánico que en cada pedido se sitúe bajo la fila adecuada. El producto cae sobre este brazo, que lo  transporta hasta la zona inferior para que pueda ser recogido.

######	Es necesario incluir refrigeración en la zona de los productos para mantener una temperatura agradable para el consumo, especialmente en las bebidas.

######	Los productos se encuentran organizados en filas y columnas, y cada producto concreto se identifica mediante la fila y la columna en la que se encuentra. Para cada uno, se utiliza una etiqueta bajo el producto que indique el identificador y el precio. Para realizar una petición, el usuario introduce las monedas necesarias e indica el identificador del producto. La máquina debe identificar las monedas y comprobar que son suficientes. En caso contrario se muestra un mensaje por la pantalla. Cuando la maquina recibe el dinero correcto extrae el producto requerido y devuelve el cambio pertinente.

######	Para obtener más información acerca de un producto (como el nombre, el precio, el identificador y las unidades restantes) se tecleará el identificador del producto en la botonera y la pantalla sobre esta mostrará lo necesario.

######	Para evitar aquellos casos en que por error un usuario introduce monedas por error o en una máquina que esté fuera de servicio, también será necesario un botón que devuelva el dinero que se acaba de introducir (esto será posible, por ejemplo, almacenando temporalmente las monedas recién introducidas en una cavidad especial hasta el momento de almacenarlas definitivamente, si se termina la transacción con éxito, o devolverlas, en caso de abortarla).

######	Para la configuración del sistema (introducción de los datos de cada producto, etc.) se dispondrá de una ranura para una tarjeta que sólo poseerán los técnicos. Se incluirá también una contraseña para acceder al menú de configuración. Este menú permitirá cambiar los precios, el nombre y otros parámetros referidos a cada identificador de producto. También permitirá abrir la máquina y retirar el vidrio protector para reparaciones. Para esta última acción también será necesaria una cerradura cuya llave sólo tenga el técnico. La cerradura sólo podrá abrirse cuando se haya habilitado mediante el menú de configuración.

######	Como forma de contabilizar el número de unidades de cada producto que se tienen, se podría implementar un sistema de sensores infrarrojos que detectase en qué posiciones hay una unidad. Así evitaríamos problemas cuando un usuario que haya introducido dinero teclee un identificador de un producto que no tenga unidades.
