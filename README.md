# Guía de uso de Stock

Esta guía explica **cómo usar el programa en el día a día**. No hace falta saber de computación. Si sos quien instala o prepara el programa, mirá el `README.md`.

---

## 1. Para empezar

### Abrir el programa
Hacé doble clic en el icono de **Stock**. Lo primero que aparece es una pantalla con dos opciones:

| Opción | Cuándo usarla |
|---|---|
| **Host** | En la **PC principal** del negocio, la que guarda toda la información. Debe estar encendida y con el programa abierto para que las demás funcionen. |
| **Usuario** | En **cualquier otra PC** que se conecta a la principal. |

Si elegís **Usuario**, escribí la **IP** y el **puerto** que te dio el administrador (por ejemplo `192.168.0.10` y `8080`) y tocá **Conectar**. También podés tocar **Buscar hosts en la red** y elegir el que aparezca. Después de la primera vez, el programa recuerda la dirección.

Con **Cambiar modo** (abajo a la izquierda, en el menú) volvés a esta pantalla.

### Iniciar sesión
Escribí tu **usuario** y tu **contraseña**.
- La primera vez que se usa el programa, el administrador entra con el usuario `admin` y la contraseña `admin1234`. **Hay que cambiarla enseguida.**
- Si no tenés usuario, pedíselo al administrador.

### Cambiar tu contraseña
Botón **Cambiar clave** (abajo a la izquierda, en el menú). Pide la contraseña actual y la nueva, de al menos 6 caracteres.

### Cambiar el tema de colores
Botón **Tema** (abajo a la izquierda): alterna entre **Automático** (como tenga Windows), **Claro** y **Oscuro**. Se guarda en tu cuenta: lo vas a ver igual desde cualquier PC.

### Salir
Botón **Salir**. Conviene hacerlo al terminar el turno, para que nadie use tu cuenta.

---

## 2. Qué ves según tu rol

Cada persona tiene un rol y ve solo lo que le corresponde:

| Rol | Qué puede hacer |
|---|---|
| **Vendedor** | Ver los productos (sin costos), vender y ver sus propias ventas. |
| **Encargado** | Todo lo del vendedor, más: crear y editar productos, ajustar el stock, hacer compras, devoluciones y anulaciones, ver ventas de todos, caja, resumen, reportes e importar. |
| **Administrador** | Todo lo del encargado, más: usuarios, datos del negocio, respaldos, red y auditoría. |

Si no ves una pestaña que mencionan en esta guía, es porque tu rol no la incluye.

---

## 3. Para todos: ver productos y vender

### Ver los productos
La pestaña **Productos** muestra todo lo que hay.
- El botón de arriba cambia entre **Iconos** (tarjetas con foto) y **Lista** (tabla).
- Para buscar, escribí en el cuadro de búsqueda parte del **nombre** o del **código**.
- Podés filtrar por **categoría**.
- Cada producto tiene una etiqueta:
  - **En stock**: hay suficiente.
  - **Stock bajo**: queda poco (llegó al mínimo).
  - **Agotado**: no quedan unidades.

### Registrar una venta, paso a paso

1. En **Productos**, tocá **+ Vender** en cada producto que lleva el cliente. Tocalo de nuevo para sumar otra unidad. *(Con un lector de códigos de barras, mirá más abajo.)*
2. Entrá a la pestaña **Venta**. El número entre paréntesis te dice cuántos productos sumaste.
3. Revisá la lista. Podés **cambiar la cantidad** de cada producto o tocar **Quitar**.
4. Si hay descuento o recargo, escribilo en **porcentaje**: con **signo menos** para descontar (por ejemplo `-10`) y positivo para recargar (por ejemplo `5`).
5. Elegí **cómo paga el cliente** (efectivo, transferencia o tarjeta) y el monto.
6. Tocá **Confirmar venta**.

