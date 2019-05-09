### [Extendeal](https://extendeal.com) Extendeal Frontend Test

![Extendeal](https://ar.extendeal.com/images/common/logo-extendeal.svg)

---

## Descripción e instalación

Se adjunta un proyecto de nodejs, con una pequeña base de datos y una api ya desarrollada. Para ejecutar el proyecto, una vez descargado hay que correr las siguientes líneas por línea de comandos en el root del proyecto:

## Installation

- `yarn install`

Los requisitos son únicamente tener instalado una versión de node >= 4 y npm. Si todo funcionó correctamente, va a correr el servidor, y vas a poder acceder a través de cualquier navegador en la dirección: localhost:8080. Se debería visualizar el html ubicado en public/index.html.

---

## Server

- `api/products`
- `node server.js`

---

## Desarrollo
El objectivo del test es desarrollar 2 componentes productList y shopingCart. productList consiste en una lista de productos con un buscador (utilizando la api incluida en el proyecto.) cuando el producto es mayor que 1 la cantidad se debe actualizar o añadir al componente shopingCart, a su vez este componente tiene un botón para eliminar este item de la lista del shopingCart y a su vez actualizar la cantidad de lista de productos en 0.

Se debe visualizar la imagen del producto con su respectivos datos al lado, como se ve a continuación:

---

![image_test](https://github.com/musoxvi/extendeal-frontend-test/blob/master/public/images/extendeal_test.png)


---

| Método HTTP| Ruta| Descripción|
| ----- | ---- |  ---- |
| GET | /api/products | Devuelve la lista de todos los productos. Para paginar necesita recibir adicionalmente los parámetros `_page` y `_limit` : `api/products/?_page=1&_limit=5`. Para buscar, necesita el parámetro q: `/api/products/?q=texto` |


---

### Criterios de evaluación
Se pide específicamente el uso de React. Dará un valor adicional, aunque no es obligatorio, el uso además de Redux y test. Adicionalmente se evaluarán los siguientes puntos:

1. Utilización de patrones, buenas prácticas en el código y arquitectura acorde.
2. Diseño lo más similar posible a las imágenes mostradas más arriba.

---

