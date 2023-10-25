# **🎲📃Patrón "Arquitectura Dirigidas por Eventos"📃🎲**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-Dirigida-Por-Eventos/imgs/investigacionDirigida%20por%20eventos.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón "Arquitectura Dirigidas por Eventos"

![](https://i.imgur.com/t1VeLnK.gif)

------

## 🎟️**🔑**Patrón Dirigidos por Eventos🔑🎟️

<img src="https://cdn-cashy-static-assets.lucidchart.com/marketing/blog/2021Q1/software-architecture-design-best-practices/software-best-practices-cta.png" alt="Indice" style="zoom:100%;" />

La arquitectura basada en eventos utiliza eventos para desencadenar y establecer comunicación entre servicios desacoplados, y es común en las aplicaciones modernas creadas con microservicios. Un evento es un cambio de estado, o una actualización, como un elemento que se coloca en un carro de compras de un sitio web de comercio electrónico. Los eventos pueden llevar el estado (el elemento comprado, su precio y una dirección de entrega) o pueden ser identificadores (una notificación de que se envió una orden)

Las arquitecturas impulsadas por eventos tienen tres componentes clave: procedimientos de eventos, enrutadores de eventos y consumidores de eventos. Un productor publica un evento para el enrutador, que filtra y envía los eventos a los consumidores. Los servicios del productor y los servicios del consumidor se desacoplan, lo que les permite escalarse, actualizarse e implementarse de manera independiente.

## Dato curioso:

Puede utilizar una arquitectura basada en eventos para coordinar sistemas entre equipos que operan y se implementan en diferentes regiones y cuentas. Al utilizar un enrutador de eventos para transferir datos entre sistemas, puede desarrollar, escalar e implementar servicios independientemente de otros equipos.

```js
Sistemas desacoplados que se ejecutan en respuesta a eventos
```
[^Informacion]: https://aws.amazon.com/es/event-driven-architecture/#:~:text=¿Qué%20es%20la%20arquitectura%20basada%20en%20eventos%3F&text=La%20arquitectura%20basada%20en%20eventos%20utiliza%20eventos%20para%20desencadenar%20y,aplicaciones%20modernas%20creadas%20con%20microservicios.
------

🎟️**⚜️**Ventajas del Patrón Dirigido por Eventos⚜️🎟️
------

<img src="https://www.tibco.com/sites/tibco/files/media_entity/2020-05/event-driven-architecture-diagram.svg" />

- **Escalado y errores por separado:** Al desacoplar los servicios, estos solo conocen el enrutador de eventos, no los demás. Esto significa que sus servicios son interoperables, pero si un servicio tiene un error, el resto seguirá funcionando. El enrutador de eventos actúa como un búfer elástico que se adapta a los aumentos repentinos de las cargas de trabajo.
- **Desarrollar con agilidad:** Ya no es necesario escribir código personalizado para sondear, filtrar y enrutar eventos; el enrutador de eventos filtrará y enviará automáticamente los eventos a los consumidores. El enrutador también elimina la necesidad de una fuerte coordinación entre los servicios productores y consumidores, acelerando su proceso de desarrollo.
- **Auditar con facilidad:** Un enrutador de eventos actúa como una ubicación centralizada para auditar su aplicación y definir políticas. Estas políticas pueden restringir quién puede publicar y suscribirse a un enrutador, y controlar qué usuarios y recursos tienen permiso para acceder a sus datos. También puede cifrar sus eventos tanto en tránsito como en reposo.
- **Reducción de costos:** Las arquitecturas basadas en eventos son de tipo push, por lo que todo ocurre bajo demanda cuando el evento se presenta en el enrutador. De este modo, no tiene que pagar por el sondeo continuo para comprobar si hay un evento. Esto significa menos consumo de ancho de banda de la red, menos consumo de CPU, menos capacidad de flota ociosa y menos handshakes SSL/TLS.
[^Informacion]: https://aws.amazon.com/es/event-driven-architecture/#:~:text=¿Qué%20es%20la%20arquitectura%20basada%20en%20eventos%3F&text=La%20arquitectura%20basada%20en%20eventos%20utiliza%20eventos%20para%20desencadenar%20y,aplicaciones%20modernas%20creadas%20con%20microservicios.
------

🎟️**⚠️**Desventajas del Patrón Dirigido por Eventos⚠️🎟️
------

<img src="https://i.pinimg.com/564x/54/81/eb/5481eb653adb22ab8ae8ff8fe5e27432.jpg" style="zoom:80%;" />

- **Complejidad:** EDA puede ser más complejo de configurar y depurar que otros métodos de arquitectura, ya que requiere un monitoreo cuidadoso de eventos y flujos. 

- **Problemas de programación y coordinación:** gestionar la secuencia y sincronización de eventos puede ser un desafío. Garantizar que los eventos se manejen en el orden correcto puede resultar complicado. 

- **Problemas detrás del flujo lógico:** debido al alto nivel de desacoplamiento, el flujo inverso de la lógica de un proceso a otro puede resultar difícil en sistemas complejos. 

- **Operaciones:** en sistemas grandes y muy complejos, la gestión de eventos puede generar costos operativos. Se debe prestar especial atención a la eficiencia y a abordar cuestiones no deseadas. 

- **Desafíos para garantizar la entrega de eventos:** Garantizar que los eventos se entreguen de manera confiable y sin pérdidas puede requerir implementación y desafíos adicionales. 

- **Requiere un modelado de eventos eficaz:** los eventos deben modelarse y documentarse adecuadamente para evitar confusiones y problemas de mantenimiento.

------

  ## 🎟️**🧮**Como Funciona el Patrón Dirigido por Eventos🧮🎟️

<img src="https://d1.awsstatic.com/product-marketing/EventBridge/1-SEO-Diagram_Event-Driven-Architecture_Diagram.b3fbc18f8cd65e3af3ccb4845dce735b0b9e2c54.png" style="zoom:60%;" />

------


## 🎟️**🎀**Aplicaciones Que Usan Patrones Dirigidos por Eventos🎀🎟️

- Sistemas de Replicación de datos entre cuentas y regiones
- Sistemas de Procesamiento en paralelo y distribución ramificada
- Sistemas de Supervisión del estado de los recursos y alertas
- Sistemas de Integración de sistemas heterogéneos

------
> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------