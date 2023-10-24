# **📔📃Patrón Blackboard📃📔**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-En-Pizarra/imgs/investigacionblackboard.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón Blackboard (En pizarra)

![](https://i.imgur.com/72GslRm.gif)

------

## 📈**🔑**Patrón Blackboard 🔑📉

<img src="https://aprendearquitecturasoftware.files.wordpress.com/2018/10/blackboard.png?w=481&h=209" alt="Indice" style="zoom:100%;" />

Consta de múltiples elementos funcionales, denominados **agentes**, y un instrumento de control denominado **pizarra**.

Los agentes están especializados en resolver una tarea concreta. Todos ellos cooperan para alcanzar una meta común, si bien, sus objetivos individuales no están aparentemente coordinados.

## Dato curioso:

Un sistema de pizarra se implementa para resolver problemas en los cuales las entidades individuales se manifiestan incapaces de aproximarse a una solución, o para los que no existe una solución analítica, o para los que si existe pero es inviable por la dimensión del espacio de búsqueda.

## Proceso de Resolución:

<img src="https://i.pinimg.com/564x/01/40/24/014024812e6556a09ffd2f2e2a7d36b9.jpg" style="zoom:50%;" />

Al comienzo del proceso de resolución, se establece el problema en la pizarra. Las fuentes tratan de resolverlo cambiando el estado. La única forma en que se comunican entre sí es a través de la pizarra. Finalmente, si de la cooperación resulta una solución adecuada, ésta aparece en la pizarra como paso final.

```js
El patrón Blackboard es un modelo  arquitectónico de software habitualmente utilizado en sistemas expertos, multiagente y basados en el conocimiento.
```

------

📈**⚜️**Ventajas del Patron Blackboard ⚜️📉
------

<img src="https://aprendearquitecturasoftware.files.wordpress.com/2018/10/1_arbmx7a21i47llvwutisdg.png?w=1100" style="zoom:80%;" />

- **Resolución de Problemas:** Es valioso para resolver problemas complejos o difíciles. 
- **Reusabilidad:** Los diferentes agentes pueden ser reusados en diferentes apartados de la pizarra.
- **Integraciones Reguladas Entre Agentes:** Posibilita la integración de agentes.
- **Flexibilidad y Modularidad:** Los agentes permiten tener flexibilidad y modularidad para el manejo de representación de la información en la pizarra. 
- **Colaboración Distribuida:** Permite que múltiples desarrolladores colaboren en la resolución del problema. Cada persona puede aportar su conocimiento y enfoque especifico.

------

📈**⚠️**Desventajas del Patrón Blackboard ⚠️📉
------

<img src="https://img.freepik.com/vector-premium/icono-error-programa-sistema-operativo-diferentes-dispositivos-simbolos-advertencia-software-roto-computadoras-telefonos-inteligentes-mal-funcionamiento-sistema-operativo-tecnologia-web-sitio-web-no-disponible-concepto-vectorial_533410-3474.jpg?w=360" style="zoom:100%;" />

- **Implementación compleja:** implementar un sistema basado en el modelo Blackboard puede ser complejo y requiere una planificación cuidadosa. Gestionar la asistencia y coordinar a los expertos puede resultar difícil. 
- **Difícil de analizar:** Determinar cuándo se ha encontrado una solución satisfactoria puede resultar difícil, ya que depende de las condiciones de parada definidas. A veces no es fácil establecer normas claras. 
- **Flexibilidad de desempeño:** El desempeño del sistema está sujeto a cambios, ya que depende del soporte y gestión de expertos. En algunos casos, el desempeño puede ser impredecible. 
- **Puede ser necesario el control de versiones:** la gestión de la pizarra y la evolución de los datos pueden requerir control de versiones para realizar un seguimiento de los cambios y permitir la reversión si es necesario. 
- **Requiere expertos calificados:** para que el sistema Blackboard funcione correctamente, se necesitan expertos con experiencia y conocimientos especializados para tomar las decisiones correctas.

------

## 📈**🧮**Estructura de los Patrones Blackboard 🧮📉

<img src="https://aprendearquitecturasoftware.files.wordpress.com/2018/10/blackboard2.jpg" style="zoom:100%;" />

- **Pizarra:** una "pizarra" es una estructura de datos centralizada para almacenar datos distribuidos y semiprocesados. Puede considerarse como un espacio de trabajo colaborativo con información sobre el problema que se está resolviendo. 
- **Expertos (Agentes):** Los "Expertos" son objetos o módulos que aportan su conocimiento y experiencia al sistema. Cada experto es responsable de analizar y procesar una parte de la información en la pizarra y tomar decisiones basadas en su experiencia específica. 
- **Controller (Controller):** El responsable del tratamiento es el responsable de la interoperabilidad entre los expertos. Supervisa el estado de la pizarra, coordina las actividades de los expertos y decide cuando se ha encontrado una solución satisfactoria. 
- **Condición de parada:** Una condición de parada es un criterio que indica cuándo el sistema ha alcanzado una solución aceptable o cuándo debe finalizar la colaboración entre expertos.

------

## 📈**🎀**Aplicaciones Que Usan Patrones Blackboard 🎀📉

- Sistemas de Visión por Computadora
- Sistemas de Diagnósticos Médicos
- Sistemas de Astronomía
- Sistemas de Optimización y Planificación
- Sistemas de Traducción automática
- Juegos de Estrategias
- Sistemas de Recomendación

------
> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------