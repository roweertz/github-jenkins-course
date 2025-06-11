
# Requisitos
- Java 11 17 OpenJDK
- Minimo RAM 2, Recomendado 4GB
- Disco 1GB
- Navegadores: Chrome, Firefox, Edge
- Acceso a red: puerto 8080

# Jobs
- Una tarea automatizada -> Servidor Jenkins
    - Podria compilar
    - Ejecutar pruebas
    - Despliegue
    - Cualquier otro proceso

- Tipos de Jobs:
    - Freestyle Project -> el mas basico y facil de configurar
    - Pipeline -> usado para flujos de CI CD -> son mas avanzado con script con groovy
    - Multibranch pipeline -> ideal para proyectos con varias ramas en git
    - Maven Project -> para proyectos en maven