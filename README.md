# **✨📃Patrón Peer  To Peer (P2P)📃✨**

![Portada](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/blob/Patron-Entre-Pares/imgs/investigacionP2P.png?raw=true)

En esta rama, exploraremos de uno de los patrones de arquitectura de software, siendo especifico el patrón Peer  To Peer (P2P)

![](https://i.imgur.com/bV7Z20x.gif)

------

## ❇️**🔑**Patrón Peer  To Peer (P2P)🔑❇️

<img src="https://www.mybeepy.com/info/wp-content/uploads/2022/09/p2p-1024x580.png" alt="Indice" style="zoom:53%;" />

Es una red de computadoras donde todos los dispositivos conectados a la red actúan como cliente y servidor a la vez. En este patrón no es necesario un servidor central que administre la, sino que todos los nodos de la red pueden comunicarse uno con otros.

## Dato curioso:

Aunque parezca que el patrón P2P es una versión del patrón Cliente-Servidor, la diferencia entre ambos es que la estructura Cliente-Servidor se fundamenta en la centralización mientras que la P2P se fundamenta en la descentralización.



```js
Las redes P2P son conocidas por su descentralización y su capacidad para distribuir la carga de manera equivalente entre los clientes.
```

------

❇️**⚜️**Ventajas del Patron Peer To Peer (P2P)⚜️❇️
------

<img src="https://i.pinimg.com/564x/6e/e5/fc/6ee5fcd5e3a61cd48f4bc70d68dfeebe.jpg" style="zoom:80%;" />

- **Descentralización:** Eliminar un servidor central permite tolerancia a fallos y gastos generales. Si un nodo falla, los demás pueden seguir funcionando. 
- **Escalabilidad:** Las redes P2P pueden escalar bien a medida que se agregan más nodos, lo que las hace adecuadas para aplicaciones más grandes. Asignación eficiente de recursos: recursos como el ancho de banda y el almacenamiento se asignan y distribuyen de manera eficiente entre los pares de la red, lo que puede reducir los costos de infraestructura. 

- **Anonimato y privacidad:** En algunas redes P2P, como las redes de intercambio de archivos, los usuarios pueden mantener cierto anonimato y privacidad. 
- **Redundancia y tolerancia a fallos:** La distribución de datos entre varios nodos proporciona redundancia y mejora la tolerancia a fallos. Los datos siguen estando disponibles incluso si algunos nodos fallan. 
- **Menor costo de infraestructura:** La falta de servidores centralizados y la capacidad de compartir recursos entre clientes puede reducir los costos de infraestructura en comparación con las arquitecturas centralizadas.

------

❇️**⚠️**Desventajas del Patron Peer To Peer (P2P)⚠️❇️
------

<img src="https://i.pinimg.com/564x/47/e9/61/47e9617d5d16214f0d08558539214936.jpg" style="zoom:80%;" />

- **Complejidad de rendimiento y comunicación:** No tener un centro de control central puede generar complejidad en la infraestructura de red y las comunicaciones, lo que puede generar problemas de rendimiento y seguridad. 
- **Seguridad y privacidad:** En algunas aplicaciones P2P, los usuarios pueden ser vulnerables a riesgos de seguridad y privacidad debido a la dificultad de confiar en sus pares. 
- **Ancho de banda limitado:** Según la red y la aplicación, las velocidades de transferencia y la calidad de la conexión pueden depender del ancho de banda de igual a igual disponible. 
- **Puede usarse para actividades ilegales:** Algunas redes P2P se han utilizado para compartir material protegido por derechos de autor y realizar actividades ilegales, lo que ha dado lugar a controversias y demandas. 
- **Complejidad del enrutamiento:** El enrutamiento de datos en una red P2P puede ser complejo y se requieren algoritmos eficientes para ubicar nodos y recursos de manera eficiente. 
- **Desafíos de implementación:** En aplicaciones empresariales y gubernamentales, puede resultar difícil implementar medidas de seguridad y cumplimiento en redes P2P.
- **Tráfico**: En redes no optimizadas como las no estructuradas, podemos saturar la red con una gran cantidad de tráfico para propagar las peticiones a los nodos adyacentes.

------

## ❇️**🧮**Tipos de Patrones Peer To Peer (P2P)🧮❇️

<img src="https://2.bp.blogspot.com/-Epb5SbMR41o/V_MYgLjdH4I/AAAAAAAAAH4/JZBSJyPWyH820X0DPGotsAI0MfWnP1JGACLcB/w1200-h630-p-k-no-nu/software.png" style="zoom:70%;" />

A pesar de ser un patrón que se fundamenta en la descentralización existen algunas variantes de este patrón que sí requieren un servidor central, con esto en mente existe una clasificación básica para los patrones P2P:

- Arquitectura P2P Pura Estructurada
- Arquitectura P2P Pura No Estructurada
- Arquitectura P2P Hidrida

------

## ❇️**🕳️**Arquitectura P2P No Pura Estructurada🕳️❇️

Este tipo de arquitectura conforman una red totalmente descentralizada, donde no existe un servidor central ni roles donde algún nodo de la red tenga más privilegios o responsabilidades, además, todos los pares actúan como cliente y servidor al mismo tiempo, estableciendo una comunicación simétrica entre sí.

En esta arquitectura un par solo se puede comunicar con los pares que conozca, es decir, que conoce la ubicación exacta. Ha estos pares conocidos se le conoce como vecinos, por lo que cada par puede tener un número de vecinos diferentes:

<img src="https://reactiveprogramming.io/_next/image?url=%2Ffigures%2Fp2p-vecinos.png&w=640&q=75" style="zoom:80%;" />

[Informacion]: https://reactiveprogramming.io/blog/es/estilos-arquitectonicos/p2p	"Informacion sacada de:"

------

## ❇️**💫**Arquitectura P2P Pura Estructurada💫❇️

La arquitectura P2P estructurada es una variante de la P2P no estructurada, por lo que mucho de la teoría planteada anteriormente aplica exactamente igual, sin embargo, la arquitectura P2P estructurada cambia la forma de buscar los recursos. En lugar de usar el método por inundación, busca los recursos basados en Tablas Hash Distribuidas (DHT por sus siglas en inglés).

Esta tabla hash mantiene un registro de todos los recursos disponibles en la red en un formato Clave-Valor (Key-Value), donde la clave es un hash del recurso y el valor corresponde a la ubicación (nodo) donde se encuentra el recurso, de esta forma, solo es necesario buscar el clave hash del recurso en la tabla para conocer su ubicación, sin embargo, no están fácil como parece. Debido a que la tabla hash es distribuida, no existe físicamente un solo servidor, sino que está distribuida entre todos los nodos de la red, y cada nodo guarda un fragmento del índice total de los recursos compartidos.

<img src="https://reactiveprogramming.io/_next/image?url=%2Ffigures%2Fp2p-pura-estructurada.png&w=750&q=75" style="zoom:80%;" />
[Informacion]: https://reactiveprogramming.io/blog/es/estilos-arquitectonicos/p2p	"Informacion sacada de:"

------

## ❇️**♾️**Arquitectura P2P Hidrida♾️❇️

La arquitectura P2P híbrida o también conocida como Centralizada se caracteriza por tener un servidor central que sirve de enlace entre los nodos de la red, de tal forma que cualquier solitud para consumir los recursos de otros nodos deberán pasar primero por este servidor.

**La diferencia fundamental que tiene esta arquitectura con el Cliente-Servidor** es que, este servidor no es el que proporciona los recursos, sino que solo sirve de enlace para conectar con otros nodos.

<img src="https://reactiveprogramming.io/_next/image?url=%2Ffigures%2Fp2p-hibrida.png&w=640&q=75" style="zoom:80%;" />

[Informacion]: https://reactiveprogramming.io/blog/es/estilos-arquitectonicos/p2p	"Informacion sacada de:"

------

## ❇️**🎀**Aplicaciones Que Usan Patrones Peer To Peer (P2P)🎀❇️

- Aplicaciones de Intercambios de Archivo
- Aplicaciones de Streaming de Contenido Multimedia
- Criptomonedas
- Juegos en Linea
- Sistemas de Almacenamiento Distribuido
- Comunicación entre Pares

------
> ## [Volver a la lista de patrones](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/Patrones-Arquitectura-Software)
>
> ## [Volver al índice](https://github.com/JuanJoseDuranRinconCAMPUS2/Investigacion-Arquitectura-Software/tree/main)

------