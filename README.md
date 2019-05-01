### [Extendeal](https://extendeal.com) Extendeal Frontend Test

![Extendeal](https://ar.extendeal.com/images/common/logo-extendeal.svg)

---

## Descripción e instalación

Se adjunta un proyecto de nodejs, con una pequeña base de datos y una api ya desarrollada. Para ejecutar el proyecto, una vez descargado hay que correr las siguientes líneas por línea de comandos en el root del proyecto:

## Installation

- `yarn install`
- `node server.js`

Los requisitos son únicamente tener instalado una versión de node >= 4 y npm. Si todo funcionó correctamente, va a correr el servidor, y vas a poder acceder a través de cualquier navegador en la dirección: localhost:8080. Se debería visualizar el html ubicado en public/index.html.

---

## server

- `api/products`
- `node server.js`

##Desarrollo
El objectivo del test es desarrollar 2 vistas utilizando la api incluida en el proyecto.

La primera consiste en una lista paginada de productos con un buscador. Se debe visualizar la imagen del producto con su respectivos datos al lado, como se ve a continuación:


##IMAGEN




| Método HTTP| Ruta| Descripción|
| ----- | ---- |  ---- |
| GET | /api/products | Devuelve la lista de todos los productos. Para paginar necesita recibir adicionalmente los parámetros `_page` y `_limit` : `api/products/?_page=1&_limit=5`. Para buscar, necesita el parámetro q: `/api/products/?q=texto` |
| GET | /api/products/id | Devuelve únicamente el producto especificado por el id |
| POST | /api/products | Crea un producto nuevo. Debe incluir el header `Content-Type: application/json`, y los parámetros en formato JSON. Ej: `{"name": "Algún nombre","price": "Algun precio","imageUrl": "Alguna URL"}` |
| DELETE | /api/products/id | Elimina el producto correspondiente al id dado. |



###Criterios de evaluación
Se pide específicamente el uso de React. Dará un valor adicional, aunque no es obligatorio, el uso además de Redux. Adicionalmente se evaluarán los siguientes puntos:

1. Utilización de patrones, buenas prácticas en el código y arquitectura acorde.
2. Documentación en el código.
3. Diseño lo más similar posible a las imágenes mostradas más arriba.
4. Tiempo en realizar la tarea.