Al confirmar, el stock se descuenta solo y se abre el detalle de la venta. Ahí podés tocar **Ver ticket** para verlo antes de imprimir, o **Imprimir** para sacarlo directamente. Si el administrador activó la opción, el ticket se imprime solo al confirmar cada venta.

> Si algún producto ya no alcanza, el programa no registra nada y te avisa cuál falta. Corregí la cantidad y confirmá de nuevo.

### Vender con el lector de códigos de barras
En la pestaña **Venta** hay un campo para escanear. Apuntá el cursor ahí, pasá el producto por el lector y se suma solo. También funciona en el buscador de **Productos**: al escanear y presionar Enter, el producto se agrega a la venta. Si el código no existe, aparece un aviso.

### Cuando el cliente paga con dos medios
En la venta tocá **+ Otro medio de pago**. Por ejemplo, `$ 5.000` en efectivo y el resto con tarjeta. El programa muestra cuánto va pagado y cuánto falta.

### Cuando el cliente deja una seña
Si el monto pagado es **menor al total**, la venta se registra igual y queda con **saldo pendiente**. El programa lo avisa en pantalla antes de confirmar. Los productos quedan descontados del stock.

Para **cobrar el resto más adelante**:
1. Entrá a **Ventas** (o **Mis ventas**) y buscá la venta. Las que tienen saldo muestran una etiqueta **Saldo**.
2. Tocá **Ver**, y después **Cobrar saldo**.
3. Elegí el medio de pago, confirmá el monto y tocá **Registrar cobro**.

### Ver tus ventas
La pestaña **Mis ventas** (o **Ventas**, si sos encargado o administrador) lista las ventas.
- Podés filtrar por **fecha** y por **medio de pago**.
- Tocá **Ver** para abrir el detalle: productos, pagos, saldo y devoluciones.

---

## 4. Para encargados y administradores

### Crear un producto
1. En **Productos**, tocá **Nuevo producto**.
2. Completá el **nombre** (es lo único obligatorio), el **código** (el del código de barras, si tiene), la **categoría**, el **costo**, el **precio de venta**, el **stock inicial** y el **stock mínimo**. Podés agregar una **foto**.
3. Tocá **Guardar**.

> El **stock mínimo** es la cantidad a partir de la cual el programa avisa que hay que reponer.

### Editar o eliminar un producto
Tocá **Editar** en el producto. Ahí cambiás sus datos o lo eliminás con **Eliminar** (el programa pide confirmación). El stock **no** se cambia desde esta pantalla, sino con el ajuste.

### Ajustar el stock
Tocá **Ajustar stock** en el producto, escribí la cantidad y el **motivo**:
- Número positivo para **sumar** (por ejemplo `10`).
- Número negativo para **restar** (por ejemplo `-3`).
- Motivos habituales: compra, merma, corrección. Queda anotado en el historial.

### Registrar una compra a un proveedor
Cuando llega mercadería:
1. Pestaña **Compras** → **Nueva compra**.
2. Escribí el **proveedor** (el programa sugiere los que ya usaste).
3. Elegí cada producto, la **cantidad** y el **costo unitario**. Con **+ Agregar producto** sumás más líneas.
4. Tocá **Registrar compra**.

El stock sube solo, y el **costo** de cada producto se actualiza con el de esta compra. Así las ganancias se calculan con costos al día.

### Saber qué hay que reponer
La pestaña **Reposición** lista los productos en el mínimo o agotados, con una **cantidad sugerida** para comprar (el doble del mínimo, menos lo que ya hay). El botón **Armar compra con estos productos** abre una compra ya cargada. Cuando entrás al programa, te avisa si hay productos para reponer.

### Corregir una venta: devolver o anular
Abrí la venta (**Ventas** → **Ver**):
- **Devolver:** para cuando el cliente devuelve **solo algunos productos**. Tocá **Devolver** en el producto, indicá la cantidad, en qué medio se le devuelve el dinero y el **motivo**. El stock se repone y el total de la venta baja.
- **Anular venta:** cancela la venta **completa**. Pide el motivo, repone todo el stock y queda registrada quién la anuló. Una venta anulada no se puede revertir.

