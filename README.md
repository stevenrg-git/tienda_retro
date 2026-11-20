# tienda_retro
Figma Página Retro 
Luis Felipe SIerra Guzmán 
Steven Rengifo Gonzales 
Camilo Corena Tascón 
Ficha: 3387459 
Requisitos: 
Requisitos Funcionales: 
RF-01: Permitir registrar un usuario mediante nombre, correo electrónico y contraseña. 
RF-02: Permitir iniciar sesión mediante correo electrónico y contraseña. 
RF-02: Permitir al usuario recuperar contraseña en caso de no recordarla. 
RF-04: El sistema debe mostrar el catálogo de consolas y videojuegos separados. 
RF-05: Cada producto debe mostrar nombre, descripción y respectivo precio de compra. 
RF-06: Se debe mostrar en el catálogo de videojuegos a qué consola es compatible. 
RF-07: El sistema debe permitir hacer scroll horizontal y vertical para explorar el catálogo. 
RF-08: El sistema debe permitir comprar los productos seleccionados en una nueva página 
de carrito. 
RF-09: El sistema debe permitir ingresar un método de pago electrónico para la compra de 
productos. 
¡ 
RF-10: . El usuario puede buscar productos por su nombre. 
Requisitos No Funcionales: 
RNF-01: Ocultar y proteger las contraseñas y ocular los datos sensibles de la tarjeta de 
pago- 
 
RNF-02: Actualizar las cantidades, subtotales, impuestos y totales de forma rápida y 
automática. 
 
RNF-03: Mostrar los precios con el formato de la moneda local. 
 
Especificación 
Requisitos funcionales 
 
ID Especificación 
RF-01 
El sistema debe ofrecer un formulario de registro con los campos nombre, 
correo electrónico y contraseña. Debe validar que el correo tenga formato 
válido y no esté ya registrado, y que la contraseña cumpla una longitud 
mínima (8 caracteres). 
RF-02 
El sistema debe ofrecer un formulario de inicio de sesión con correo y 
contraseña, y dar acceso solo si las credenciales coinciden con un usuario 
registrado. 
RF-03 El sistema debe ofrecer la opción “¿Olvidaste tu contraseña?”, que solicite el 
correo y envíe un enlace temporal para crear una nueva contraseña. 
RF-04 El sistema debe mostrar dos secciones separadas, “Consolas” y “Juegos”, 
cada una con sus productos en tarjetas. 
RF-05 Cada tarjeta de producto debe mostrar nombre, descripción corta y precio de 
compra. 
RF-06 Cada tarjeta de videojuego debe indicar la consola con la que es compatible. 
RF-07 El catálogo debe poder recorrer con scroll vertical (página) y horizontal (filas 
de tarjetas por sección). 
RF-08 Al pulsar “Comprar”, el producto se agrega y el usuario es llevado a una 
página de carrito donde ve los productos seleccionados, cantidades y total. 
RF-09 En el carrito debe existir un formulario para ingresar un método de pago 
electrónico (tarjeta) y confirmar la compra. 
RF-10 El sistema debe ofrecer una barra de búsqueda que filtre los productos por 
nombre mientras el usuario escribe. 
 
 
Requisitos no funcionales 
 
