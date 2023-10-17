# **⛽📃Patrón Cliente Servidor📃⛽**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-Cliente-Servidor/imgs/investigacionCliente%20Servidor.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón de Cliente Servidor.

![](https://i.imgur.com/EMHS3Qr.gif)

------

## 🉑**🔑**Patrón Cliente Servidor🔑🉑

<img src="https://definicion.de/wp-content/uploads/2016/10/cliente-servidor.png" alt="Indice" style="zoom:53%;" />

La **arquitectura cliente-servidor** es un modelo de diseño de software en el que las tareas se reparten entre los proveedores de recursos o servicios, llamados **servidores**, y los demandantes, llamados **clientes**. Un cliente realiza peticiones a otro programa, el **servidor**, quien le da respuesta. Esta idea también se puede aplicar a programas que se ejecutan sobre una sola computadora, aunque es más ventajosa en un sistema operativo **multiusuario** distribuido a través de una **red de computadoras**.

[^Cita]: https://es.wikipedia.org/wiki/Cliente-servidor

```
Divide la aplicación en dos partes principales: el cliente, que solicita servicios o recursos, y el servidor, que proporciona esos servicios o recursos.
```

------

## 🉑**🔀**Caracteristicas Cliente Servidor🔀🉑

![](https://i.imgur.com/HgCjMI5.gif)

- El cliente envía solicitudes al servidor, que las procesa y devuelve las respuestas correspondientes.
- Las funciones de Cliente y Servidor pueden estar en plataformas separadas, o en la misma plataforma.
- La comunicación entre el cliente y el servidor suele ocurrir a través de protocolos estándar como HTTP, TCP/IP o protocolos personalizados.

------
## 🉑**💥**Beneficios Cliente Servidor💥🉑

<img src="https://assets.isu.pub/document-structure/230205193406-0d454d6653332600c4a7ac6ca45dce8a/v1/bacf44297dd72e376a5038a3d968d2d9.jpeg" style="zoom:87%;" />

- **Escalabilidad**: El enfoque Cliente-Servidor permite escalar el sistema de manera eficiente al agregar más clientes o servidores según sea necesario.
- **Reutilización de Recursos**: Los servidores centralizados pueden administrar recursos compartidos, lo que evita la duplicación de datos y funcionalidad.
- **Separación de Responsabilidades**: Al estar distribuidas las funciones y responsabilidades entre varios ordenadores independientes, es posible reemplazar, reparar, actualizar, o incluso trasladar un servidor, mientras que los clientes no se verán afectados por ese cambio (o se afectarán mínimamente).
- **Fácil mantenimiento**: Los clientes y servidores pueden ser implementados en diferentes tecnologías y plataformas, lo que permite una mayor flexibilidad.

------

> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------