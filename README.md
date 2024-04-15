# Aplicación de Microservicios con Spring Boot y Eureka

Esta es una aplicación de ejemplo que utiliza Spring Boot y Eureka para implementar una arquitectura de microservicios. A continuación se muestra el orden en el que deben ser inicializados los servicios:

1. **Eureka Server**: Este servicio actúa como el servidor de registro y descubrimiento de microservicios. Es necesario iniciarlo primero para que los demás servicios puedan registrarse correctamente.

2. **Gateway**: El servicio de Gateway es responsable de enrutar las solicitudes a los microservicios correspondientes. Se recomienda iniciarlo después de Eureka Server para que pueda descubrir los microservicios registrados.

3. **Config**: El servicio de Config es responsable de centralizar las configuraciones de los microservicios. Se recomienda iniciarlo después de Gateway para que los microservicios puedan obtener sus configuraciones correctamente.

4. **Teacher**: El servicio de Teacher es un microservicio que gestiona la información de los profesores.

5. **Student**: El servicio de Student es un microservicio que gestiona la información de los estudiantes.

6. **Nota**: El servicio de Nota es un microservicio que gestiona las notas de los estudiantes.

Recuerda que es importante seguir este orden de inicialización para garantizar que los microservicios se registren correctamente en Eureka y puedan comunicarse entre sí de manera adecuada.

## Configuración

Cada servicio puede tener su propia configuración específica. Asegúrate de revisar los archivos de configuración de cada microservicio para ajustar cualquier parámetro necesario.

## Contribución

Si deseas contribuir a este proyecto, siéntete libre de hacerlo. Puedes enviar pull requests con mejoras o correcciones.

## Licencia

Este proyecto se encuentra bajo la licencia MIT. Puedes consultar el archivo [LICENSE](LICENSE) para obtener más información.
