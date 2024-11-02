# Proyecto ADN Mutante

Este proyecto es una API REST que permite verificar si un humano es mutante basándose en su secuencia de ADN. La verificación se realiza mediante un algoritmo que busca secuencias de cuatro letras iguales de forma horizontal, vertical y diagonal. El resultado de la verificación se guarda en una base de datos H2 y se pueden obtener estadísticas de las verificaciones realizadas.

## Estructura del Proyecto

El proyecto está estructurado en capas: controladores, servicios, repositorios y entidades.

- **Controladores**: Manejan las solicitudes HTTP y las respuestas.
- **Servicios**: Contienen la lógica del negocio y las operaciones relacionadas con el ADN.
- **Repositorios**: Interactúan con la base de datos.
- **Entidades**: Representan las estructuras de datos que se almacenan en la base de datos.

## Tecnologías Utilizadas

- Java 17
- Spring Boot
- H2 Database
- Lombok
- JPA (Java Persistence API)

## Instrucciones para Ejecutar la Aplicación

1. **Descargar el repositorio en zip**
2. **Descomprimir el proyecto**
3. **Usar un IDE (Entorno de desarrollo integrado) para abrir el proyecto**
4. **Ejecutar la aplicacion desde el ide**
5. **Para probar las peticiones de la API** 
- Usar la aplicacion de Postman
- Crear una nueva coleccion con los metodos POST Y GET
- Para el endpoint POST usamos el link: http://localhost:8080/mutant/
  En la parte de raw colocar la siguiente estructura
  {
  "dna":["ATGCGA","CAGTGC","TTATGT","AGAAGG","CCCCTA","TCACTG"]
  }
- Para el endpoint GET usamos el link:http://localhost:8080/stats
- Solo va a funcionar cuando este localmente activo
- Para ver la base de datos ingresamos al link: http://localhost:8080/h2-console
  
6.**Para probar la app desde render**
- Usar la aplicacion de Postman
- Crear una nueva coleccion con los metodos POST Y GET
- Para el endpoint POST usamos el link: https://backendfinal-4pg1.onrender.com/mutant
- Para el endpoint GET usamos el link: https://backendfinal-4pg1.onrender.com/stats


  
