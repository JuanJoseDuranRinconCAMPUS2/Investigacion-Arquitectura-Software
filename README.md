# **🎲📃Patrón "Arquitectura Orientada a Servicios"📃🎲**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-Orientada-A-Servicios/imgs/investigacionSOA.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón "Arquitectura Orientada a Servicios"

![](https://i.imgur.com/fsOY5LE.gif)

------

## 🚾**🔑**Patrón Orientado a Servicios(SOA)🔑🚾

<img src="https://f.hubspotusercontent20.net/hubfs/2829524/H_arquitectura_orientada_servicios.jpg" alt="Indice" style="zoom:60%;" />

La arquitectura orientada a servicios(SOA, por sus siglas en inglés) es un método de desarrollo de software que utiliza componentes de software llamados servicios para crear aplicaciones empresariales. Cada uno de estos servicios brinda una capacidad empresarial y, además, pueden comunicarse también con el resto de servicios mediante diferentes plataformas y lenguajes. Los desarrolladores usan SOA para reutilizar servicios en diferentes sistemas o combinar varios servicios independientes para realizar tareas complejas.

SOA, o arquitectura orientada a servicios, define una manera de hacer que los componentes de software sean reutilizables a través de interfaces de servicio. Los servicios utilizan estándares de interfaz comunes y un patrón arquitectónico para que puedan incorporarse rápidamente a aplicaciones nuevas. De este modo, se evitan determinadas tareas al desarrollador de aplicaciones, que antes debía volver a desarrollar o duplicar la funcionalidad existente o tenía que saber cómo conectar o proporcionar Inter operatividad con las funciones existentes.

## Dato curioso:

Aunque la SOA y la [arquitectura de microservicios comparten muchas palabras en común (es decir, "servicio" y "arquitectura"), solo están relacionadas de manera vaga y, de hecho, operan en diferentes ámbitos, como se explica más adelante en este artículo.

```js
Los servicios utilizan estándares de interfaz comunes y un patrón arquitectónico para que puedan incorporarse rápidamente a aplicaciones nuevas. 
```
[^Informacion]: https://aws.amazon.com/es/what-is/service-oriented-architecture/
------

🚾**⚜️**Ventajas del Patrón Orientado a Servicios(SOA)⚜️🚾
------

<img src="https://static.s123-cdn-static-c.com/uploads/2175538/2000_5ce9a575c6f7c.png" style="zoom:80%;" />

- **Reducción del plazo de comercialización:** Los desarrolladores reutilizan servicios en diferentes procesos empresariales para ahorrar tiempo y dinero. Pueden crear aplicaciones en menos tiempo con SOA en lugar de escribir código y llevar a cabo integraciones desde cero.
- **Mantenimiento eficiente:** Es más fácil crear, actualizar y corregir errores en servicios pequeños que en bloques grandes de código en aplicaciones monolíticas. La modificación de un servicio en SOA no afecta a la funcionalidad general del proceso empresarial.
- **Excelente capacidad de adaptación:** La SOA se adapta de mejor manera a los avances tecnológicos. Puede modernizar sus aplicaciones de forma eficiente y rentable. Por ejemplo, los organizaciones de atención médica pueden utilizar la funcionalidad de sistemas de registro de salud electrónico antiguos en aplicaciones basadas en la nube que son más recientes.
[^Informacion]: https://aws.amazon.com/es/what-is/service-oriented-architecture/
------

🚾**⚠️**Desventajas del Patrón Orientado a Servicios(SOA)⚠️🚾
------

<img src="https://i.pinimg.com/564x/6e/bf/a6/6ebfa6babb801c4981571b5636764a5d.jpg" style="zoom:60%;" />

- **Escalabilidad limitada:** La escalabilidad de sistemas se ve seriamente afectada cuando los servicios comparten varios recursos y necesitan coordinarse para realizar su respectiva funcionalidad. 

- **Aumento en las interdependencias:** Los sistemas de la arquitectura orientada a servicios (SOA) se pueden volver cada vez más complejos y desarrollar varias interdependencias entre servicios. Puede ser complicado modificar o corregir errores si varios servicios se llaman entre sí en bucle. Los recursos compartidos, como las bases de datos centralizadas, también pueden ralentizar el sistema.

- **Punto único de error:** Para las implementaciones de SOA con un ESB, este crea un punto único de error. Se trata de un servicio centralizado, que va en contra de la idea de descentralización que defiende la SOA Los clientes y servicios no se pueden comunicar entre sí en lo absoluto si el ESB se cae.
[^Informacion]: https://aws.amazon.com/es/what-is/service-oriented-architecture/
  ------

  ## 🚾**🧮**Principios Básicos de los Patrones Orientados a Servicios(SOA)🧮🚾

<img src="https://blog.seur.com/wp-content/uploads/2012/11/efra.jpg" style="zoom:60%;" />

- ## **Interoperabilidad**
- ## **Acoplamiento Flexible**
- ## **Abstracción**
- ## **Granularidad** 
[^Informacion]: https://aws.amazon.com/es/what-is/service-oriented-architecture/
------

## 🚾**📛**Interoperabilidad📛🚾

<img src="https://cdn-icons-png.flaticon.com/512/7047/7047158.png" style="zoom:57%;" />

Cada servicio en SOA incluye documentos descriptivos que especifican la funcionalidad del servicio, así como las condiciones y términos relacionados. Cualquier sistema de cliente puede ejecutar un servicio, independientemente de la plataforma o el lenguaje de programación subyacente. Por ejemplo, los procesos empresariales pueden utilizar servicios escritos en C# y Python. Dado que no hay interacciones directas, los cambios realizados en un servicio no afectan a otros componentes que lo utilizan.

------

## 🚾🧱Acoplamiento Flexible🧱🚾

<img src="https://cdn.pixabay.com/photo/2014/04/02/14/10/cogwheels-306402_1280.png" style="zoom:37%;" />

Los servicios en SOA deben acoplarse de forma flexible, teniendo tan poca dependencia en recursos externos, como modelos de datos o sistemas de información, como sea posible. También deben prescindir de un estado sin retener ninguna información sobre sesiones o transacciones pasadas. De esta forma, si se modifica un servicio, no afectará de forma significativa a las aplicaciones del cliente ni a otros servicios que utilicen dicho servicio.

------
## 🚾**💻**Abstracción💻🚾

<img src="https://artmiamimagazine.com/wp-content/uploads/2020/09/Abstraccio%CC%81n_Geome%CC%81trica.jpg" style="zoom:57%;" />

Los clientes o usuarios de servicios en SOA no tienen la necesidad de conocer la lógica del código del servicio o los detalles de la implementación. Para ellos, los servicios deben aparecer como una caja negra. Los clientes obtienen la información necesaria sobre lo que hace el servicio y cómo utilizarlo a través de contratos de servicio u otros documentos descriptivos sobre el servicio.

------
## 🚾**📛**Granularidad📛🚾

<img src="https://icloudseven.com/wp-content/uploads/2020/12/desarrollo-software-i-cloud-seven-3.png" style="zoom:57%;" />

Los servicios en SOA deben tener el tamaño y el alcance adecuados; idealmente, deben contar con una función empresarial discreta por servicio. Los desarrolladores, por su parte, pueden utilizar varios servicios para crear un servicio compuesto para que lleve a cabo operaciones complejas

------
## 🚾**♾️**Componentes de los Patrones Orientados a Servicios(SOA)♾️🚾

Existen cuatro componentes principales de la arquitectura orientada a servicios (SOA).

- ## Servicio

- ## Proveedor de Servicios

- ## Consumidor de Servicios

- ## Registros de Servicios

------
## 🚾**📈**Servicio📈🚾

<img src="https://www.manageengine.com/products/service-desk/help-desk-software/images/it-service-desk-software.png" style="zoom:37%;" />

Los servicios son los componentes básicos de la SOA. Pueden ser privados (disponibles únicamente para los usuarios internos de una organización) o públicos (accesibles para todos en Internet). Cada servicio individual tiene tres características principales:

- **Implementación de servicios:** La implementación de servicios es el código que crea la lógica para realizar la función de servicio específica, como la autenticación de usuarios o el cálculo de una factura.
- **Contrato del servicio:** El contrato del servicio define la naturaleza del servicio y sus condiciones y términos asociados, como los prerrequisitos para utilizar el servicio, su costo y la calidad del servicio proporcionado.
- **Interfaz del servicio:** En SOA, otros servicios o sistemas se comunican con un servicio a través de su interfaz. Esta interfaz define la manera en que se puede invocar al servicio para llevar a cabo actividades o intercambiar datos. Reduce las dependencias entre los servicios y quien los solicita. Por ejemplo, incluso los usuarios con poco o nulo entendimiento de la lógica de código subyacente pueden utilizar un servicio a través de su interfaz. 

------
## 🚾**💥**Proveedor de Servicios💥🚾

<img src="https://www.negitec.com/nicaragua/wp-content/uploads/sites/4/2020/05/desarrollo-software.png" style="zoom:57%;" />

El proveedor de servicios crea, mantiene y proporciona uno o más servicios que otros pueden utilizar. Las organizaciones pueden crear sus propios servicios o adquirirlos de proveedores de servicios externos.

------
## 🚾**🎭**Consumidor de Servicios🎭🚾

<img src="https://dyacodeprojects.com/wp-content/uploads/2019/02/Desarrollo-Software-Medida.png" style="zoom:27%;" />

El consumidor de servicios solicita al proveedor de estos poner en marcha un servicio específico. Puede ser un sistema completo, aplicación u otro servicio. El contrato de servicio especifica las reglas que el proveedor y el consumidor de servicios deben seguir al momento de interactuar entre sí. Los proveedores y consumidores de servicios pueden pertenecer a departamentos, organizaciones o incluso sectores diferentes.

------
## 🚾**📛**Granularidad📛🚾

<img src="https://silice.biz/wp-content/uploads/2014/11/software-factory.png" style="zoom:100%;" />

Un registro de servicios, o repositorio de servicios, es un directorio de servicios disponibles accesible a través de redes. Almacena documentos descriptivos sobre el servicio que pertenecen a los proveedores de servicios. Los documentos descriptivos contienen información acerca del servicio y cómo comunicarse con él. Los consumidores de servicios pueden descubrir fácilmente los servicios que necesitan por medio de dicho registro.

[^Informacion]: https://aws.amazon.com/es/what-is/service-oriented-architecture/

------


## 🚾**🎀**Aplicaciones Que Usan Patrones Orientados a Servicios(SOA)🎀🚾

- Sistemas de Comercio Electrónico
- Sistemas de Servicios de Salud
- Sistemas de Transporte y Logística
- Sistemas de Aplicaciones Empresariales
- Sistemas de Telecomunicaciones
- Juegos de Gobierno Electrónico
- Sistemas de Industria Manufacturera

------
> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------