### Hacer el cierre de caja
1. Pestaña **Caja**.
2. Elegí el **día** (por defecto es hoy).
3. Ahí ves cuánto se cobró en total, **por medio de pago** y **por vendedor**, y cuántas ventas y anulaciones hubo.

El dinero se cuenta **el día en que se cobró**: si cobrás hoy el saldo de una venta de la semana pasada, aparece en la caja de hoy. Las devoluciones de dinero restan.

### Ver cómo va el negocio
- **Resumen:** ventas y ganancia de hoy, de los últimos 7 días y del mes, un gráfico de los últimos 14 días, los productos más vendidos y los que tienen poco stock.
- **Reportes:** elegí el tipo (ventas con ganancia, productos más vendidos, ventas por día o productos sin movimiento) y las fechas. El botón **Exportar a CSV / Excel** lo guarda para abrirlo en Excel.
- **Movimientos:** historial de cada entrada y salida de stock, con fecha, producto, cantidad y motivo.

### Cargar muchos productos de una vez
Pestaña **Importar y precios**:
1. Tocá **Descargar plantilla** y completala en Excel con tus productos. Las columnas son: Código, Nombre, Categoría, Precio, Costo, Stock y Stock mínimo. Solo el nombre es obligatorio.
2. Guardala como `.xlsx` o `.csv`, elegí el archivo y tocá **Importar**.
3. El programa informa cuántos productos **creó** y cuántos **actualizó**. Si un código ya existe, **actualiza ese producto** (y el stock del archivo reemplaza al actual).

Si alguna fila tiene un error, te dice cuál. Las demás se cargan igual.

### Cambiar precios de muchos productos
En la misma pestaña, **Cambio masivo de precios**: escribí un **porcentaje** (negativo para bajar), elegí si se aplica al **precio de venta**, al **costo** o a **ambos**, y si es para **todos** los productos o solo una **categoría**. El programa pide confirmación antes de aplicarlo.

---

## 5. Solo para administradores

### Usuarios
Pestaña **Usuarios**:
- **Nuevo usuario:** nombre, contraseña (mínimo 6 caracteres) y rol.
- Para cambiar el **rol**, usá el selector en la fila de la persona.
- **Nueva clave:** si alguien olvidó la suya.
- **Bloquear / Activar:** impide o permite que entre sin borrar su historial.
- **Eliminar:** borra la cuenta.

No podés bloquear, eliminar ni cambiar el rol de tu propia cuenta. Cuando cambiás algo de otra persona, esa persona debe volver a iniciar sesión.

### Datos del negocio
Pestaña **Negocio**: **nombre**, **logo**, **símbolo de moneda**, **dirección**, **teléfono** y una **nota** para el pie del ticket (por ejemplo "Gracias por su compra"). También elegís el **ancho del papel** (80 mm, el más común, o 58 mm) y si el ticket se imprime solo al confirmar cada venta. El nombre y el logo aparecen en el programa y en los tickets.

### Respaldos (copias de seguridad)
En **Negocio**:
- Elegí cada cuánto se hace una copia automática (cada 6 o 12 horas, todos los días o cada 2 días) y cuántas copias guardar. Las copias se hacen **mientras el programa esté abierto en la PC principal**.
- **Hacer un respaldo ahora** crea una copia al instante.
- **Restaurar** vuelve a una copia anterior. Solo se puede hacer desde la PC principal. Antes de restaurar, el programa guarda una copia de lo que hay, por seguridad. Después de restaurar, todos deben volver a iniciar sesión.
- El botón **Descargar respaldo** (arriba a la derecha, en esta misma pestaña) descarga una copia para guardarla en un pendrive o en la nube.

> Una buena costumbre: copiar de vez en cuando la carpeta de respaldos a un pendrive.

