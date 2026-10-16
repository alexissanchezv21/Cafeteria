app.js:
Es la conexion con el servidor, donde entran los parametros del formulario por medio del puerto 3000

database.js:
Se comunica con la BD

pedidoModel.js:
Ejecutar las setencias SQL, este tiene la función registrarPedido(), esta recibe los datos ya validados por el controlador. 
Ademas devuelve el ID del pedido.

pedidosControlador.js:
Recibe los datos enviados por el usuario y verifica que no esten vacios, en caso de estarlo manda un mensaje de error, envia los datos a
pedidoModel.js para guardalos en MySQL, ademas de generar la url que redirige al usuario

pedidoRoutes.js:
Es decirle al servidor que cuando el usuario mande sus datos, los envie a pedidosControlador

index.html:
Contiene el formulario diseñado para que el usuario mande sus datos por el metodo POST

style.css:
Le da el diseño al index

script.js:
Verifica que los campos no esten vacios, en caso de estarlos manda un mensaje de error.

resumen.html:
Es el que contiene la informacion registrada por el usuario con todos sus datos

resumen.css:
Contiene el diseño del resumen simulando un ticket de compra

scriptt.js:
Lee la barra de direcciones del navegador utilizando URLSearchParams
