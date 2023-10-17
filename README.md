# **⛽📃Patrón Arquitectura de tres niveles📃⛽**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-Arquitectura-Tres-Niveles/imgs/investigacion3niveles.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón de Arquitectura de tres niveles.

![](https://i.imgur.com/7ud53ww.gif)

------

## 🈹**🔑**Patrón Arquitectura de tres niveles🔑🈹

<img src="https://upload.wikimedia.org/wikipedia/commons/e/ea/Tres_capas.PNG" alt="Indice" style="zoom:93%;" />

La arquitectura de tres niveles es un patrón de arquitectura de software que divide una aplicación en tres capas lógicas distintas, cada una con sus propias responsabilidades.

```
Este enfoque promueve la modularidad, la escalabilidad y la mantenibilidad de un sistema de software.
```

------

## 🈹**🔀**Capas y Niveles🔀🈹

![](https://i.imgur.com/HgCjMI5.gif)

- ## Capa de presentación: 

  Es la que ve el usuario presenta el sistema al usuario, le comunica la información y captura la información del usuario en un mínimo de proceso (realiza un filtrado previo para comprobar que no hay errores de formato). También es conocida como interfaz gráfica y debe tener la característica de ser **amigable** para el usuario. Esta capa se comunica únicamente con la capa de negocio.

- ## Capa de negocio: 

  Es donde residen los programas que se ejecutan, se reciben las peticiones del usuario y se envían las respuestas tras el proceso. Se denomina capa de negocio porque es aquí donde se establecen todas las reglas que deben cumplirse. Esta capa se comunica con la capa de presentación, para recibir las solicitudes y presentar los resultados, y con la capa de datos, para solicitar al gestor de base de datos almacenar o recuperar datos de él. También se consideran aquí los programas de aplicación.

- ## Capa de datos: 

  Es donde residen los datos y es la encargada de acceder a los mismos. Está formada por uno o más gestores de bases de datos que realizan todo el almacenamiento de datos, reciben solicitudes de almacenamiento o recuperación de información desde la capa de negocio.

------
## 🈹**💥**Beneficios Arquitectura de tres niveles💥🈹

<img src="https://i0.wp.com/www.disrupciontecnologica.com/wp-content/uploads/2019/09/TresCapasNivel.png?resize=337%2C349&ssl=1" style="zoom:87%;" />

- **Modularidad**: La división en tres capas permite separar las preocupaciones y simplifica el diseño y la gestión de la aplicación.
- **Escalabilidad**: Cada capa puede escalarse de manera independiente, lo que facilita la gestión del rendimiento.
- **Mantenibilidad**: Los cambios en una capa no afectan directamente a las otras capas, lo que facilita las actualizaciones y el mantenimiento.
- **Reutilización**: Las capas se pueden reutilizar en diferentes aplicaciones o proyectos, ya que están bien definidas y aisladas.
- **Seguridad**: Al separar la lógica de negocio y la capa de acceso a datos, se pueden implementar estrategias de seguridad específicas para cada capa.

------

> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------