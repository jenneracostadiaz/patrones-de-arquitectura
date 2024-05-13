# Acceso a Datos

## Gateway de datos de Tabla

Es un objeto que encapsula el acceso a un sistema o recurso externo, se caracteriza por:

- Una única instancia maneja todas las filas de la tabla
- Normalmente existe uno por cada tabla de la base de datos
- Patrón de acceso a datos más sencillo

### ¿Con qué patrones de dominio funciona mejor?

- Script de Transacción ✅
- Modelo de dominio ❌
- Módulo de tabla ✅

## Gateway de datos de Fila

- Se tiene una instancia por cada fila de la tabla
- No debería tener lógica de negocio

### ¿Con qué patrones de dominio funciona mejor?

- Script de Transacción ✅
- Modelo de dominio ❌
- Módulo de tabla ✅

## Active Records

- Muy similar al gateway de datos de fila
- Es un objeto que tiene tanto datos como comportamiento
- Contiene tanto lógica de negocio como lógica de acceso a datos

### Algunas implementaciones

- Active Record (Ruby)
- Django (Python)
- Laravel (Eloquent) Yii

### ¿Con qué patrones de dominio funciona mejor?

- Script de Transacción ✅
- Modelo de dominio ✅
- Módulo de tabla ❌

### Críticas

- Mezclar lógica de negocio y acceso a datos va en contra del principio de única responsabilidad

## Mapeador de datos (Data Mapper)

- Es una capa de mapeadores que mueve datos entre objetos y base de datos
- Mantiene independencia entre el dominio y el acceso a datos
- Es útil para escenarios complejos

### Funcionalidades que puede necesitar

- Mapear clases cuyos datos vienen de múltiples tablas
- Clases con herencia
- Detectar qué objetos deben ser insertados, actualizados o eliminados
- Cargar datos de acuerdo a las relaciones entre objetos
- Llevar registro de qué objetos ya fueron cargados

### Frameworks ORM

- Mapeo Objeto-Relacional
- Alternativa para implementar mapeo entre objetos y tablas

### Algunos ejemplos de ORM

- Hibernate (Java)
- Entity Framework NHibernate (.NET)

### ¿Con qué patrones de dominio funciona mejor?

- Script de Transacción ❌
- Modelo de dominio ✅
- Módulo de tabla ❌

## Conclusiones

- El patrón Gateway de datos de Tabla es más sencillo y adecuado para acceder a una tabla completa en la base de datos.
- El patrón Gateway de datos de Fila es útil cuando se necesita acceder a filas individuales de una tabla.
- Active Records permite combinar datos y comportamiento en un solo objeto, pero puede violar el principio de única responsabilidad.
- El Mapeador de datos (Data Mapper) es útil para escenarios complejos donde se necesita mapear datos entre objetos y la base de datos de manera independiente.
- Los Frameworks ORM proporcionan una alternativa para implementar el mapeo entre objetos y tablas, siendo útiles en el modelo de dominio.
