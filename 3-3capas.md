# Arquitectura de 3 capas

La arquitectura de 3 capas es un patrón de diseño comúnmente utilizado en el desarrollo de software. Se basa en dividir una aplicación en tres capas distintas, cada una con su propia responsabilidad y función específica. Estas capas son:

## Capa de presentación (o interfaz de usuario)

Esta capa es la encargada de interactuar con el usuario final. Aquí se encuentra la interfaz gráfica o la interfaz de línea de comandos a través de la cual los usuarios pueden interactuar con la aplicación. Su objetivo principal es mostrar la información al usuario y recibir sus acciones o entradas.

Ejemplos:

- Una aplicación web.
- Una interfaz por consola.
- Una aplicación de escritorio.
- Una aplicación móvil.
- Un servicio web.
- Un API

## Capa de Dominio / Capa de lógica de negocio

Esta capa contiene la lógica y las reglas de negocio de la aplicación. Aquí se procesan y manipulan los datos de acuerdo con las reglas y requisitos específicos del negocio. Esta capa es independiente de la interfaz de usuario y se encarga de realizar todas las operaciones y cálculos necesarios para que la aplicación funcione correctamente.

Ejemplo:

- Cálculos basados en datos de entrada y datos almacenados.
- Validaciones de datos que vienen de la capa de presentación.
- Definir qué algoritmo o lógica de negocio utilizar.

Otros nombres para la capa de dominio

- Capa de negocio.
- Capa de lógica de negocio.
- Capa de lógica de dominio.

## Capa de acceso a datos

Esta capa se encarga de interactuar con la base de datos o cualquier otro sistema de almacenamiento de datos utilizado por la aplicación. Aquí se realizan las operaciones de lectura y escritura de datos, consultas a la base de datos y cualquier otra interacción necesaria para acceder y manipular los datos de la aplicación.

Otros nombres para la capa de acceso a datos

- Capa de persistencia.
- Capa de datos.

## Conclusiones

La arquitectura de 3 capas proporciona una separación clara de responsabilidades y promueve la modularidad y la reutilización del código. Cada capa puede ser desarrollada y probada de forma independiente, lo que facilita el mantenimiento y la escalabilidad del sistema.
