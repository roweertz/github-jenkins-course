
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

# Builds
- Es una ejecución de un job
- Cada vez que se realice una ejecucion, se genera un build
    - Obtener el codigo fuente
    - Ejecuta los pasos que se ah obtenido
    - Registra la salida en la consola
    - Guarda artefactos (Opcional)
    - Muestra el resultado del build en la interfaz

# Disparadores automaticos
- Polling SCM -> Revisar periodicamente si hay cambios en el repositorio git
- Webhook -> Dispara el job cuando hay un cambio en el codigo
- Programacion Cron -> Se ejecuta en intervalos de tiempo
- Disparo por otro job -> Un job podra ejecutar cuando otro job termine

# Variables
- BUILD_NUMBER: Numero del build actual
- JOB_NAME: Nombre de job que se esta ejecutando
- WORKSPACE: directorio donde jenkis almacena los archivos del job
- GIT_COMMIT: hash del commit si el job usa git

# Ejecutar un programa en python desde jenkins
Docker -> Contenedor(Linux - Jenkins)

docker exec -it --user root nombrecontenedor /bin/bash
apt-get update
apt-get install -y python3 python3.pip