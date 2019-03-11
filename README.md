# Prueba Angular

### Desarrollar una aplicación de catalogo de contenidos simple en angular 7 que cumpla con los siguientes requisitos:

- Para la obtención de datos, se realizara la llamada:
`https://orangetv.orange.es/pc/api/rtv/v1/GetUnifiedList?client=json&external_category_id=SED_14462&filter_empty_categories=true&statuses=published`
, esta retornara una serie de elementos correspondientes a una serie de televisión.

  Las imagenes de caratula residen dentro de attachments, utilizar el elemento con name `'APP_COVER5'`. Para obtener la url completa de la imagen se deberan añadir como prefijo al value del elemento `'https://orangetv.orange.es/pc/api/rtv/v1/images'`.
  
  ```
  Ejemplo:
  
      https://orangetv.orange.es/pc/api/rtv/v1/images/IMAGES/O/PRG_0000061327HD_APP_COVER5.jpg
  ```
- Se debera crear un componente carousel similar al que usa Netflix para sus series (no hace falta que sea un calco, se trata solo de un ejemplo de funcionalidad). El componente admitira como input un array de datos sobre el que construira el carousel.

- Se creara adicionalmente un componente detail al cual se navegara al pulsar sobre un elemento del carousel mostrando información adicional sobre el elemento sobre el cual se esta navegando.

- Mostrar un spinner o placeholder component durante la navegacion hacia el detail (simular el delay con un timeout de 1 segundo).

- No hace falta que los estilos y/o animaciones sean muy sofisticados, pero hacer que la aplicación se vea razonablemente bien y en cuanto a responsive que se pueda visualizar almenos en los tamaños de pantalla de tipo desktop, de hd a fullHd.

- No se puede usar librerias externas para la construcción del carousel.

- Una vez completada la prueba subir a un repositorio de Github y añadir un `README.md` explicando como hacer el run/deploy para visualizar la prueba.

### Puntos opcionales:

- El componente de carousel debera de aceptar un input para poder hacer un uso del mismo en forma de layout horizontal o vertical.

- Crear una directiva que se pueda aplicar al carousel para dar soporte de desplazamiento al scroll wheel del ratón.

- El indice inicial del carousel se podra controlar con queryParams.

- Hacer uso de NgRx para el state management de la aplicacion.