### Permitir que otras PC se conecten
En la **PC principal**, pestaña **Red**:
1. En **Quién puede conectarse**, elegí **Toda la red local**.
2. Anotá la **IP y el puerto** que aparecen en "Los usuarios se conectan a". Esos datos son los que se escriben en las otras PC.
3. Tocá **Abrir en el firewall** y aceptá el permiso que pide Windows. Solo hace falta la primera vez.
4. Si querés limitar el acceso, escribí en **IP permitidas** las direcciones de las PC autorizadas, separadas por espacios. Si lo dejás vacío, puede entrar cualquier equipo de la red.
5. Tocá **Aplicar cambios**.

Más abajo ves quién está **conectado** en este momento. Si cambiás el puerto, las otras PC tienen que volver a conectarse con el nuevo.

> Consejo: pedile a quien administra tu red que reserve una IP fija para la PC principal. Así la dirección no cambia al reiniciar.

### Auditoría
Pestaña **Auditoría**: lista de lo que hizo cada persona (ventas, cambios de productos y de precios, anulaciones, cambios de usuarios, ingresos y también los intentos de ingreso fallidos). Sirve para saber quién cambió qué y cuándo.

---

## 6. Rutina recomendada

**Al abrir el negocio**
- Abrí el programa en la PC principal (Host) y revisá la pestaña **Reposición** o el aviso de productos por reponer.

**Durante el día**
- Cada venta, en la pestaña **Venta**.
- Cuando llega mercadería, **Compras** (así el stock y los costos quedan al día).

**Al cerrar**
- Mirá la **Caja** del día y compará con el dinero real.
- Cerrá sesión (**Salir**).

**Cada semana o cada mes**
- Revisá **Resumen** y **Reportes** (más vendidos, sin movimiento, ganancias).
- Copiá la carpeta de respaldos a un lugar seguro.

---

## 7. Preguntas frecuentes

**Me equivoqué al registrar una venta. ¿Qué hago?**
Si el error fue en **algunos productos**, usá **Devolver**. Si fue en **toda la venta**, **Anulá** la venta y hacé una nueva. Las dos opciones requieren rol de encargado o administrador: si sos vendedor, pedile ayuda a uno.

**Me aparece "No hay stock suficiente".**
Alguien vendió ese producto antes que vos, o el stock cargado no coincide con la realidad. Un encargado puede corregirlo con **Ajustar stock**.

**No veo una pestaña o un botón que mencionan.**
Depende de tu rol (sección 2).

**Un producto muestra toda la venta como ganancia.**
Tiene el **costo en 0**. Cargale el costo desde **Editar** o registrando una compra.

**La pantalla no se actualiza.**
Los cambios de otras PC llegan en unos 3 segundos. Si tenés un cuadro abierto, se actualiza al cerrarlo.

**No logro conectar desde otra PC.**
Revisá que la PC principal tenga el programa abierto en modo **Host**, que la IP y el puerto estén bien escritos, y pedile al administrador que revise la pestaña **Red** (modo *Toda la red local* y firewall).

**Me olvidé la contraseña.**
Pedile al administrador que te asigne una nueva desde **Usuarios**.

**¿Puedo trabajar sin internet?**
Sí. El programa funciona solo con la red local, o con una sola PC, sin internet.

---

## 8. Glosario

| Palabra | Qué significa |
|---|---|
| **Host** | La PC principal, donde se guardan los datos. |
| **Usuario (modo)** | Una PC que se conecta al host. |
| **Código (SKU)** | El código propio de cada producto; sirve para el lector de códigos de barras. |
| **Stock mínimo** | Cantidad desde la cual el programa avisa que hay que reponer. |
| **Seña** | Pago parcial de una venta; el resto queda como saldo pendiente. |
| **Saldo** | Lo que falta cobrar de una venta. |
| **Movimiento** | Cada vez que el stock sube o baja (venta, compra, ajuste, devolución). |
| **Respaldo** | Una copia de seguridad de toda la información. |
