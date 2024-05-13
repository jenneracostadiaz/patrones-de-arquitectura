# Implementar Capas

## Cómo se puede implementar una capa?

- Un método
- Una clase
- Un paquete
- Una librería

## Cómo se puede implementar una capa de dominio?

Tenemos 4 patrones principales:

- Script de transacción
- Modelo de dominio
- Módulo de tabla
- Capa de servicios

### Script de transacción

Es una forma de implementar una capa de dominio utilizando un script o secuencia de comandos que encapsula la lógica de negocio relacionada con una transacción específica.

### ¿En qué casos usar script de transacción?

Los scripts de transacción son útiles en los siguientes casos:

- Cuando se necesita implementar una lógica de negocio simple y directa que se ejecuta en una transacción específica.
- Cuando se desea tener un control detallado sobre la secuencia de pasos en una transacción.
- Cuando se necesita una implementación rápida y sencilla sin la necesidad de crear clases o estructuras de datos complejas.

### ¿Qué problemas tiene este patrón?

- Duplicidad de código
- Es difícil escribir una lógica de dominio compleja
- No es fácil mantener un diseño coherente

## Modelos de Dominio

Se utilizan para representar y encapsular la lógica de negocio y las reglas del dominio en una aplicación. Consiste en definir clases y estructuras que representan los conceptos y entidades del dominio, así como las relaciones y comportamientos entre ellos.

Es un modelo de objetos que tienen tanto comportamiento como datos.

Es similar a un modelo de base de datos, pero tiene diferencias:

- Mezcla de datos y procesamiento
- Tiene atributos multivaluados (arreglos, colecciones, listas, etc.)
- Puede incluir relaciones complejas
- Soporta herencia

### ¿Cómo organizar los modelos?

- Simple: Relación uno a uno entre tablas y clases
- Elaborada: Se ve diferente al diseño de base de datos

### ¿En qué casos usar el modelo de dominio?

- Aplicaciones complejas
- Reglas de negocio cambiantes que requieren múltiples cálculos, validaciones, entre otros.

### ¿Qué problemas tiene este patrón?

- Los objetos se pueden tornar enormes
- Acceso a base de datos complicado por el mapeo entre clases del dominio y las tablas

## Capa de Servicios

- Define operaciones disponibles para distintos clientes.
- Permite separar la lógica de negocio de la lógica de la aplicación.
- Se implementan como fachadas.

## Módulo de tabla

- Se tiene una única instancia que maneja la lógica de negocio para todas las filas en una tabla de la base de datos.

## Conclusiones

- La implementación de capas es una práctica común en el desarrollo de software para separar las responsabilidades y mejorar la modularidad.
- Los diferentes patrones de implementación de capas ofrecen distintas ventajas y desafíos, por lo que es importante elegir el enfoque adecuado según las necesidades del proyecto.
- Los modelos de dominio son especialmente útiles en aplicaciones complejas con reglas de negocio cambiantes, pero requieren una cuidadosa organización y consideración del acceso a la base de datos.
- La capa de servicios permite separar la lógica de negocio de la lógica de la aplicación, lo que facilita la reutilización y el mantenimiento.
- El módulo de tabla es una opción más simple para manejar la lógica de negocio en una tabla de la base de datos, pero puede tener limitaciones en aplicaciones más complejas.
