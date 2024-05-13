# Patrón de Arquitectura por Capas

El patrón de arquitectura por capas es ampliamente utilizado en el desarrollo de aplicaciones empresariales y sistemas complejos. Conocida también como arquitectura de multicapas / N capas. Es un patrón donde tenemos grupos de subtareas. El patrón de arquitectura por capas proporciona una estructura organizada y modular para el desarrollo de aplicaciones. Permite separar las responsabilidades y funcionalidades en diferentes capas, lo que facilita la mantenibilidad y escalabilidad del sistema.

## Características:

- Los componentes están organizados en capas horizontales.
- Cada capa tiene un rol y una responsabilidad única dentro de la aplicación.
- Tiene que haber capas de alto nivel y capas de bajo nivel.
  - Mientras más arriba la capa, está más cerca del cliente.
  - Una capa de bajo nivel está más cerca del hardware.
- El patrón no define cuántas capas son ni de qué tipo deben ser.
- Las capas inferiores no deben tener ningún conocimiento de las capas superiores.
- Cada capa crea una abstracción de la funcionalidad que ofrece, una abstracción oculta ciertos detalles de cómo está hecha.
- Si las capas están bien diseñadas, se pueden reemplazar unas por otras.
- Los componentes de cada capa solo deben hacer tareas relacionadas con la capa.

Existen 2 tipos de capas en general:

- Capas Cerradas
- Capas Abiertas

Las capas cerradas son aquellas que no pueden ser modificadas o extendidas, mientras que las capas abiertas permiten la adición de nuevas funcionalidades.

## Conclusiones

- Es importante diseñar las capas de manera adecuada, evitando que las capas inferiores dependan de las superiores.
- La abstracción de la funcionalidad en cada capa permite ocultar detalles de implementación y facilita la sustitución de componentes.
- Cada capa debe enfocarse en tareas relacionadas con su responsabilidad específica.
- El número y tipo de capas puede variar según los requisitos y características del proyecto.
