# Revisión de TuGallinero.app

Archivo preparado para publicar: `registro-huevos.html`.

## Correcciones aplicadas

1. Los datos de producción se separan por semana; al comenzar una nueva, el registro diario se reinicia.
2. Las ventas ahora exigen una cantidad entera positiva y no pueden superar el stock disponible.
3. Las fichas, encargados y ventas se renderizan con nodos seguros en lugar de insertar datos del usuario como HTML.
4. Las fotos se validan, se limita su tamaño a 8 MB y se informa cuando el almacenamiento local no alcanza.
5. Se añadieron botones para eliminar registros y un aviso accesible para lectores de pantalla.
6. El formulario responde a la tecla Enter y los campos de foco son más visibles.
7. Se verificó la sintaxis de los dos scripts y la codificación UTF-8 del archivo.

## Mejoras recomendadas

- Permitir editar los registros existentes, además de eliminarlos.
- Conservar y consultar el historial de semanas anteriores (la versión actual protege contra mezclar semanas, pero no crea una vista de historial).
- Valorar IndexedDB si se esperan muchas fotos.
- Ordenar el CSS: hay reglas repetidas para `.dashboard` y media queries duplicadas, lo que hace más difícil mantenerlo.
- Incluir un `README.md` para publicación y, si se convierte en proyecto, separar CSS y JavaScript del HTML.

## Prueba realizada

Se revisó el HTML, CSS y JavaScript estáticos. La sintaxis de los dos scripts y la codificación UTF-8 se verificaron tras aplicar los cambios. La inspección visual automatizada del enlace `file://` fue bloqueada por la política del navegador integrado.
