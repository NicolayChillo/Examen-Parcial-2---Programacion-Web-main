# Examen-Parcial-2---Programacion-Web
1. Estructura del sistema de préstamos
Los libros prestados se organizan como un array separado llamado librosPrestados. Para manipularlos:

Para agregar un libro a la lista de prestado usamos el método push para insertar el libro desde la lista de libros disponibles.
Para eliminar un libro de la lista de prestados usamos splice para removerlo de la lista y regresarlo a la de disponibles.
Nos permite gestionar fácilmente los libros con métodos de array, asegurando que no haya duplicados y manteniendo el estado actualizado .

2. Filtrado y búsquedas dinámicas
Para buscar libros por título, autor o género, utilizamos filtros. Comparando el criterio ingresado por el usuario con los atributos de cada libro, podemos devolver coincidencias. Esto permite búsquedas flexibles y resultados en tiempo real. Convertimos las cadenas a minúsculas ayuda a que la búsqueda sea insensible a mayúsculas o minúsculas.

3. Interacción con el usuario
La lista de libros disponibles y prestados se muestra manipulando el DOM. Esto se hace accediendo a los elementos HTML (como listas <ul>) y actualizando su contenido con elementos dinámicos. Cada vez que cambia el estado de los libros, se reconstruyen estas listas para reflejar los cambios. Esto brinda al usuario una interfaz clara e interactiva.

4. Alertas y recordatorios
Los recordatorios automáticos para la devolución de libros se pueden gestionar usando temporizadores. Con setTimeout, enviamos una alerta única después de un período específico, mientras que setInterval permite recordatorios periódicos. Esto mejora la experiencia al recordar al usuario la fecha límite de devolución de un libro prestado.

5. Eventos y usabilidad
Los eventos como onclick o onmouseover mejoran la interacción del usuario:

Eventos de clic: Asignan acciones específicas a botones
Eventos de mouse: Cambian el estilo al pasar el cursor, mejorando la visualización de elementos interactivos.
Eventos en inputs: Destacan los campos en los que el usuario escribe, haciendo la experiencia más amigable y accesible.

6. Funciones avanzadas
Funciones autoejecutables: Se utilizan para inicializar el sistema en el momento en que se carga la página, evitando conflictos de nombres en el código.
Funciones asíncronas: Son útiles para manejar operaciones que toman tiempo, como simulaciones o interacciones con un servidor. Estas permiten un flujo más lógico y fácil de entender para procesos secuenciales.

7. Simulación de procesos asíncronos
Para simular tiempos de espera al reservar o devolver libros, usamos temporizadores y promesas. Esto imita el retraso que ocurriría en una operación real (como una solicitud a un servidor). Las promesas permiten gestionar estos procesos de forma estructurada, proporcionando un flujo claro para manejar éxitos y errores, lo cual es ideal para crear una experiencia de usuario más realista.