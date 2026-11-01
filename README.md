# diw-flexbox1-jimenez-prieto-jose

1.  Flexbox
    Para que el pie de página no se me quede flotando a mitad de la pantalla cuando hay poco contenido, configuré el body como un contenedor Flexbox en columna (display: flex y flex-direction: column) ocupando el 100% del alto de la ventana (min-height: 100vh). Luego le metí un flex: 1 a la clase .principal. Con esto consigo que el contenedor del centro absorba todo el espacio disponible y empuje el footer al final automáticamente.

-

2. Cabecera
   En la .cabecera usé Flexbox centrado verticalmente con justify-content: space-around para repartir el espacio entre la marca y la navegación. Para no tener problemas en móviles, le añadí flex-wrap: wrap y la propiedad gap: 1rem; así, si la pantalla es estrecha, el menú baja de línea limpiamente sin romperse.

3. Estilos del menú
   A la lista .menu\_\_lista le quité los puntos que vienen por defecto mediante list-style: none y coloqué los enlaces en horizontal usando display: flex. Para indicar la pestaña activa sin crear clases extra innecesarias, aproveché el atributo de accesibilidad usando el selector [aria-current="page"], dándole negrita y un borde inferior amarillo (#facc15).

4. Pie de página
   En el contenedor .pie volví a tirar de Flexbox, pero esta vez usé justify-content: space-between. Con esto envío el copyright al extremo izquierdo y la lista de enlaces legales al derecho sin andar metiendo márgenes a ojo.
