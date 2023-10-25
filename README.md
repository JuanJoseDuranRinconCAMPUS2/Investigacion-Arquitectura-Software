# **♻️📃Patrón "Arquitectura Orientada a Microservicios"📃♻️**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-Arquitectura-MicroServicios/imgs/investigacionmicroservicios.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón "Arquitectura Orientada a Microservicios"

![](https://i.imgur.com/7ud53ww.gif)

------

## ♻️**🔑**Patrón Orientado a Microservicios🔑♻️

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTgArxwaVxun8KpIKG9nEycC9k6Zr95xAFa6kObcygizlPpbbPvKYivZTBqTHNrOVjqOKM&usqp=CAU" alt="Indice" style="zoom:120%;" />

La arquitectura de microservicios es un método de desarrollo de aplicaciones software que funciona como un conjunto de pequeños servicios que se ejecutan de manera independiente y autónoma, proporcionando una funcionalidad de negocio completa. En ella, cada microservicio es un código que puede estar en un lenguaje de programación diferente, y que desempeña una función específica. Los microservicios se comunican entre sí a través de APIs, y cuentan con sistemas de almacenamiento propios, lo que evita la sobrecarga y caída de la aplicación.

Los microservicios son pequeños e independientes, y están acoplados de forma imprecisa. Un único equipo reducido de programadores puede escribir y mantener un servicio.

## Dato curioso:

Admite la programación políglota. Por ejemplo, no es necesario que los servicios compartan la misma pila de tecnología, las bibliotecas o los marcos.

```js
Cada servicio es un código base independiente, que puede administrarse por un equipo de desarrollo pequeño.
```
[^Informacion]: https://learn.microsoft.com/es-es/azure/architecture/guide/architecture-styles/microservices
------

♻️**⚜️**Ventajas del Patrón Orientado a Microservicios⚜️♻️
------

<img src="https://www.chakray.com/wp-content/uploads/2021/05/microservices-spanish.svg" style="zoom:80%;" />

- **Modularidad:** al tratarse de servicios autónomos, se pueden desarrollar y desplegar de forma independiente. Además un error en un servicio no debería afectar la capacidad de otros servicios para seguir trabajando según lo previsto.
- **Escalabilidad:** como es una aplicación modular, se puede escalar horizontalmente cada parte según sea necesario, aumentando el escalado de los módulos que tengan un procesamiento más intensivo.
- **Versatilidad:** se pueden usar diferentes tecnologías y lenguajes de programación. Lo que permite adaptar cada funcionalidad a la tecnología más adecuada y rentable.
- **Rapidez de actuación:** el reducido tamaño de los microservicios permite un desarrollo menos costoso, así como el uso de “contenedores de software” permite que el despliegue de la aplicación se pueda llevar a cabo rápidamente.
- **Mantenimiento simple y barato:** al poder hacerse mejoras de un solo módulo y no tener que intervenir en toda la estructura, el mantenimiento es más sencillo y barato que en otras arquitecturas.
- **Agilidad:** se pueden utilizar funcionalidades típicas (autenticación, trazabilidad, etc.) que ya han sido desarrolladas por terceros, no hace falta que el desarrollador las cree de nuevo.
[^Informacion]: https://decidesoluciones.es/arquitectura-de-microservicios/
------

♻️**⚠️**Desventajas del Patrón Orientado a Microservicios⚠️♻️
------

<img src="https://i.pinimg.com/564x/7c/96/38/7c9638e1180f4cdae0398c06d82e2257.jpg" />

- **Alto consumo de memoria:** al tener cada microservicio sus propios recursos y bases de datos, consumen más memoria y CPU.

- **Inversión de tiempo inicial:** al crear la arquitectura, se necesita más tiempo para poder fragmentar los distintos microservicios e implementar la comunicación entre ellos.

- **Complejidad en la gestión:** si contamos con un gran número de microservicios, será más complicado controlar la gestión e integración de los mismos. Es necesario disponer de una centralización de trazas y herramientas avanzadas de procesamiento de información que permitan tener una visión general de todos los microservicios y orquesten el sistema.

- **Perfil de desarrollador:** los microservicios requieren desarrolladores experimentados con un nivel muy alto de experiencia y un control exhaustivo de las versiones. Además de conocimiento sobre solución de problemas como latencia en la red o balanceo de cargas.

- **No uniformidad:** aunque disponer de un equipo tecnológico diferente para cada uno de los servicios tiene sus ventajas, si no se gestiona correctamente, conducirá a un diseño y arquitectura de aplicación poco uniforme.

- **Dificultad en la realización de pruebas:** debido a que los componentes de la aplicación están distribuidos, las pruebas y test globales son más complicados de realizar.

- **Coste de implantación alto:** una arquitectura de microservicios puede suponer un alto coste de implantación debido a costes de infraestructura y pruebas distribuidas.

[^Informacion]: https://decidesoluciones.es/arquitectura-de-microservicios/
------

  ## ♻️**🧮**Características de los Patrones Orientados a Microservicios🧮♻️

<img src="https://blog.seur.com/wp-content/uploads/2012/11/efra.jpg" style="zoom:60%;" />

- ## **Autónomos**

- ## Especializados
[^Informacion]: https://aws.amazon.com/es/microservices/
------

## ♻️**📛**Autónomos📛♻️

<img src="https://static.wixstatic.com/media/35ed10_dc731e82dcb84ef8a1cf8131ba933c78~mv2.png/v1/fit/w_1000%2Ch_620%2Cal_c%2Cq_80,enc_auto/file.jpg" style="zoom:57%;" />

Cada servicio componente en una arquitectura de microservicios se puede desarrollar, implementar, operar y escalar sin afectar el funcionamiento de otros servicios. Los servicios no necesitan compartir ninguno de sus códigos o implementaciones con otros servicios. Cualquier comunicación entre componentes individuales ocurre a través de API bien definidas.

------

## ♻️🧱Especializados🧱♻️

<img src="https://media.licdn.com/dms/image/C5612AQHJ7qhfGK0dIg/article-cover_image-shrink_600_2000/0/1618584375404?e=2147483647&v=beta&t=miDHd9SdRgWjCChovzVbsLkpHF8SimakIrJ0I0SC-Ak" />

Cada servicio está diseñado para un conjunto de capacidades y se enfoca en resolver un problema específico. Si los desarrolladores aportan más código a un servicio a lo largo del tiempo y el servicio se vuelve complejo, se puede dividir en servicios más pequeños.

------
## ♻️**💻**SOA en comparación con los microservicios💻♻️

<img src="https://learn.microsoft.com/es-es/azure/architecture/includes/images/microservices-logical.png" style="zoom:57%;" />

La arquitectura de microservicios es una evolución del estilo arquitectónico de SOA. Los microservicios tratan los defectos de SOA para hacer que el software sea más compatible con entornos empresariales modernos basados en la nube. Son detallados y favorecen la duplicación de datos en contraste con el intercambio de datos. Por ello, son completamente independientes y cuentan con sus propios protocolos de comunicación que se exponen a través de API sencillas. Básicamente, es el trabajo de los consumidores utilizar el microservicio a través de su API, lo que elimina la necesidad de un ESB centralizado.

[^Informacion]: https://aws.amazon.com/es/what-is/service-oriented-architecture/
------

## ♻️**🎀**Aplicaciones Que Usan Patrones Orientados a Microservicios🎀♻️

- Aplicaciones Web y Móviles
- Aplicaciones de Juegos en Línea
- Redes Sociales
- Plataformas de Viajes y Reservas
- Comercio Electrónico
- Servicios de Salud
- Plataformas de E-learning

------
> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------