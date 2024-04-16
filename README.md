# Prueba técnica Frontend Middle

## Contexto
El objetivo de la prueba es conocer las habilidades técnicas del candidato bajo el entorno de desarrollo con el que se trabaja en Arkeero 2.0.

## Desarrollo frontend
Desarrolla una pequeña aplicación usando NextJS que cumpla con los siguientes requisitos:

1. Se debe contar con una sección de bienvenida.
2. Usar rutas de next para navegar entre las diferentes vistas.
3. La aplicación debe mostrar una lista de clientes, con su paginación.
4. Dentro de la lista o tabla debe tener un input que permite buscar cliente por su nombre, la búsqueda debe hacerse por cada página no es necesario búsqueda global.
5. Cada cliente debe mostrar su nombre, status(active, disable), descripción y tipo de cuenta(master, owner, basic).
6. Debe haber un botón “nuevo cliente”.
7. Al hacer clic en el botón para agregar un nuevo cliente, se debe abrir una nueva página donde estén dos tabs:
    - ClienteOne: este debe contener nuevo formulario de ClienteOne, los campos para el formulario deben ser:
        i. Nombre
        ii. Status (active, disabled)
        iii. Descripción
        iv. Tipo de cuenta(master, owner, basic)
        v. contactos, los contactos pueden ser más de uno, separando por (,) o espacios, el siguiente contacto en un mismo input (input multiple).
    - ClienteTwo: éste debe ser igual al formulario de ClienteOne solo que debe tener un radiobutton que diga: “cargar datos del ClienteOne” y se deben rellenar los campos del ClienteOne, en dado caso que no solo rellenar los campos de forma manual.
8. Al dar clic en el botón guardar debe aparecer un modal de confirmación: ”Está seguro de guardar los datos”. Si es si los datos se deben enviar (dejar la data en console log del lado del servidor de nextJS), si es no los debe volver al formulario.
9. Dentro de la lista o tabla de clientes cada cliente debe tener editar cliente, se debe abrir el modal con los datos de crear para editar el cliente y permitir editar los datos del cliente visualizado.
10. Al dar clic en guardar debe tener el modal de confirmación: ”Está seguro de guardar los datos”. Si es si los datos se deben enviar (dejar la data en console log del lado del servidor de next), si es no los debe volver al formulario.
11. Dentro de los clientes debe tener un botón de activar o deshabilitar cliente esto permite cambiar el estatus del cliente sin recargar la lista o tabla de clientes.

## Nota para ejecución
- Consumir el endpoint: https://api.json-generator.com/templates/9ZT8mBiV5UFu/data
- Token del endpoint: Bearer muwzxphjdhmgfwvsoqbsnwb2tdvs6sdsnggh6mko

## Qué se evaluará
- Creación de componentes reutilizables.
- Hacer uso del paso propiedades entre componentes.
- Consumo de APIs consumiendo de forma correcta el API y usando de forma correcta el servidor de NextJS y el cliente de NextJS.
- Se debe validar dentro del formulario de creación de cliente que la descripción no sea mayor a 150 caracteres, validación de errores dentro del formulario.
- Uso de contextos o stores (Redux, Zustand, o el de su preferencia).
- Uso de buenas prácticas.
- Diseño responsivo.
- El diseño es a libre albedrío de igual manera el uso de framework de diseño en dado caso no usarlo explicar que no los uso.
- Cada prueba se evaluará según su completitud, calidad del código, manejo de errores, seguridad y eficiencia.
- La prueba debe enviarse en un repositorio público de GitHub.

## Puntos Extras
- Uso de React Hook Form para validación de formularios, acompañado de un schema builder (zod, yup, valibot, o el de su preferencia).
- Despliegue de la aplicación (compartir el URL del despliegue).
- Hacer commits de progreso.

¡Suerte y que la fuerza te acompañe!
