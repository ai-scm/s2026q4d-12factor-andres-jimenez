# s2026q4d-12factor-andres-jimenez
This repo contains the information of the 4 most important factors and their justification.

## Factor 1 - Código Base (Codebase):

Mantener un solo código controlado por versiones y con múltiples despliegues es vital para el desarrollo de un proyecto. Esto, pues permite tener de forma unida en el repositorio la información de los módulos y facilita la legibilidad y seguimiento de este. Además, el versionar el código permite realizar algún rollback en caso de tener un error y trazar los cambios hasta este.

## Factor 3 - Configuraciones (Config):

Este factor indica que se debe guardar la configuración que varía entre entornos, es decir, las variables de entorno. Esto es fundamental, pues permite configurar y adaptar el comportamiento de un sistema operativo y las aplicaciones, sin que sea nefcesario modificar el código fuente. Además otorga un nivel de seguridad de datos sensibles.

## Factor 10 - Paridad entre desarrollo y producción (Dev/prod parity):

Indica que se deben mantener los entornos de desarrollo y producción lo más similar que se pueda. Así mismo, se incluye el entorno de pruebas. De esta forma, se permite reducir el tiempo que lleva la escritura de código hasta su puesta en producción. Realiza una integración de los desarrolladores con el equipo de operaciones, solucionando el problema del muro de la confusión.

## Factor 11 - Historiales / Registros (Logs):

Indica que se deben tratar los logs como flujos de eventos continuos sin que la app decida dónde se almacenan o rotarlos. De esta forma, se desacopla su persistencia de la aplicación. Evita que la aplicación llene la memoria del servidor o contenedor, reduce el acoplamiento con el sistema de archivos local, permitiendo el cambio de erramienta de monitoreo.

El uso de logs, al tratarlos como flujos de eventos, permiten tener trazabilidad de las funciones en la aplicación, por ejemplo, para la revisión de fallos.