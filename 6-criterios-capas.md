# Criterios para usar la Arquitectura por Capas

## Beneficios

- Separación de responsabilidades: La arquitectura por capas permite separar las diferentes responsabilidades de un sistema en capas distintas, lo que facilita la comprensión y el mantenimiento del código.
- Reutilización de código: Al tener una estructura modularizada en capas, es más fácil reutilizar componentes y funcionalidades en diferentes partes del sistema.
- Escalabilidad: La arquitectura por capas permite escalar el sistema de manera más sencilla, ya que cada capa puede ser escalada de forma independiente.
- Facilidad de prueba: Al separar las capas, es más fácil realizar pruebas unitarias y de integración en cada una de ellas, lo que mejora la calidad del software.
- Flexibilidad: La arquitectura por capas permite realizar cambios en una capa sin afectar a las demás, lo que brinda mayor flexibilidad al sistema.

## Desventajas

- Mayor complejidad: La arquitectura por capas puede introducir una mayor complejidad en el sistema debido a la necesidad de gestionar las interacciones entre las capas.
- Sobrecarga de comunicación: Al existir una separación clara entre las capas, puede haber una sobrecarga de comunicación entre ellas, lo que puede afectar el rendimiento del sistema.
- Rigidez: La arquitectura por capas puede resultar en una mayor rigidez del sistema, ya que los cambios en una capa pueden requerir modificaciones en otras capas.
- Dificultad para mantener la consistencia: Si no se gestionan adecuadamente, las capas pueden dificultar el mantenimiento de la consistencia de los datos en el sistema.
- Mayor tiempo de desarrollo: La estructura por capas puede requerir más tiempo de desarrollo inicial debido a la necesidad de diseñar y desarrollar las diferentes capas de manera independiente.

## Atipatrones

- Monolito: En lugar de separar las responsabilidades en capas, todas las funcionalidades se encuentran en un único componente monolítico, lo que dificulta la comprensión y el mantenimiento del código.
- Capas acopladas: Las capas están fuertemente acopladas entre sí, lo que significa que los cambios en una capa pueden tener un impacto directo en otras capas, generando una mayor complejidad y rigidez en el sistema.
- Capas con dependencias circulares: Existen dependencias circulares entre las capas, lo que dificulta la comprensión y el mantenimiento del código, así como la reutilización de componentes.
- Capas con lógica de negocio: Las capas contienen lógica de negocio en lugar de simplemente actuar como capas de abstracción, lo que puede generar una mayor complejidad y dificultad para realizar cambios.
- Capas con exceso de responsabilidades: Las capas tienen un exceso de responsabilidades, lo que dificulta la comprensión y el mantenimiento del código, así como la reutilización de componentes.

## Calificación del Patrón

- Facilidad de Desarrollo ✅
- Testeabilidad ✅
- Agilidad 🎭
- Rendimiento 🎭
- Facilidad despiegue ❌
- Escalabilidad ❌
