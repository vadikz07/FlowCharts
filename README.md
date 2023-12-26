# Entrada de datos por CLI -> JSON

## Descripción
Programa para insertar datos validados de objetos en formato JSON.

## Estructura de datos
- Estructura de un objeto en formato json, con sus tipos de datos.
 ``` {
    "uuid": str,
    "nombre": str,
    "modelo": str,
    "fabricante": str,
    "cantidad": int,
    "cantidadAviso": int,
    "cantidadMaxima": int,
    "datasheet": str,
    "notas": str,
    "fechaInsercion": str,
    "localizacion": int
  }
  ```

## Flujo del programa
- Ver flowchart añadido para mas instrucciones.
- En el momento que el usuario escriba exit en cualquiera de los campos, forzar salida del bucle de insercion, y guardar datos almacenados hasta ese punto.

## Notas importantes
- Los campos 'uuid' y 'fechaInsercion' son generados automaticamente por la interfaz grafica, no es necesaria su insercion por el formulario CLI.

## Requisitos de validacion
- [ ] 'nombre' = tipo str, longitud de cadena entre 3 y 30 **(inclusivos)**

- [ ] 'modelo' = tipo str, longitud de cadena entre 3 y 30 **(inclusivos)**

- [ ] 'fabricante' = tipo str, **si el campo esta vacio, debe considerarse valido**, pero si tiene texto ha de ser str, y con una longitud de entre 3 y 15 **(inclusivos)**

- [ ] 'cantidad' = tipo int, cantidad entre 1 y 999 (inclusivos)

- [ ] 'cantidadAviso' = tipo int, cantidad entre 1 y 999 **(inclusivos)**

- [ ] 'cantidadMaxima' = tipo int, cantidad entre 1 y 999 **(inclusivos)**

- [ ] 'datasheet' = tipo str, **si el campo esta vacio, debe considerarse valido**, pero si tiene texto ha de ser str, y con una longitud de entre 3 y 100 **(inclusivos)**

- [ ] 'notas' = tipo str, **si el campo esta vacio, debe considerarse valido**, pero si tiene texto ha de ser str, y con una longitud de entre 5 y 400 **(inclusivos)**

- [ ] 'localizacion' = tipo int, numero entre 1 y 99 **(inclusivos)**

## Formato de salida
- [ ] El programa debe generar un fichero JSON, que contenga todos los objetos que haya guardado el programa hasta que el usuario escriba exit en alguno de los campos.
