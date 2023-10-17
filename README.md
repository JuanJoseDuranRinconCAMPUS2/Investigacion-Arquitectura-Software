# **⛽📃Patrón Modelo Vista Controlador📃⛽**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-Modelo-Vista-Controlador/imgs/investigacionModeloVistaC.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón de Modelo Vista Controlador.

![](https://i.imgur.com/bV7Z20x.gif)

------

## 🈯**🔑**Patrón Modelo Vista Controlador🔑🈯

<img src="https://www.freecodecamp.org/espanol/news/content/images/2021/06/MVC3.png" alt="Indice" style="zoom:23%;" />

Modelo-vista-controlador (MVC) es un patrón de arquitectura de software, que separa los datos y principalmente lo que es la lógica de negocio de una aplicación de su representación y el módulo encargado de gestionar los eventos y las comunicaciones. Para ello MVC propone la construcción de tres componentes distintos que son el modelo, la vista y el controlador; es decir: por un lado define componentes para la representación de la información y, por otro lado, para la interacción del usuario.

```
Este patrón de arquitectura de software se basa en las ideas de reutilización de código y la separación de conceptos, características que buscan facilitar la tarea de desarrollo de aplicaciones y su posterior mantenimiento.
```

------

## 🈯**🔀**Componentes🔀🈯

![](https://i.imgur.com/t1VeLnK.gif)

- ## **Modelo**:

  - El Modelo representa la capa de datos o la lógica de negocio de la aplicación. Es responsable de la gestión y manipulación de datos, así como de implementar las reglas de negocio.
  - El Modelo notifica a la Vista y al Controlador sobre cualquier cambio en los datos a través de eventos u observadores.
  - De manera ideal, el Modelo no debe estar directamente relacionado con la interfaz de usuario y debe ser independiente de cómo se presenta la información.

- ## **Vista**:

  - La Vista es la capa de presentación de la aplicación. Representa la interfaz de usuario y se encarga de mostrar la información al usuario de una manera comprensible.
  - La Vista también se suscribe a eventos del Modelo para mantener su representación actualizada cuando los datos cambian.
  - En un sistema MVC bien diseñado, puede haber varias Vistas que muestren la misma información de diferentes maneras, lo que facilita la reutilización.

- ## **Controlador**:

  - El Controlador actúa como intermediario entre la Vista y el Modelo. Recibe las interacciones del usuario a través de la Vista y las traduce en acciones en el Modelo.
  - El Controlador es responsable de gestionar la lógica de navegación y de controlar la interacción entre la Vista y el Modelo.
  - No tiene conocimiento directo de la lógica de negocio, sino que coordina cómo los datos fluyen entre la Vista y el Modelo.

------
## 🈯**💥**Beneficios Modelo Vista Controlador💥🈯

<img src="https://codigofacilito.com/photo_generales_store/29.jpg" style="zoom:47%;" />

- **Separación de Responsabilidades**: MVC separa claramente las preocupaciones, lo que facilita la modificación y el mantenimiento de componentes individuales.
- **Reutilización**: Las capas Model y View pueden reutilizarse en diferentes contextos o en múltiples vistas de la misma aplicación.
- **Pruebas Unitarias**: La separación de lógica de negocio (Model) y control de interfaz de usuario (Controlador y Vista) facilita las pruebas unitarias.

------

> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------