ID Especificación 
RNF-01 
Los campos de contraseña deben mostrarse enmascarados (••••) y 
almacenarse cifradas. El número de tarjeta debe mostrarse parcialmente 
oculto (solo últimos 4 dígitos) y el CVV nunca debe mostrarse ni guardarse. 
RNF-02 Al cambiar cantidades o eliminar productos, el carrito debe recalcular subtotal, 
impuestos y total al instante, sin recargar la página. 
RNF-03 Todos los precios deben mostrarse en pesos colombianos (COP), con 
separador de miles, por ejemplo $150.000. 
 
 
Criterios de Aceptación 
Requisitos Funcionales 
 
 
ID Criterios de aceptación 
☑RF-01 
• Con datos válidos, la cuenta se crea y se muestra un mensaje de éxito. 
• Si el correo ya existe, se muestra un error claro. 
• Si falta algún campo o el correo es inválido, no se permite enviar el formulario. 
☑RF-02 
• Con credenciales correctas, el usuario accede a la tienda. 
• Con credenciales incorrectas, se muestra “Correo o contraseña incorrectos”. 
• No se revela cuál de los dos datos falló. 
☑RF-03 
• Al ingresar un correo registrado, se envía el enlace de recuperación. 
• El enlace permite definir una nueva contraseña y expira después de un 
tiempo. 
• Si el correo no existe, se muestra un mensaje genérico. 
☑RF-04 
• Consolas y juegos aparecen en secciones distintas y rotuladas. 
• Todos los productos de cada categoría son visibles. 
☑RF-05 • Ninguna tarjeta aparece sin nombre, descripción o precio. 
☑RF-06 
• Cada juego muestra el nombre de su consola compatible. 
• La consola mostrada coincide con la del producto. 
☑RF-07 
• Se puede desplazar la página hacia abajo y las filas de tarjetas hacia los 
lados. 
• El desplazamiento funciona con mouse, teclado y pantalla táctil. 
☑RF-08 
• Al pulsar “Comprar”, el producto aparece en el carrito. 
• El carrito lista nombre, cantidad, precio y total. 
• El usuario puede quitar productos. 
☑RF-09 
• El formulario pide número de tarjeta, titular, vencimiento y CVV. 
• Con datos inválidos no se permite confirmar la compra. 
• Con datos válidos se muestra confirmación de compra. 
☑RF-10 
• Al escribir un nombre, solo se muestran los productos que coinciden (sin 
importar mayúsculas). 
• Si no hay coincidencias, se muestra “No se encontraron productos”. 
 
 
Requisitos no funcionales 
 
ID Criterios de aceptación 
☑RNF-01 
• La contraseña se ve como puntos al escribirla. 
• El número de tarjeta se ve como •••• •••• •••• 1234 después de ingresarlo. 
• El CVV nunca queda visible. 
☑RNF-02 
• El total se actualiza en menos de 1 segundo tras cambiar una cantidad. 
• Subtotal + impuestos = total, sin errores de cálculo. 
☑RNF-03 
• Todos los precios usan el símbolo $ y puntos como separador de miles.w 
• El formato es el mismo en catálogo, carrito y confirmación. 
 
 
 
 
 
 
Requerimientos como Historia de Usuario 
 
 
ID Historia de usuario 
RF-01 Como visitante, quiero registrarme con mi nombre, correo y contraseña, para 
poder crear una cuenta y comprar en la tienda. 
RF-02 Como usuario registrado, quiero iniciar sesión con mi correo y contraseña, para 
acceder a mi cuenta de forma segura. 
RF-03 Como usuario, quiero recuperar mi contraseña si la olvido, para volver a entrar 
sin perder mi cuenta. 
RF-04 Como cliente, quiero ver las consolas y los videojuegos en secciones 
separadas, para encontrar fácilmente lo que busco. 
RF-05 Como cliente, quiero ver el nombre, la descripción y el precio de cada producto, 
para decidir si me conviene comprarlo. 
RF-06 Como cliente, quiero saber con qué consola es compatible cada juego, para no 
comprar uno que no pueda usar. 
RF-07 Como cliente, quiero desplazarme vertical y horizontalmente por el catálogo, 
para explorar todos los productos cómodamente. 
RF-08 Como cliente, quiero que los productos que elijo pasen a una página de carrito, 
para revisar mi compra antes de pagar. 
RF-09 Como cliente, quiero ingresar un método de pago electrónico, para pagar mi 
compra sin salir de la tienda. 
RF-10 Como cliente, quiero buscar productos por su nombre, para encontrar rápido un 
juego o consola específica. 
RNF-01 Como cliente, quiero que mi contraseña y los datos de mi tarjeta estén ocultos y 
protegidos, para sentirme seguro al usar la tienda. 
RNF-02 Como cliente, quiero que las cantidades, subtotales, impuestos y totales se 
actualicen solos y rápido, para saber siempre cuánto voy a pagar. 
RNF-03 Como cliente, quiero ver los precios en pesos colombianos co
